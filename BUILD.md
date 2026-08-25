# How to build this course (site + slides)

Everything here was verified working on this Mac in August 2026. The awkward part is that
**none of the required tools are on your `PATH` by default** — they live inside a conda
environment, inside RStudio.app, and in `~/Library/TinyTeX`. Every command below sets `PATH`
explicitly for that reason. If a build fails with "command not found" or "pandoc version …
is required", you almost certainly skipped the `export PATH` line.

## The toolchain

| Tool | Where it actually lives | Why |
|---|---|---|
| **R 4.5.2** | `/opt/homebrew/anaconda3/envs/eco3253/bin/R` | The `eco3253` conda env. Has `bookdown`, `pacman`, `tidyverse`. The *system* R at `/usr/local/bin/R` is 4.4.3 and is **missing `pacman`** — the book build dies on `03-getting-started.Rmd` with it. |
| **pandoc 3.8.3** | `/opt/homebrew/anaconda3/envs/eco3253/bin/pandoc` | Same env. Not installed system-wide; `bookdown` fails without it. |
| **quarto 1.5.57** | `/Applications/RStudio.app/Contents/Resources/app/quarto/bin/quarto` | Bundled with RStudio; there is no standalone `quarto` on this machine. Only needed for slides. |
| **XeLaTeX** | `~/Library/TinyTeX/bin/universal-darwin/` | The slide decks are Beamer → PDF. |

Set this once per shell and both builds below work:

```bash
export PATH="/opt/homebrew/anaconda3/envs/eco3253/bin:$HOME/Library/TinyTeX/bin/universal-darwin:$PATH"
```

## Build the website (bookdown)

The published site is the `docs/` folder on `main`, served by GitHub Pages. **Pushing a rebuilt
`docs/` is what updates the live site** — editing an `.Rmd` alone changes nothing publicly.

```bash
cd "path/to/2026-2/ECO3253_fall2026"
export PATH="/opt/homebrew/anaconda3/envs/eco3253/bin:$PATH"
rm -f _main.Rmd                      # stale merge file confuses bookdown
Rscript -e "bookdown::render_book('index.Rmd')"
```

Takes a few minutes (522 chunks). Then:

```bash
git add -A && git commit -m "Rebuild site" && git push origin main
```

GitHub Pages takes **1–3 minutes after the push** to serve the new build, and it caches. To
confirm the deploy actually landed rather than trusting the push:

```bash
curl -s -H 'Cache-Control: no-cache' -L https://jrm87.github.io/ECO3253_fall2026/schedule.html | grep -c "10/06"
```

Non-zero means the new build is live.

## Build the slides (quarto → beamer)

Each deck is `slides/<name>/<name>.qmd` and renders to a PDF beside it. About 15 s per deck.

```bash
export PATH="/opt/homebrew/anaconda3/envs/eco3253/bin:$HOME/Library/TinyTeX/bin/universal-darwin:$PATH"
Q="/Applications/RStudio.app/Contents/Resources/app/quarto/bin/quarto"

# one deck
cd slides/01-intro && "$Q" render 01-intro-slides.qmd --to beamer

# all decks
cd slides
for d in */; do
  q=$(ls "$d"*.qmd 2>/dev/null | head -1); [ -z "$q" ] && continue
  (cd "$d" && "$Q" render "$(basename "$q")" --to beamer) \
    && echo "OK ${d%/}" || echo "FAIL ${d%/}"
done
```

The slide PDFs are committed to the repo but are **not** part of the website build — the site
does not link to them. Rebuilding slides does not require rebuilding the book, or vice versa.

## Things that have bitten us

- **Two `9_` readings.** `readings/` contains both `9_clemens_…` and `9_tabellini_…`. When
  refreshing Canvas file IDs, do not assume one ID per number prefix.
- **Canvas IDs are per-course.** Copying a Canvas course reassigns every file and assignment ID.
  A link like `courses/<id>/files/folder/papers?preview=<file_id>` needs **both** numbers
  updated; changing only the course ID yields a link that loads the folder but not the paper.
  Current course is **92072**. The ID map lives in `../INSTRUCTOR_NOTES_fall2026.md`.
- **Data URLs point at this repo.** Chapters and decks load `.rds` files over the network from
  `raw.githubusercontent.com/jrm87/ECO3253_fall2026/main/…`. If you rename or make the repo
  private, **every build breaks** and so does any student running the code. The retired
  `jrm87/ECO3253_repo` is gone; do not reintroduce references to it.
- **Don't build in `/tmp`.** macOS wiped `/private/tmp` mid-session once and took an in-progress
  clone with it. Build in place, in Drive.
- **Google Drive is slow for git.** A `git status` in the Drive copy can hang for minutes while
  Drive hydrates placeholder files. It finishes; be patient rather than killing it.

## Semester rollover checklist

> This covers only the **code** side. For the parts that need Jon's hands or Jon's answers
> — Canvas course/file/assignment IDs, pasting site links into Canvas assignment
> descriptions, iClicker setup, unpublishing the old site — see
> **`Public Econ/SEMESTER_ROLLOVER.md`**.

When you clone this for the next term:

1. `ECO3253_fall2026` → new repo name in `index.Rmd`, `_output.yml`, `README.md`, `CLAUDE.md`,
   and every `raw.githubusercontent.com` data URL in `*.Rmd` and `slides/*/*.qmd`.
2. Semester strings in `index.Rmd` (`subtitle`, `description`) and `_output.yml`.
3. `00-schedule.Rmd` — rebuild the whole table for the new calendar.
4. Canvas course ID **and** every file/assignment ID (see above).
5. Grade weights appear in **three** places: the syllabus table, the syllabus prose
   ("Projects 0–4 (12%)"), and the `## Grades` slide in `slides/01-intro/`. Update all three.
6. Meeting time and room appear **twice** in the syllabus (Attendance section and Course Format
   section). Update both.
7. Rebuild the book *and* the slides, then push.

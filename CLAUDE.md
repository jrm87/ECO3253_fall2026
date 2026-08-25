# CLAUDE.md

## Primary task

Help Jon keep the **ECO 3253 — Economics of Public and Social Issues** course site updated. Day-to-day work falls into three buckets:

1. **Site maintenance** — fix broken links, update deadlines, refresh data URLs, correct typos in `index.Rmd`, `00-schedule.Rmd`, the `project*.Rmd` files, and the chapter/tutorial Rmds listed in `_bookdown.yml`.
2. **New lectures** — draft new chapters or expand existing ones (`02-causaleff-neigh.Rmd`, `03-mto-placebased.Rmd`, `04-mob-hist-int.Rmd`, `05-mob-ed.Rmd`, `06-ed-higher.Rmd`, `07-k12.Rmd`, `08-teachers-charters.Rmd`, `09-race-ineq.Rmd`, `10-criminal-justice.Rmd`, etc.).
3. **Slides** — update or create new slide decks under `slides/`.

The published site lives at <https://jrm87.github.io/ECO3253_fall2026/> and is served from the `docs/` folder on the `main` branch via GitHub Pages. Pushing a rebuilt `docs/` to `main` is what updates the live site (a few minutes after push).

## Repository layout

- `index.Rmd` — landing page; also the file you pass to `bookdown::render_book()`
- `_bookdown.yml` — **the source of truth for which Rmds end up in the site**. Any `.Rmd` not listed here is invisible to the build. If you add a new chapter, add it here.
- `_output.yml` — output format / theme settings
- `00-schedule.Rmd`, `01-intro.Rmd`, `02-…` through `10-…`, `91-appendixA.Rmd`, `project0–4.Rmd` — current chapters in the book
- `data/`, `rds/` — local copies of course datasets (the canonical remote copies live at `https://raw.githubusercontent.com/jrm87/ECO3253_fall2026/main/data/...` and are loaded with `readRDS(gzcon(url(...)))`)
- `images/`, `slides/` — figures and lecture slides
- `docs/` — **generated output**, committed to git, served by GitHub Pages. Don't hand-edit; rebuild instead.
- `book.bib`, `packages.bib` — bibliography

## Building the site

> See **[BUILD.md](BUILD.md)** for the full toolchain (R, pandoc, quarto, TinyTeX — none of
> which are on `PATH` by default), how to build the **slide decks**, how to verify a Pages
> deploy actually landed, and the semester-rollover checklist.

Use the `eco3253` conda env. The trick is that `Rscript` needs the env's `pandoc` on `PATH`, otherwise it errors with "pandoc version 1.12.3 or higher is required":

```bash
PATH="/opt/homebrew/anaconda3/envs/eco3253/bin:$PATH" \
  /opt/homebrew/anaconda3/envs/eco3253/bin/Rscript -e \
  "setwd('/Users/hql910/Library/CloudStorage/GoogleDrive-mm.jonmore@gmail.com/My Drive/UTSA/Teaching/Public Econ/2026-2/ECO3253_fall2026'); bookdown::render_book('index.Rmd')"
```

A full render takes a few minutes and writes everything to `docs/`. Always rebuild before committing site-affecting changes — the live site reflects whatever is in `docs/` on `main`.

The `conda run -n eco3253 …` form documented in `README.md` does not work here because it strips the env's `PATH` entries that R needs to find pandoc. Use the `PATH=…` form above.

## Standard workflow for site changes

1. Edit the relevant `.Rmd` (or `_bookdown.yml`, `style.css`, `book.bib`, etc.).
2. Rebuild with the command above.
3. Sanity-check `docs/` for the file that should have changed (`docs/project3.html`, `docs/index.html`, …).
4. `git add` the edited Rmd(s) **and** the touched files in `docs/` together.
5. Commit and push. After a few minutes, verify on <https://jrm87.github.io/ECO3253_fall2026/>.

## Conventions and gotchas

- **Data URLs** must point at `https://raw.githubusercontent.com/jrm87/ECO3253_fall2026/main/data/<file>`. The old `jrm87/ECO3253_repo` repo is gone — never use it. The `jrm87/ECO3253_fall2023` repo still works but prefer the fall2026 one for consistency.
- **`07-ml.Rmd` is gone** as of April 2026 (it was leftover ModernDive content). If a future ML chapter is needed, write a new one with course-specific content and add it to `_bookdown.yml`.
- **Cross-references** (`\@ref(label)`) only resolve to chapters listed in `_bookdown.yml`. After a render, look at the build output for `WARNING ... label(s) ... not found` lines.
- **Don't commit secrets** — Canvas links (`utsa.instructure.com/courses/92072/...`) are fine to commit, they require login to actually access.
- Conda env name is `eco3253`. R lives at `/opt/homebrew/anaconda3/envs/eco3253/bin/Rscript`.
- The course site is built for students — when fixing or adding content, prefer clarity and concrete examples over jargon. Jon teaches Tue/Thu 2:30–3:45 pm in McKinney Humanities 2.01.08; Fall 2026 classes began
  August 19, 2026 (first meeting Thu 08/20) and the last class is Thu 12/03. Weekly quizzes run
  in iClicker at the start of each Thursday class.

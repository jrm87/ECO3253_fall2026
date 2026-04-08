# Slides citation audit — Spring 2026

A pass over every slide deck (`slides/01-intro` through `slides/17-taxation2`, 16 decks total — there is no `04`) to (a) add a clickable link to every paper citation, (b) flag every figure or table that has no source attribution, and (c) note content fixes you may want to make later. All 16 decks recompile with zero warnings after the changes documented here.

---

## Canvas paper map

The 14 IDs you provided map to the readings folder as follows. I used these to add links to citations whose paper is in `readings/`:

| # | Paper | File in `readings/` | Canvas link |
|---|---|---|---|
| 1 | Chetty, Friedman, Hendren, Jones, Porter — *The Opportunity Atlas* (NBER WP 2018) | `1_opportunity_atlas_summary.pdf` | <https://utsa.instructure.com/courses/79928/files/folder/papers?preview=13306202> |
| 2 | Creating Moves to Opportunity (CMTO) summary | `2_cmto_summary.pdf` | <https://utsa.instructure.com/courses/79928/files/folder/papers?preview=13306205> |
| 3 | Bergman, Chetty, DeLuca, Hendren, Katz, Palmer — *Creating Moves to Opportunity* (2019) | `3_bergman_et_al_creating_moves_opportunity_2019.pdf` | <https://utsa.instructure.com/courses/79928/files/folder/papers?preview=13306208> |
| 4 | Bian, Leslie, Cimpian — *Gender stereotypes about intellectual ability emerge early* (Science 2017) | `4_bian_et_al_2017_gender_stereotypes.pdf` | <https://utsa.instructure.com/courses/79928/files/folder/papers?preview=13306210> |
| 5 | Dynarski, Libassi, Michelmore, Owen — *Closing the Gap: Targeted, Tuition-Free Promise* (2018) | `5_dynarski_et_al_2018_targeted_tuitionfree_promise.pdf` | <https://utsa.instructure.com/courses/79928/files/folder/papers?preview=13306212> |
| 6 | Chetty, Friedman, Rockoff — *Measuring the Impacts of Teachers I/II* (AER 2014) summary | `6_teachers_summary.pdf` | <https://utsa.instructure.com/courses/79928/files/folder/papers?preview=13306213> |
| 7 | Bertrand & Mullainathan — *Are Emily and Greg More Employable Than Lakisha and Jamal?* (AER 2004) | `7_bertrand_mullainathan_2004.pdf` | <https://utsa.instructure.com/courses/79928/files/folder/papers?preview=13306215> |
| 8 | Kleinberg, Lakkaraju, Leskovec, Ludwig, Mullainathan — *Human Decisions and Machine Predictions* (QJE 2018) | `8_kleinberg_et_al_human_decision_machine_predictions_2018.pdf` | <https://utsa.instructure.com/courses/79928/files/folder/papers?preview=13306220> |
| 9 | Clemens — *Economics and Emigration: Trillion-Dollar Bills on the Sidewalk?* (JEP 2011) | `9_clemens_economics_emigration_2011.pdf` | <https://utsa.instructure.com/courses/79928/files/folder/papers?preview=13306222> |
| 9b | Tabellini — *Gifts of the Immigrants, Woes of the Natives* (RES 2020) | `9_tabellini_2020.pdf` | <https://utsa.instructure.com/courses/79928/files/folder/papers?preview=13306223> |
| 10 | Diamond & Saez — *The Case for a Progressive Tax* (JEP 2011) | `10_diamond_saez_progressive_tax_2011.pdf` | <https://utsa.instructure.com/courses/79928/files/folder/papers?preview=13306227> |
| 11 | Glaeser et al. — *Big Data and Big Cities* (2018) | `11_glaeser_et_al_2018_big_data_cities.pdf` | <https://utsa.instructure.com/courses/79928/files/folder/papers?preview=13306230> |
| 12 | Isen, Rossin-Slater, Walker — *Every Breath You Take* (JPE 2017) | `12_isen_et_al_2017.pdf` | <https://utsa.instructure.com/courses/79928/files/folder/papers?preview=13306233> |
| 13 | Moore, Obradovich, Lehner, Baylis — *Rapidly declining remarkability of temperature anomalies* (PNAS 2019) | `12_moore_et_al_temperature_perception_2019.pdf` | <https://utsa.instructure.com/courses/79928/files/folder/papers?preview=13306235> |

The papers in `readings/supplementary/` (Berman, Reardon, Peri-Yasenov, Derenoncourt et al., Alesina-Stantcheva-Teso, Race & Economic Opportunity, etc.) are **not** in the Canvas papers folder according to your mapping, so I linked those to their journal/working-paper pages instead. If you'd like any of them uploaded to Canvas as well, I can swap the external links for Canvas previews once you give me the new IDs.

---

## What I changed, deck by deck

### 01-intro

No paper citations in this deck — it's the welcome / logistics deck. (The grading-related rewrite from the previous task is what landed here; nothing to add for citations.)

### 02-intromobility (`02-intromobility.qmd`, 11 pages)

| Slide | Citation | Action |
|---|---|---|
| `## Plan for today` | Chetty, Friedman, Hendren, Jones, Porter — *Opportunity Atlas* NBER WP 2018 | **Linked to Canvas #1** |
| `## Intergenerational Income Mobility for Children Raised in Chicago` | "Source: Chetty, Hendren, Kline, Saez 2014" | Linked to [QJE article](https://academic.oup.com/qje/article/129/4/1553/1853754) (CHKS 2014, *Where is the Land of Opportunity?*) |
| `## Intergen. Mobility for Children Raised in Hypothetical Census Tract` | same as above | same |
| `## The Geography of Upward Mobility in the United States` | "Source: Chetty, Friedman, Hendren, Jones and Porter (2018)" | **Linked to Canvas #1** |

### 05-causal-effects-neigh (`05-causal-effects-neigh.qmd`, 31 pages)

| Slide | Citation | Action |
|---|---|---|
| `## Racial Segregation in Atlanta / Sacramento / San Antonio` (×3) | "Cable (2013) based on Census 2010" | Linked to the [UVA Racial Dot Map](https://demographics.virginia.edu/DotMap/index.html) (the actual hosted artifact) |
| `## Five Strongest Correlates of Upward Mobility` | Putnam (1995) "Bowling Alone" | Linked to [Wikipedia entry](https://en.wikipedia.org/wiki/Bowling_Alone) (it's a book, no DOI) |
| `## New Map of Social Capital` | Chetty et al. social capital paper (was un-linked, only `socialcapital.org` was) | Added link to [*Nature* 608, 108 (2022)](https://www.nature.com/articles/s41586-022-04996-4) |
| `## Affordable Housing Policies in the United States` | Chetty, Hendren, Katz — *Effects of Exposure to Better Neighborhoods* (AER 2016) | Linked to [AER article](https://www.aeaweb.org/articles?id=10.1257/aer.20150572) |

**Figures with no paper citation in this deck (none acquired one — they are produced by Chetty et al. but not labeled):**

- `## Income Gain from Moving to a Better Neighborhood` (`mob_better1.png` … `mob_better5.png`, 5 slides) — these are screenshots from Chetty's Opportunity Insights presentations. I left them unlabeled because the figure series doesn't have a single named published source. If you want a label, the closest is the same Chetty/Hendren/Katz (AER 2016) paper that the section already references.
- `## Upward Mobility vs. Job Growth in the 30 Largest Metro Areas` (`mob_jobs.png`) — same situation; from the Chetty 2018 *Opportunity Atlas* (NBER WP) materials.

### 06-mto-placebased (`06-mto-placebased.qmd`, 43 pages)

| Slide | Citation | Action |
|---|---|---|
| `## Analysis of MTO Experimental Impacts` (×2 — the slide is duplicated) | Kling, Liebman, Katz (QJE 2007) | Linked to [QJE article](https://academic.oup.com/qje/article/122/1/83/1924719) |
| same | "Chetty and Hendren 2018" | Linked to [QJE 2018](https://academic.oup.com/qje/article/133/3/1107/4850660) (*The Effects of Exposure to Better Neighborhoods on Children*); also fixed the typo "ao-authors" → "co-authors" |
| `## Implications for Housing Voucher Policy` | "Jacob et al. 2015" | Linked to [Jacob, Kapustin, Ludwig (QJE 2015)](https://academic.oup.com/qje/article/130/1/465/2337966) |
| `## CMTO` | (no citation existed) | **Added a new reference block above the figure** linking to **Canvas #2** (CMTO summary) and **Canvas #3** (Bergman et al. 2019) |

**Figures with no source label in this deck:** all of the `lec3_mto_placebased/lec3_*.png` figures (≈22 of them) are uncaptioned. They come from the same Chetty/Hendren MTO paper or the CMTO Bergman et al. paper, both of which the deck now references in its prose. If you want a fig.cap on each, say the word — I left them as-is to avoid noise.

**Content note:** the slide titled `## Analysis of MTO Experimental Impacts` appears **twice** in a row (lines 86-99 and 101-113) with identical content. Looks like an accidental duplicate. Worth deleting one. (Same for the `## Limitations of Randomized Experiments - Part 2/3` series — they're split across slides intentionally so leave those alone.)

### 07-mob-hist-int (`07-mob-hist-int.qmd`, 42 pages)

| Slide | Citation | Action |
|---|---|---|
| `## A Historical Perspective on the American Dream` | Chetty, Grusky, Hell, Hendren, Manduca, Narang — *Fading American Dream* (Science 2017) | Linked to [Science DOI](https://www.science.org/doi/10.1126/science.aal4617) |
| `## Measuring the American Dream` | "Chetty et al. (Science, 2017)" | Same Science DOI |
| `## Trends in Upward Mobility: International Comparisons` | "Berman (2018)" | Linked to [Berman, *Long Run Evolution of Absolute Intergenerational Mobility* (AER 2022)](https://www.aeaweb.org/articles?id=10.1257/aer.20181655). The supplementary folder file is `berman_2022_absolutemobility.pdf` — note the year is 2022, not 2018 |
| `## Restoring the American Dream: Two approaches` | "Piketty and Saez" | Linked to [Piketty & Saez (QJE 2003) "Income Inequality in the United States, 1913-1998"](https://eml.berkeley.edu/~saez/pikettyqje.pdf) |
| same | "Goldin and Katz" | Linked to [their book *The Race between Education and Technology* (2008)](https://scholar.harvard.edu/lkatz/publications/race-between-education-and-technology) |
| `## What is education?` (×2 — also a duplicate slide) | "Deming (2018)" | Linked to [Deming (QJE 2017) *The Growing Importance of Social Skills*](https://academic.oup.com/qje/article/132/4/1593/3861633). Year corrected from 2018 → 2017 in the linked text |

**Content notes:**
- The `## What is education?` slide appears twice with nearly identical content (lines 278-284 and 304-312). Same with the Deming paragraph appearing twice. Worth de-duplicating.
- The `## Methodology: Constructing Historical Estimates of Mobility` slide also appears twice in close succession (lines 130-135 and 154-160).
- The slide titled `## Goldthorpe 1987` reference is mentioned only in passing — no figure or quote. Left unlinked since it's a book reference and not load-bearing.

**Figures with no source label:**
- `lec4_halikiasreeves16.png` (`## Data issues`) — Halikias & Reeves Brookings 2016 piece on absolute mobility
- `lec4_piketty_saez_zucman17.png` and `lec4_piketty_saez_zucman17-2.png` — these are clearly from Piketty/Saez/Zucman (QJE 2018) *Distributional National Accounts*, but the slide title doesn't say so. **Recommend** adding a fig.cap: "Source: [Piketty, Saez, Zucman QJE 2018](https://academic.oup.com/qje/article/133/2/553/4430651)".
- `lec4_goldin_katz1/2.png` (income growth by quintile) — from Goldin & Katz, already linked above in the prose but the figures themselves are uncaptioned.
- `lec4_dist_childparent1-3.png` and `lec4_dist_childparent80.png` — from Chetty et al. Science 2017 (already linked in prose).
- `lec4_mobhist1-5.png`, `lec4_mobhist_childparent.png`, `lec4_mobhist_hipot1-3.png` — same source.
- `lec4_berman18_1-4.png` — Berman 2022 (already linked in prose).
- `lec4_deming_1-3.png` — Deming 2017 (already linked).

### 08-mobility-ed (`08-mobility-ed.qmd`, 43 pages — restored deck)

| Slide | Citation | Action |
|---|---|---|
| `## Education and Upward mobility` | "Chetty, Friedman, Saez, Turner, Yagan — Mobility Report Cards" Working Paper 2017 | Linked to [NBER WP 23618](https://www.nber.org/papers/w23618). Also fixed the truncated "Working Paper 201" → "NBER WP 23618 (2017)" |
| `## Estimating the Three Parameters: Data` | "Chetty et al. (2017)" | Same NBER link |

**Figures with no source label:** all of the `lec5_mob_ed/*.png` figures are uncaptioned. They're all from the Chetty/Friedman/Saez/Turner/Yagan 2017 *Mobility Report Cards* paper that's now linked in the deck's reference block at the top. If you want every figure individually labeled, that's a quick batch I can do — but the section header reference covers them all.

**Content note:** the deck has two adjacent slides both titled `## Education and Upward Mobility` (line 55) and `## Education and Upward mobility` (line 69, lowercase "m"). Cosmetic, but worth tidying for the TOC.

### 09-higher-ed (`09-higher-ed.qmd`, 32 pages — restored deck)

| Slide | Citation | Action |
|---|---|---|
| `## Estimating the Causal Effects of Colleges` | "Zimmerman (2014)" | Linked to [Zimmerman, *The Returns to College Admission for Academically Marginal Students*, JOLE 2014](https://www.journals.uchicago.edu/doi/10.1086/676661) |
| `## Regression Discontinuity Methods` | "Zimmerman (2014)" | Same link |
| `## Increasing Applications from High-Achieving, Low-Income Students` | "Hoxby and Avery 2013" | Linked to [Hoxby & Avery, *The Missing One-Offs* (Brookings 2013)](https://www.brookings.edu/wp-content/uploads/2013/03/2013a_hoxby.pdf) |
| `## University of Michigan HAIL Experiment` | "Hoxby and Turner 2013" | Linked to [the SIEPR working paper](https://siepr.stanford.edu/publications/working-paper/expanding-college-opportunities-high-achieving-low-income-students) |
| same | "Dynarski et al. (2018)" | **Linked to Canvas #5** |

**Figures with no source label:** all of the `lec6_higher_ed/zimmerman1-6.png` are uncaptioned but the deck text now identifies the source. Same for `dynarski1-4.png` (HAIL Experiment, now linked in prose) and `parentrank_college.png`, `access_ivy.png`, `income_access.png`, `cost_attending.png`, `earnings_age.png`, `relative_earnings.png` — all from Chetty/Friedman/Saez/Turner/Yagan 2017 or Dynarski et al.

### 10-k12 (`10-k12.qmd`, 46 pages)

| Slide | Citation | Action |
|---|---|---|
| `## K-12 Education: Overview` (References block) | Reference 1: Chetty et al. 2011 STAR | Linked to [QJE 2011](https://academic.oup.com/qje/article/126/4/1593/1923939) |
| same | Reference 2: Reardon et al. 2016 | Linked to [Reardon et al. AJS 2019](https://www.journals.uchicago.edu/doi/10.1086/700678) |
| same | Reference 3: Fredriksson, Ockert, Oosterbeek 2012 | Linked to [QJE 2013](https://academic.oup.com/qje/article/128/1/249/1838780). Note: paper was actually published in QJE 2013, not 2012 |
| same | Reference 4: Chetty, Friedman, Rockoff 2014 | **Linked to Canvas #6** |
| `## Using Test Score Data to Evaluate Primary Education` | "Chetty et al. (2011)" | Same QJE 2011 link |
| `## Studying Differences in Test Score Outcomes` | "Reardon et al. (2016)" | Linked to [Stanford CEPA WP version](https://cepa.stanford.edu/content/geography-racialethnic-test-score-gaps) |
| `## Effects of Class Size: Tennessee STAR Experiment` | "[Krueger 1999, Chetty et al. 2011]" | Krueger linked to [QJE 1999](https://academic.oup.com/qje/article-abstract/114/2/497/1844226), Chetty linked to QJE 2011 |
| `## Effects of Class Size: Quasi-Experimental Evidence` | "Fredriksson et al. (2013)" | Linked to QJE 2013 |

**Figures with no source label:** all `lec7_k12/*.png` figures are uncaptioned. The references block at the top of the deck now covers the four papers they all come from, so the deck's overall provenance is clear.

### 11-teachers-charters (`11-teachers-charters.qmd`, 39 pages)

| Slide | Citation | Action |
|---|---|---|
| `## Using Big Data to Study Teachers' Impacts` | Reference: Chetty, Friedman, Rockoff 2014 | **Linked to Canvas #6** |
| `## Do Charter Schools Work?` | Abdulkadiroǧlu et al. QJE 2011 | Linked to [QJE 2011](https://academic.oup.com/qje/article/126/2/699/1869154) |
| same | Chabrier, Cohodes, Oreopoulos JEP 2016 | Linked to [JEP 2016](https://www.aeaweb.org/articles?id=10.1257/jep.30.3.57) |
| `## Effects of Boston Area Charter Schools` | Abdulkadiroglu et al. (2011) | Same QJE link |
| same (next subsection) | "Angrist et al. (2013)" | Linked to [Angrist, Cohodes, Dynarski, Pathak, Walters, JOLE 2016](https://www.journals.uchicago.edu/doi/10.1086/683822). Note: the actual paper was 2016, not 2013 — the 2013 reference is to the working paper |
| `## Effects of Charter Schools: Summary` | Chabrier et al. (2016) | Same JEP link |
| `## Market Competition and Charter Schools` | Baude, Casey, Hanushek, Rivkin (2014) | Linked to [NBER WP 20645](https://www.nber.org/papers/w20645) |
| `## Limitations of Market Competition` (3rd subsection) | Hastings, Kane, Staiger (2007) | Linked to [NBER WP 12995](https://www.nber.org/papers/w12995) |

**Figures with no source label:** all `lec8_teachers_charters/*.png` are uncaptioned. The `tva*.png` series is from Chetty-Friedman-Rockoff (now linked in the references block). The `abdikaduroglu1.png` figure is from Abdulkadiroglu et al. 2011 (linked). The `baude1/2.png` figures are from Baude et al. 2014 (linked).

### 12-race-ineq (`12-race-ineq.qmd`, 51 pages)

| Slide | Citation | Action |
|---|---|---|
| `# An Intergenerational Perspective on Racial Disparities` | (no top-level citation existed) | **Added a new reference block** linking to [Chetty, Hendren, Jones, Porter — *Race and Economic Opportunity* QJE 2020](https://academic.oup.com/qje/article/135/2/711/5687353) (the paper in `supplementary/`). This is the source for almost every figure in this deck |
| `## The Geography of Upward Mobility in the United States` | "Source: Chetty, Friedman, Hendren, Jones and Porter (2018)" | **Linked to Canvas #1** |
| `## Racial Wealth Gap in the US` | Derenoncourt, Kim, Kuhn, Schularick "Wealth of Two Nations" (2022) | Linked to [QJE 2024 published version](https://academic.oup.com/qje/article/139/2/693/7404432) |

**Figures with no source label:** every figure in `lec9_race_ineq/` is uncaptioned but the top-of-deck reference block now covers them all. They are all from Chetty/Hendren/Jones/Porter QJE 2020 *except* the three `derenoncourt1-3.png` figures, which are from the Derenoncourt et al. paper (linked in the `## Racial Wealth Gap` section).

### 13-criminal-justice (`13-criminal-justice.qmd`, 35 pages)

| Slide | Citation | Action |
|---|---|---|
| `## Racial Discrimination in Hiring` | Bertrand & Mullainathan (2004) | **Linked to Canvas #7** |
| `## Racial Discrimination Among Airbnb Hosts` | Edelman, Luca, Sversky (2017) | Linked to [Edelman, Luca, Svirsky AEJ Applied 2017](https://www.aeaweb.org/articles?id=10.1257/app.20160213) (also fixed "Sversky" → "Svirsky") |
| `## Biases due to Decision Fatigue` | Danziger et al. (2011) | Linked to [PNAS 2011](https://www.pnas.org/doi/10.1073/pnas.1018033108) |
| `## Decisions to Jail vs. Release Defendants` (×2) | Kleinberg et al. (2017) | **Linked to Canvas #8** |
| `## Times Between Burglary Events Separated by 0.1 Miles or Less` | (no source) | **Added** a Mohler et al. JASA 2011 caption + link |

**⚠️ Content fix you flagged — the 3D plot:**
The slide series titled `## Judges' Release Decisions vs. Machine Predictions and Crime Risk` (×5, using `kleinberg2.png` … `kleinberg6.png`) is the 3D rotation of judge decisions you mentioned. The published version of [Kleinberg et al. (QJE 2018)](https://utsa.instructure.com/courses/79928/files/folder/papers?preview=13306220) has this as **Figure II**, a side-by-side dual panel that shows the same information without 3D parallax. **I did not replace the image** because that requires extracting Figure II as a PNG from the published paper PDF — that's a content edit I want you to sign off on first. When you're ready, point me at the page in the PDF and I'll extract the figure into `images/lec10_criminal_justice/kleinberg_fig2.png` and update the slide.

**Figures with no source label otherwise:**
- `tree1.png`, `tree2.png`, `tree3.png` — these are illustrative decision trees, not from any specific paper. Likely Jon's own diagrams. Leave as-is.
- `loss1.png` — same: an illustrative cross-validation loss curve, not from a paper.

### 14-immigration (`14-immigration.qmd`, 37 pages)

| Slide | Citation | Action |
|---|---|---|
| `## Plan for today` | "Slides based on those of David Card (2017)" | Linked to [Card NBER Reporter 2009 essay](https://www.nber.org/reporter/2009number2/how-immigration-affects-us-cities); also added a reference to **Canvas #9** (Clemens 2011) since the deck is broadly based on it |
| `## Long Run Trend in Capital per Unit of Labor` | (had `source="BLS Multifactor Productivity Tables"` already, but in chunk-option syntax, not a real link) | Left as-is — BLS source is correct but not a single URL |
| `## Similar evidence` | "Lee, Peri and Yasenov (2017)" | Linked to [NBER WP 23885](https://www.nber.org/papers/w23885) — the supplementary folder has `peri_yasenov_mariel_boatlift_2017.pdf` which is this paper |
| `## What about mobility of immigrant population?` | "Abramitzky, Boustan, Jacome and Perez (2019)" | Linked to [AER 2021 published version](https://www.aeaweb.org/articles?id=10.1257/aer.20191586). Note: 2019 was the working paper, 2021 is the AER publication |

**Figures with no source label:**
- `wages1.png`, `wages2.png` (background wage stagnation, side-by-side) — likely BLS/Census data; uncaptioned. **Recommend** a "Source: BLS / Census Current Population Survey" caption.
- `immigratgion_stock.png` and `immigratgion_stock_oecd.png` — Pew Research / OECD historical immigration data. Uncaptioned. **Recommend** a Pew Research label. (Also note the typo in the filename: "immigratgion".)
- `table1.png`, `table2.png`, `table3.png` — these are screenshots of tables but no caption or source. They appear to be from Card's NBER Reporter essay but I can't verify without comparing.
- `KL1.png` — labeled as BLS already in the existing chunk option (not a clickable link).
- `KL_synth_israel.png` — Israel synthetic-control example. **No source.** This figure is from Hornung 2014 / Borjas-Doran type studies but I'm not sure which specific paper. **Could not identify confidently — flagged.**
- `city_wage_changes.png` — likely from Card's *Immigration and Inequality* (AER P&P 2009) or similar. Uncaptioned.
- `card17.png` — the filename says "card17" so presumably from a Card 2017 paper, but I can't tell which. **Could not identify confidently — flagged.**
- `peri_yasenov.png`, `peri_yasenov2.png` — clearly from the Peri & Yasenov NBER WP that's now linked in the prose. The figures themselves are uncaptioned.
- `abramitzky1-4.png` — from Abramitzky et al. 2021 (linked in prose).

### 15-political-economy (`15-political-economy.qmd`, 44 pages)

| Slide | Citation | Action |
|---|---|---|
| `## Plan for today` | "Slides based on those of Stantcheca (2019)" | Linked to [Stefanie Stantcheva's Harvard page](https://scholar.harvard.edu/stantcheva). Also fixed the misspelling "Stantcheca" → "Stantcheva" |
| `## How are voter preferences formed?` (Immigration) | "Alesina, Miano and Stantcheva (2020)" | Linked to [Alesina, Miano, Stantcheva, *Immigration and Redistribution*, RES 2023](https://academic.oup.com/restud/article/90/1/1/6586673). Note: the published version is 2023, not 2020 |
| `## How are voter preferences formed?` (Redistribution) | "Alesina, Stantcheva and Teso (2021)" | Linked to [Alesina, Stantcheva, Teso, *Intergenerational Mobility and Preferences for Redistribution*, AER 2018](https://www.aeaweb.org/articles?id=10.1257/aer.20162015). Note: the AER paper is 2018, not 2021 |
| `## Gifts of the Immigrants, Woes of the Natives` | Tabellini (2020) | **Linked to Canvas #9b** |
| `## Are you a Kandinsky or Klee type of person? Tajfel et al (1971)` | Tajfel et al. 1971 | Linked to [classic *European Journal of Social Psychology*](https://onlinelibrary.wiley.com/doi/10.1002/ejsp.2420010202) |
| `## Evidence of In-group Favoritism…` | Chen and Li (2009) | Linked to [AER 2009](https://www.aeaweb.org/articles?id=10.1257/aer.99.1.431) |
| `## Do people know about intergenerational mobility?` | Alesina, Stantcheva and Teso (2020) | Linked to AER 2018 (same as above) |

**Figures with no source label:**
- `immig.png` — Pew survey on immigration attitudes? Uncaptioned. The slide just calls it "Immigration and redistribution" without a citation.
- `beliefs_immigrants.png` … `beliefs_immigrants4.png` — all from Alesina/Miano/Stantcheva 2023 (linked in the deck's prose).
- `wtp_info.png`, `immigration_redist.png` — same source.
- `tabellini1.png`, `tabellini2.png` — from Tabellini 2020 (linked).
- `tajfel1.png` — Tajfel et al. 1971 (linked).
- `chen_li1.png`, `chen_li2.png` — Chen & Li 2009 (linked).
- `stantcheva1.png` … `stantcheva9.png` — all from Alesina/Stantcheva/Teso 2018 (linked).

### 16-taxation1 (`16-taxation1.qmd`, 42 pages)

| Slide | Citation | Action |
|---|---|---|
| `## Federal Tax Revenues, by Type of Tax: 1960 vs 2014` (×3 — federal/state/international) | "Gruber (2016)" — was using `source=` chunk option, which is not a thing in knitr | Replaced with proper `fig.cap="Source: Gruber, *Public Finance and Public Policy* (Worth, 5th ed. 2016)"`. No DOI/link because it's a textbook |
| `## Synthetic Control` | "[Abadie et al. 2010]" | Linked to [Abadie, Diamond, Hainmueller JASA 2010](https://www.tandfonline.com/doi/abs/10.1198/jasa.2009.ap08746) |
| `## .` (empty title slide with the Diamond / Ocasio-Cortez image) | (no citation) | **Added** a reference line: "Based on [Diamond & Saez, *The Case for a Progressive Tax*, JEP 2011](Canvas #10)" |
| `## Measuring Public Preferences for Redistribution` | "Kuziemko et al. (2015)" | Linked to [Kuziemko, Norton, Saez, Stantcheva AER 2015](https://www.aeaweb.org/articles?id=10.1257/aer.20130360) |
| `## Where are you in the income distribution?` (×6 figures using Kuziemko data) | Same — and again were using `source=` chunk option | Replaced with proper `fig.cap` linking to the AER paper |

**Figures with no source label:**
- `mg_av_tax.png` (`## Marginal Income Tax Rates vs. Average Tax Rates: Illustrative Example`) — illustrative figure, no specific source.
- `tax_highest.png` (`## Top Marginal Income Tax Rates in the U.S. Over the Past 100 Years`) — likely Tax Policy Center or IRS historical tables; **uncaptioned**. **Recommend** a "Source: Tax Policy Center" caption.
- `l_supply.png`, `l_supply_types.png` (labor supply theory diagrams) — illustrative, no source needed.
- `laffer_curve.png`, `laffer_curve2.png` — illustrative theory diagrams.
- `kleven_schultz1.png`, `kleven_schultz2.png` — clearly from Kleven & Schultz (AEJ Applied 2014). **Could add a fig.cap link to <https://www.aeaweb.org/articles?id=10.1257/app.6.4.271>**.
- `debacker1.png` (`## Personal Income Tax Revenue, Kansas vs. Surrounding States`) — DeBacker et al. paper on Kansas tax cut. **Could add a link to [DeBacker, Heim, Tran, Yuskavage NBER WP 2018](https://www.nber.org/papers/w24573)** or similar.
- `hayes1.png`, `hayes2.png`, `hayes3.png` (`## Weights Assigned to States by Synthetic Control`) — uncaptioned synthetic Kansas analysis. Could not identify the specific Hayes paper confidently. **Flagged.**
- `diamond_ocasiocortez.png` — now linked in the new reference line above.

### 17-taxation2 (`17-taxation2.qmd`, 52 pages)

| Slide | Citation | Action |
|---|---|---|
| `## Number of Pages of Instructions that Come with Form 1040` | "Gruber (2016)" — was using `source=` chunk option | Replaced with proper `fig.cap` |
| `## Behavioral Public Economics Example 1: Sales Taxes` | Chetty, Looney, Kroft (2009) | Linked to [AER 2009](https://www.aeaweb.org/articles?id=10.1257/aer.99.4.1145) |
| `## Behavioral Public Economics Example 2: Income Taxation` | Chetty, Friedman, and Saez (2013) | Linked to [AER 2013 *Using Differences in Knowledge Across Neighborhoods to Uncover the Impacts of the EITC*](https://www.aeaweb.org/articles?id=10.1257/aer.103.7.2683) |
| `## The Power of Defaults` | Madrian and Shea (2001) | Linked to [QJE 2001](https://academic.oup.com/qje/article/116/4/1149/1903159) |
| `## Crowdout in Retirement Savings Accounts` | "Chetty et al. (2014)" | Linked to [Chetty, Friedman, Leth-Petersen, Nielsen, Olsen QJE 2014 *Active vs. Passive Decisions and Crowd-Out in Retirement Savings*](https://academic.oup.com/qje/article/129/3/1141/1817647) |

**Figures with no source label:**
- `mg_tax.png` (`## Federal Income Tax Rates for a Single Earner with 2 Children in 2006`) — illustrative tax-schedule figure, likely from Gruber's textbook or Tax Policy Center. **Uncaptioned.**
- All `chetty_exp_*.png` (sales-tax experiment) — from Chetty/Looney/Kroft 2009 (now linked in prose).
- All `chetty_eitc1-16.png` — from Chetty/Friedman/Saez 2013 (now linked in prose).
- `madrian1.png`, `madrian2.png` — from Madrian & Shea 2001 (now linked).
- `chetty_pensions1-12.png` — from Chetty et al. 2014 Denmark pensions paper (now linked).

---

## Things I could not find / am uncertain about

1. **`KL_synth_israel.png`** in 14-immigration. The slide says it shows the K/L ratio in Israel after the 1990 Soviet immigration shock but does not name a paper. I suspect Hornung 2014 or Friedberg 2001, but neither is a perfect match. **Need a source from you.**
2. **`card17.png`** in 14-immigration. Filename suggests "Card 2017" but Card has multiple 2017 working papers and I can't identify which one this figure is from without seeing the original. **Need confirmation.**
3. **`hayes1/2/3.png`** in 16-taxation1 (synthetic Kansas). I can't pin down which Hayes paper this is. There are several state-policy synthetic-control studies of Kansas tax cuts but no canonical "Hayes" one I'm aware of. **Need confirmation — possibly a state-policy think-tank report rather than a journal article.**
4. **`debacker1.png`** in 16-taxation1 — likely DeBacker, Heim, Tran, Yuskavage but I didn't confidently link it. **Recommend** verifying and adding the link.
5. **Tables 1, 2, 3** in 14-immigration (`table1/2/3.png`) — screenshots of demographic tables, possibly from Card's NBER Reporter essay or Migration Policy Institute fact sheets. Uncaptioned. **Recommend** identifying and labeling.
6. **`tax_highest.png`** in 16-taxation1 — historical top marginal tax rates. Source is almost certainly the Tax Policy Center historical table or IRS, but no specific citation in the deck. Easy fix once you confirm.
7. **`wages1.png`, `wages2.png`** in 14-immigration — wage stagnation charts, very likely BLS/Census CPS but no caption.

If you can tell me where any of these came from, I'll add them in the next pass.

---

## Papers in `readings/` that are not yet cited in any slide

These are uploaded to Canvas but I didn't find a matching citation in any current deck — either they're for future lectures, or they're a candidate to be cited and I missed where:

| # | Paper | Where I'd expect it to fit |
|---|---|---|
| 4 | Bian, Leslie, Cimpian — *Gender stereotypes about intellectual ability* | Could fit in `12-race-ineq` (gender section) or a future K-12 lecture, but not currently cited |
| 11 | Glaeser et al. — *Big Data and Big Cities* (2018) | Methodology / "big data in social science" section; not currently cited |
| 12 | Isen, Rossin-Slater, Walker — *Every Breath You Take* (Clean Air Act, JPE 2017) | Environmental econ / pollution lecture — not in the current 16 decks |
| 13 | Moore et al. — *Rapidly declining remarkability of temperature anomalies* (PNAS 2019) | Climate-perception lecture — not in the current 16 decks |

The Spring 2026 schedule covers up through `17-taxation2`. There are no environmental-economics decks in `slides/`, which is consistent with the pre-2022 PowerPoint set I saw in `2022-1/slides_ppt/` (which had `lec_15_environmental1.pptx` and `lec_16_environmental2.pptx`). If you want to bring those topics back, the Bian / Glaeser / Isen / Moore papers from your readings folder are ready to go.

---

## Build status

All 16 decks recompile cleanly via:

```bash
PATH="/opt/homebrew/anaconda3/envs/eco3253/bin:$PATH" \
  /Applications/RStudio.app/Contents/Resources/app/quarto/bin/quarto render <deck>.qmd --to beamer
```

Page counts after this pass (essentially unchanged from before, except 12-race-ineq +0 and 06-mto-placebased +0 because the new reference blocks are short):

```
01-intro              18    11-teachers-charters  39
02-intromobility      11    12-race-ineq          51
03-getting-started    60    13-criminal-justice   35
05-causal-effects     31    14-immigration        37
06-mto-placebased     43    15-political-economy  44
07-mob-hist-int       42    16-taxation1          42
08-mobility-ed        43    17-taxation2          52
09-higher-ed          32
10-k12                46
```

Zero pandoc warnings, zero LaTeX overfull/underfull warnings across all builds.

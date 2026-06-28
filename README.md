# To Be Immersed or Not to Be: AI Companions for Dementia Care

A pre-registered, within-subjects study comparing two delivery modalities for an
AI companion, immersive virtual reality (IVR) and desktop, on four outcomes:
social presence, engagement, attitudes toward AI, and usability. This repository
holds the analysis code and the rendered statistical report that accompany the
master's dissertation.

**Pre-registration:** https://osf.io/65k7s

**Rendered report:** https://convai3.github.io/ai-companions-dementia-ivr-desktop/

---

## Data availability

> The participant-level dataset is **not included** in this repository.

The study was conducted with people living with dementia. Because that
population carries heightened privacy and consent-capacity considerations, the
individual records (`kiera_study_data.csv`) are held privately by the research
team and are not published here.

This does not limit what you can read:

- The report is distributed as a **pre-rendered file** and is also hosted via
  GitHub Pages at the link above. All statistics, tables, and figures were
  computed at the time of knitting and are embedded in the output, so the
  complete results are available without the dataset.
- The **analysis code is provided in full**, so every step of the pipeline can
  be inspected. Re-execution from raw data requires access to the private
  dataset.

Requests for access to the underlying data may be directed to the research team
and are subject to the study's ethical approval and data-protection conditions.

## Purpose

This repository accompanies the dissertation for two purposes:

1. **Examination.** It gives examiners and supervisors a single place to review
   the full analysis, the tables and figures, and the rationale behind each
   statistical decision.
2. **Methodological transparency.** Consistent with open-science practice, it
   documents not only the final estimates but the reasoning that produced them.
   For example, the pre-registered test sequence, assumption checks, exclusion
   handling, and sensitivity analyses are all shown; every departure from the
   pre-registered plan is labelled `[Exploratory]` or `[UNPLANNED]`; and a
   convergence check reports the parametric and non-parametric results side by
   side so robustness can be judged directly.

## Repository contents

| File | Description |
|------|-------------|
| `Dataanalysis_AI_Companions_Dementia_IVR_Desktop.Rmd` | The R Markdown source that produces the report. |
| `LICENSE` | Terms of use for the code in this repository. |
| `README.md` | This file. |

The rendered HTML output is hosted via GitHub Pages at
https://convai3.github.io/ai-companions-dementia-ivr-desktop/.

The dataset `kiera_study_data.csv` is intentionally absent (see *Data
availability*).

## Reproducibility

The report is written in R Markdown and built with `rmarkdown::render()`. It
depends on `tidyverse`, `lubridate`, `ez`, `lme4`, `lmerTest`, `effectsize`,
`car`, and `kableExtra`. Analyses follow the pre-registered plan, apply Type III
sums of squares with sum-to-zero contrasts, and report generalised eta-squared
with confidence intervals as the effect-size measure.

## Citation

Please cite the pre-registration when referring to this work:

> Pre-registration, *To Be Immersed or Not to Be: AI Companions for Dementia
> Care*. OSF. https://osf.io/65k7s

## Scope

This repository is the **analysis component** of the dissertation. The full
thesis, including the title page, bilingual abstract, introduction, literature
review, methods and ethics, discussion, conclusion, and APA 7 references, is a
separate document into which these results, tables, and figures are imported.

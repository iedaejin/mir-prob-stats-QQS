# Probability and Statistics (for Policy Analysis)

This repository is for **Probability and Statistics for Policy Analysis**, the Term 1 course in the Master in International Relations (MIR), SPEGA, IE University (SEP-2026 S-2).

It is a session-by-session map from that course’s syllabus to the code and data in [kosukeimai/qss](https://github.com/kosukeimai/qss), the supplementary materials for Imai & Webb Williams, *Quantitative Social Science: An Introduction in tidyverse*. Use the tidyverse files (`*-tidy`). This repository does not copy the textbook or the QSS code; it only points to the sections assigned in class.

**Faculty:** Dae-Jin Lee · daelee@faculty.ie.edu · IE University — Scitech

The full guide is below and in [`QSS-repository-links.md`](QSS-repository-links.md).

---

**Course:** Probability and Statistics for Policy Analysis  
**Programme:** Master in International Relations (MIR), SPEGA · Term 1, SEP-2026 S-2  
**Faculty:** Dae-Jin Lee · daelee@faculty.ie.edu · IE University — Scitech  
**Book:** Imai & Webb Williams, *Quantitative Social Science: An Introduction in tidyverse* (Princeton University Press), as assigned in the syllabus.

Repository: [kosukeimai/qss](https://github.com/kosukeimai/qss).  
The syllabus follows the tidyverse edition. In each chapter folder, the files to use are the ones with `-tidy` in the name (`*.R`, `*.Rmd`, `*.pdf`). The files without `-tidy` are the original 2017 base-R scripts.

Chapter 5 (Discovery) is not assigned. Within the assigned chapters, section 4.2.4 is skipped in session 6 and taken up in session 13, and section 4.4.3 (regression discontinuity) is not assigned.

Errata for the tidyverse edition: [QSS_tidyverse_errata.pdf](https://github.com/kosukeimai/qss/blob/master/errata/QSS_tidyverse_errata.pdf) · [source](https://github.com/kosukeimai/qss/blob/master/errata/QSS_tidyverse_errata.Rmd).

The scripts call `data(..., package = "qss")`. That package lives in a separate repository, [kosukeimai/qss-package](https://github.com/kosukeimai/qss-package). The same files are in the chapter folders below, and each script also shows a `read_csv()` alternative.

Line numbers below point at `causality-tidy.Rmd` and the other chapter R Markdown files on `master`.

## Chapter folders

| QSS | Folder | Tidyverse script | Rendered code |
|---|---|---|---|
| Ch. 1 | [INTRO](https://github.com/kosukeimai/qss/tree/master/INTRO) | [intro-tidy.Rmd](https://github.com/kosukeimai/qss/blob/master/INTRO/intro-tidy.Rmd) · [intro-tidy.R](https://github.com/kosukeimai/qss/blob/master/INTRO/intro-tidy.R) | [intro-tidy.pdf](https://github.com/kosukeimai/qss/blob/master/INTRO/intro-tidy.pdf) |
| Ch. 2 | [CAUSALITY](https://github.com/kosukeimai/qss/tree/master/CAUSALITY) | [causality-tidy.Rmd](https://github.com/kosukeimai/qss/blob/master/CAUSALITY/causality-tidy.Rmd) · [causality-tidy.R](https://github.com/kosukeimai/qss/blob/master/CAUSALITY/causality-tidy.R) | [causality-tidy.pdf](https://github.com/kosukeimai/qss/blob/master/CAUSALITY/causality-tidy.pdf) |
| Ch. 3 | [MEASUREMENT](https://github.com/kosukeimai/qss/tree/master/MEASUREMENT) | [measurement-tidy.Rmd](https://github.com/kosukeimai/qss/blob/master/MEASUREMENT/measurement-tidy.Rmd) · [measurement-tidy.R](https://github.com/kosukeimai/qss/blob/master/MEASUREMENT/measurement-tidy.R) | [measurement-tidy.pdf](https://github.com/kosukeimai/qss/blob/master/MEASUREMENT/measurement-tidy.pdf) |
| Ch. 4 | [PREDICTION](https://github.com/kosukeimai/qss/tree/master/PREDICTION) | [prediction-tidy.Rmd](https://github.com/kosukeimai/qss/blob/master/PREDICTION/prediction-tidy.Rmd) · [prediction-tidy.R](https://github.com/kosukeimai/qss/blob/master/PREDICTION/prediction-tidy.R) | [prediction-tidy.pdf](https://github.com/kosukeimai/qss/blob/master/PREDICTION/prediction-tidy.pdf) |
| Ch. 6 | [PROBABILITY](https://github.com/kosukeimai/qss/tree/master/PROBABILITY) | [probability-tidy.Rmd](https://github.com/kosukeimai/qss/blob/master/PROBABILITY/probability-tidy.Rmd) · [probability-tidy.R](https://github.com/kosukeimai/qss/blob/master/PROBABILITY/probability-tidy.R) | [probability-tidy.pdf](https://github.com/kosukeimai/qss/blob/master/PROBABILITY/probability-tidy.pdf) |
| Ch. 7 | [UNCERTAINTY](https://github.com/kosukeimai/qss/tree/master/UNCERTAINTY) | [uncertainty-tidy.Rmd](https://github.com/kosukeimai/qss/blob/master/UNCERTAINTY/uncertainty-tidy.Rmd) · [uncertainty-tidy.R](https://github.com/kosukeimai/qss/blob/master/UNCERTAINTY/uncertainty-tidy.R) | [uncertainty-tidy.pdf](https://github.com/kosukeimai/qss/blob/master/UNCERTAINTY/uncertainty-tidy.pdf) |

Each folder also holds datasets used only in the chapter exercises. Those are not listed session by session.

## Block 1. From the question to association

### Session 1 — Introduction · QSS Ch. 1

Whole chapter. The script works through R, the tidyverse, and the UN population file.

- Script: [intro-tidy.Rmd](https://github.com/kosukeimai/qss/blob/master/INTRO/intro-tidy.Rmd) · companion [UNpop-tidy.R](https://github.com/kosukeimai/qss/blob/master/INTRO/UNpop-tidy.R)
- Data: [UNpop.csv](https://github.com/kosukeimai/qss/blob/master/INTRO/UNpop.csv) · [UNpop.dta](https://github.com/kosukeimai/qss/blob/master/INTRO/UNpop.dta) · [UNpop.RData](https://github.com/kosukeimai/qss/blob/master/INTRO/UNpop.RData)

### Session 2 — Causation and counterfactuals · QSS 2.1–2.3

Racial discrimination audit study, subsetting, potential outcomes. Section 2.4 is not this session; it is session 16.

- [2.1 Racial discrimination](https://github.com/kosukeimai/qss/blob/master/CAUSALITY/causality-tidy.Rmd#L28-L125)
- [2.2 Subsetting data in R](https://github.com/kosukeimai/qss/blob/master/CAUSALITY/causality-tidy.Rmd#L126-L365)
- [2.3 Causal effects and the counterfactual](https://github.com/kosukeimai/qss/blob/master/CAUSALITY/causality-tidy.Rmd#L366-L373)
- Data: [resume.csv](https://github.com/kosukeimai/qss/blob/master/CAUSALITY/resume.csv)

### Session 3 — Describing a single variable · QSS 2.6 and 3.1–3.5

- [2.6 Descriptive statistics for a single variable](https://github.com/kosukeimai/qss/blob/master/CAUSALITY/causality-tidy.Rmd#L544-L634) — continues the minimum-wage file from 2.5. Read 2.5 itself in session 14.
- [3.1 Civilian victimization](https://github.com/kosukeimai/qss/blob/master/MEASUREMENT/measurement-tidy.Rmd#L28-L103)
- [3.2 Missing data](https://github.com/kosukeimai/qss/blob/master/MEASUREMENT/measurement-tidy.Rmd#L104-L174)
- [3.3 Visualizing a single variable](https://github.com/kosukeimai/qss/blob/master/MEASUREMENT/measurement-tidy.Rmd#L175-L330)
- [3.4 Survey sampling](https://github.com/kosukeimai/qss/blob/master/MEASUREMENT/measurement-tidy.Rmd#L331-L392) — assigned again in session 11
- [3.5 Political polarization](https://github.com/kosukeimai/qss/blob/master/MEASUREMENT/measurement-tidy.Rmd#L393-L394) — the measurement argument; the congressional scatter plots are 3.6, in session 4
- Data: [minwage.csv](https://github.com/kosukeimai/qss/blob/master/CAUSALITY/minwage.csv) · [afghan.csv](https://github.com/kosukeimai/qss/blob/master/MEASUREMENT/afghan.csv)

### Session 4 — Correlation, part 1 · QSS 3.6–3.7

- [3.6 Summarizing bivariate relationships](https://github.com/kosukeimai/qss/blob/master/MEASUREMENT/measurement-tidy.Rmd#L395-L523)
- [3.7 Quantile–quantile plot](https://github.com/kosukeimai/qss/blob/master/MEASUREMENT/measurement-tidy.Rmd#L524-L576)
- Data: [congress.csv](https://github.com/kosukeimai/qss/blob/master/MEASUREMENT/congress.csv) · [USGini.csv](https://github.com/kosukeimai/qss/blob/master/MEASUREMENT/USGini.csv)

The *k*-means section that follows 3.7 in the same file is not assigned.

### Session 5 — Correlation, part 2

No new chapter. Revisit [3.6–3.7](https://github.com/kosukeimai/qss/blob/master/MEASUREMENT/measurement-tidy.Rmd#L395-L576).

### Session 6 — Regression for description and prediction, part 1 · QSS 4.1 and 4.2, skip 4.2.4

- [4.1 Predicting election outcomes](https://github.com/kosukeimai/qss/blob/master/PREDICTION/prediction-tidy.Rmd#L30-L374)
- [4.2.1–4.2.3 Facial appearance, correlation, least squares](https://github.com/kosukeimai/qss/blob/master/PREDICTION/prediction-tidy.Rmd#L375-L469)
- [4.2.5 Merging data sets](https://github.com/kosukeimai/qss/blob/master/PREDICTION/prediction-tidy.Rmd#L472-L518) — the join only. The Obama 2008–2012 regression that follows is 4.2.4.
- Data: [polls08.csv](https://github.com/kosukeimai/qss/blob/master/PREDICTION/polls08.csv) · [pollsUS08.csv](https://github.com/kosukeimai/qss/blob/master/PREDICTION/pollsUS08.csv) · [pres08.csv](https://github.com/kosukeimai/qss/blob/master/PREDICTION/pres08.csv) · [pres12.csv](https://github.com/kosukeimai/qss/blob/master/PREDICTION/pres12.csv) · [face.csv](https://github.com/kosukeimai/qss/blob/master/PREDICTION/face.csv)

Leave [4.2.4](https://github.com/kosukeimai/qss/blob/master/PREDICTION/prediction-tidy.Rmd#L470-L554) for session 13. In the R Markdown file the 4.2.4 heading has no code of its own; the demonstration is the standardized 2008–2012 regression at lines 521–554, after the merge that builds the data.

### Session 7 — Regression for description and prediction, part 2 · QSS 4.2.6

- [4.2.6 Model fit](https://github.com/kosukeimai/qss/blob/master/PREDICTION/prediction-tidy.Rmd#L556-L670)
- Data: [florida.csv](https://github.com/kosukeimai/qss/blob/master/PREDICTION/florida.csv)

### Session 8 — Midterm exam 1

No new reading. Covers sessions 1–7.

## Block 2. Uncertainty and inference

### Session 9 — Probability, part 1 · QSS 6.1–6.2

- [6.1 Probability](https://github.com/kosukeimai/qss/blob/master/PROBABILITY/probability-tidy.Rmd#L28-L110)
- [6.2 Conditional probability](https://github.com/kosukeimai/qss/blob/master/PROBABILITY/probability-tidy.Rmd#L111-L588), including Bayes’ rule and surname prediction
- Data: [FLVoters.csv](https://github.com/kosukeimai/qss/blob/master/PROBABILITY/FLVoters.csv) · [names.csv](https://github.com/kosukeimai/qss/blob/master/PROBABILITY/names.csv) · [FLCensusVTD.csv](https://github.com/kosukeimai/qss/blob/master/PROBABILITY/FLCensusVTD.csv)

### Session 10 — Probability, part 2 · QSS 6.3–6.4

- [6.3 Random variables and probability distributions](https://github.com/kosukeimai/qss/blob/master/PROBABILITY/probability-tidy.Rmd#L589-L793)
- [6.4 Law of large numbers and the central limit theorem](https://github.com/kosukeimai/qss/blob/master/PROBABILITY/probability-tidy.Rmd#L794-L928)
- Data: [pres08.csv](https://github.com/kosukeimai/qss/blob/master/PROBABILITY/pres08.csv). The standardized presidential file `pres.csv` is written by the Chapter 4 script (`write_csv` near the 4.2.4 example); it is not stored in the repository.

### Session 11 — Estimation and uncertainty · QSS 3.4 and 7.1

- [3.4 Survey sampling](https://github.com/kosukeimai/qss/blob/master/MEASUREMENT/measurement-tidy.Rmd#L331-L392), first assigned in session 3
- [7.1 Estimation](https://github.com/kosukeimai/qss/blob/master/UNCERTAINTY/uncertainty-tidy.Rmd#L28-L464): unbiasedness, standard error, confidence intervals, polls, and the STAR experiment
- Data: [afghan.csv](https://github.com/kosukeimai/qss/blob/master/MEASUREMENT/afghan.csv) · [pres08.csv](https://github.com/kosukeimai/qss/blob/master/UNCERTAINTY/pres08.csv) · [polls08.csv](https://github.com/kosukeimai/qss/blob/master/UNCERTAINTY/polls08.csv) · [STAR.csv](https://github.com/kosukeimai/qss/blob/master/UNCERTAINTY/STAR.csv)

### Session 12 — Hypothesis testing · QSS 7.2 and 7.3.4

- [7.2 Hypothesis testing](https://github.com/kosukeimai/qss/blob/master/UNCERTAINTY/uncertainty-tidy.Rmd#L465-L716)
- [7.3.4 Inference about coefficients](https://github.com/kosukeimai/qss/blob/master/UNCERTAINTY/uncertainty-tidy.Rmd#L775-L797). Sections 7.3.1–7.3.3 are the setup for that output; 7.3.5 (inference about predictions) is not the assigned section.
- Data: [resume.csv](https://github.com/kosukeimai/qss/blob/master/UNCERTAINTY/resume.csv) · [women.csv](https://github.com/kosukeimai/qss/blob/master/UNCERTAINTY/women.csv) · [minwage.csv](https://github.com/kosukeimai/qss/blob/master/UNCERTAINTY/minwage.csv)

### Session 13 — Reversion to the mean · QSS 4.2.4

- Heading: [4.2.4 Regression towards the mean](https://github.com/kosukeimai/qss/blob/master/PREDICTION/prediction-tidy.Rmd#L470-L471)
- The worked example, after the merge from 4.2.5: [Obama 2008–2012](https://github.com/kosukeimai/qss/blob/master/PREDICTION/prediction-tidy.Rmd#L521-L554)
- Data: [pres08.csv](https://github.com/kosukeimai/qss/blob/master/PREDICTION/pres08.csv) · [pres12.csv](https://github.com/kosukeimai/qss/blob/master/PREDICTION/pres12.csv)

### Session 14 — Why correlation does not imply causation · QSS 2.5 and 4.3

- [2.5 Observational studies](https://github.com/kosukeimai/qss/blob/master/CAUSALITY/causality-tidy.Rmd#L425-L543): minimum wage, confounding, before-and-after, difference-in-differences
- [4.3 Regression and causation](https://github.com/kosukeimai/qss/blob/master/PREDICTION/prediction-tidy.Rmd#L671-L672) — the argument in the script is this short section. The women-reservation regressions that follow open section 4.4, assigned in sessions 18 and 20.
- Data: [minwage.csv](https://github.com/kosukeimai/qss/blob/master/CAUSALITY/minwage.csv)

### Session 15 — Midterm exam 2

No new reading. Covers sessions 9–14.

## Block 3. From association to cause

### Session 16 — Randomized experiments, part 1 · QSS 2.4

Taught here, not in session 2.

- [2.4 Randomized controlled trials](https://github.com/kosukeimai/qss/blob/master/CAUSALITY/causality-tidy.Rmd#L374-L424), the social-pressure turnout experiment
- Data: [social.csv](https://github.com/kosukeimai/qss/blob/master/CAUSALITY/social.csv)

### Session 17 — Randomized experiments, part 2

No new chapter. Revisit [2.4](https://github.com/kosukeimai/qss/blob/master/CAUSALITY/causality-tidy.Rmd#L374-L424).

### Session 18 — Controlling for confounders, part 1 · QSS 4.4.1

- Setup for the section, the women-reservation experiment: [4.4 opening](https://github.com/kosukeimai/qss/blob/master/PREDICTION/prediction-tidy.Rmd#L673-L698)
- [4.4.1 Regression with multiple predictors](https://github.com/kosukeimai/qss/blob/master/PREDICTION/prediction-tidy.Rmd#L699-L765)
- Data: [women.csv](https://github.com/kosukeimai/qss/blob/master/PREDICTION/women.csv) · [social.csv](https://github.com/kosukeimai/qss/blob/master/PREDICTION/social.csv)

Section 4.4.3, regression discontinuity, starts at [line 879](https://github.com/kosukeimai/qss/blob/master/PREDICTION/prediction-tidy.Rmd#L879) and is not assigned. Its data file is [MPs.csv](https://github.com/kosukeimai/qss/blob/master/PREDICTION/MPs.csv).

### Session 19 — Controlling for confounders, part 2

No new chapter. Revisit [4.4.1](https://github.com/kosukeimai/qss/blob/master/PREDICTION/prediction-tidy.Rmd#L699-L765), including which controls help and which do not.

### Session 20 — Mechanisms · QSS 4.4.2

- [4.4.2 Heterogeneous treatment effects](https://github.com/kosukeimai/qss/blob/master/PREDICTION/prediction-tidy.Rmd#L766-L878)
- Data: [social.csv](https://github.com/kosukeimai/qss/blob/master/PREDICTION/social.csv) (loaded in 4.4.1)

### Sessions 21–22 — Final exam

No new reading. Cumulative, with emphasis on sessions 16–20.

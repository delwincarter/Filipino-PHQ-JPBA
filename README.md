# Psychometric Evaluation of the PHQ-8 Among Filipino American Emerging Adults  
## Reproducible Workflow Supplement

This repository contains the executable Quarto workflow and computational materials associated with the manuscript:

**Psychometric Evaluation of the 8-Item Patient Health Questionnaire Among Filipino American Emerging Adult Men and Women**

The supplement provides a reproducible analytic pipeline for:

- data preparation and subgroup definition
- item-level descriptive statistics
- confirmatory factor analyses of one-factor and two-factor models
- multigroup measurement invariance testing
- correlations between PHQ-8 scores and theoretically related constructs
- bootstrap confidence intervals for correlational validity estimates
- reproduction of the manuscript’s computational results, tables, and figures

All confirmatory factor analysis and measurement invariance models are estimated in **R** using **lavaan**, with **WLSMV estimation**, polychoric correlations for ordinal indicators, and the **THETA parameterization**.

---

## Supplement materials

### Interactive HTML workflow

The interactive HTML version is recommended for reviewing the complete code, outputs, tables, and section-level navigation:

https://delwincarter.github.io/Filipino-PHQ-JPBA/

The GitHub Pages site is generated from:

`index.html`

### Journal-formatted PDF

[Download the PDF supplement](PHQ-8-Filipino-American.pdf)

Repository filename:

`PHQ-8-Filipino-American.pdf`

### Executable Quarto source

`PHQ-8 Filipino American.qmd`

The Quarto source contains the complete analytic workflow used to generate both the HTML and PDF supplements.

All numerical values reported in the manuscript tables—including fit indices, standardized factor loadings, factor correlations, reliability estimates, measurement invariance statistics, and validity correlations—are regenerated directly from this workflow. Tables in the repository function as computational verification tables; the published manuscript presents the same results in journal-typeset form.

---

## Repository structure

```text
Filipino-PHQ-JPBA/
├── README.md
├── index.html                              # Interactive HTML workflow
├── PHQ-8-Filipino-American.pdf             # Journal-formatted PDF supplement
├── PHQ-8 Filipino American.qmd             # Executable Quarto source
├── tables/                                 # Tables generated from gt
├── figures/                                # CFA diagrams and other figures
├── data/
│   ├── phq_final_manuscript.sav            # De-identified analytic dataset
└── Filipino PHQ JPBA.Rproj                 # RStudio project file
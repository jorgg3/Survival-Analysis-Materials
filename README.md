
# Applied Survival Analysis: Course Materials & R Tutorials

This repository contains a comprehensive collection of **RMarkdown** tutorials, laboratory sessions, and theoretical notes developed during my tenure as a **Teaching Assistant** for the  **Survival Analysis** courses at the **Faculty of Sciences, UNAM** (National Autonomous University of Mexico).

The goal of these materials is to bridge the gap between abstract statistical theory and practical implementation in **R**, specifically for students and researchers in Actuarial Science and Data Science.

---

##  Repository Structure

The content follows the logical progression of a specialized survival analysis syllabus:

### 1. Foundations & Non-Parametric Methods
* **`01-Intro-OLS-vs-Survival`**: A demonstration of why Ordinary Least Squares regression fails with censored data and the fundamental logic of survival models.
* **`02-Non-Parametric-Methods`**: Step-by-step manual construction of the **Kaplan-Meier** estimator using `dplyr` and comparison of survival curves via Log-rank and Wilcoxon tests.
* **`03-AIDS-Case-Study`**: A complete non-parametric analysis using the classic `Aids2` dataset to evaluate survival differences by age and transmission category.

### 2. Parametric Modeling (AFT Framework)
* **`04-Parametric-Models`**: Fitting **Exponential**, **Weibull**, and **Log-Normal** distributions and mapping `survreg` outputs to theoretical parameters.
* **`05-Model-Diagnostics`**: Graphical linearization techniques (Log-Log plots) and formal **Likelihood Ratio Tests (LRT)** for model selection.

### 3. Semi-Parametric Models & Extensions
* **`06-Cox-Proportional-Hazards`**: Multivariable modeling using the UIS dataset, interpretation of Hazard Ratios, and verification of the proportionality assumption.
* **`07-Variable-Selection`**: Advanced strategies for model refinement using **AIC** and diagnostics for non-linearity (quadratic terms vs. factors).
* **`08-GLM-Workshop`**: A foundational review of Logistic and Poisson regression, including overdispersion diagnostics.

---

## Requirements

To replicate these analyses, you will need **R** and the following specialized libraries:

* `survival`: Core survival analysis functions.
* `survminer`: Advanced visualization (ggplot2-based).
* `ggplot2` & `dplyr`: Data manipulation and custom plotting.
* `MASS` & `collett`: Academic datasets for practical examples.

```r
# Installation command
install.packages(c("survival", "survminer", "ggplot2", "dplyr", "MASS", "collett"))

---
Author: José Jorge Martínez de la Cruz

Teaching Assistant, Facultad de Ciencias, UNAM

Data Science Candidate | Survival Analysis Enthusiast
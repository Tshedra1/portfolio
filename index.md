# 🧠 Tamara Harness

### Public Health | Epidemiology | Data Analysis

---

# 📊 Project: Predictors of Respiratory Muscle Strength in Cystic Fibrosis

## 📌 Overview

This project examines clinical and physiological predictors of respiratory muscle strength using a cystic fibrosis dataset. The outcome of interest is maximum expiratory pressure (PEmax), a key indicator of respiratory muscle function.

---

## 🎯 Research Question

What factors are associated with respiratory muscle strength (PEmax) in individuals with cystic fibrosis?

---

## 🧪 Methods

* Study design: Cross-sectional analysis
* Model: Multivariable linear regression

### Variables:

* Outcome: **PEmax**
* Predictors:

  * Age
  * Sex
  * Body Mass Percentile (BMP)
  * FEV1 (lung function)
  * Residual Volume (RV)

### Model Decisions:

* Removed height due to multicollinearity (VIF > 7)
* Final model confirmed with VIF < 5
* Diagnostic plots confirmed assumptions

---

## 📊 Results

| Variable             | Estimate | 95% CI       | p-value   |
| -------------------- | -------- | ------------ | --------- |
| Age                  | 4.64     | (2.01, 7.XX) | 0.0XX     |
| Sex                  | 0.78     | (-25.4, XX)  | 0.93      |
| Body Mass Percentile | -0.36    | (-1.54, XX)  | 0.46      |
| FEV1                 | **1.71** | (0.12, XX)   | **0.037** |
| Residual Volume (RV) | 0.15     | (-0.06, XX)  | 0.14      |

---

## 🧠 Interpretation

FEV1 was a significant predictor of respiratory muscle strength, indicating that better lung function is associated with higher PEmax. Age was also positively associated with PEmax. Other variables were not statistically significant.

---

## 📈 Model Diagnostics

* No major violations of linearity
* Residuals approximately normal
* No influential outliers
* No multicollinearity (VIF < 5)

---

## 🛠️ Tools Used

* R (lm, broom, dplyr)
* car (VIF diagnostics)

---

## 💻 Code

👉 [View full analysis on GitHub]https://github.com/Tshedra1/nhanes-obesity-hypertension

---

## 👩‍⚕️ About Me

Public health professional with training in epidemiology and applied biostatistics. Experienced in R, Stata, and data-driven health research.

---

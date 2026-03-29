# NHANES / Cystic Fibrosis Analysis: Obesity, Lung Function, and Respiratory Strength

## 📌 Overview

This project examines the relationship between pulmonary function, body composition, and respiratory muscle strength using a cystic fibrosis dataset. The primary objective is to identify predictors of maximum expiratory pressure (PEmax), a key measure of respiratory muscle function.

---

## 🎯 Research Question

What clinical and physiological factors are associated with respiratory muscle strength (PEmax) in individuals with cystic fibrosis?

---

## 📊 Methods

* Multivariable linear regression was used
* Outcome: **PEmax (maximum expiratory pressure)**
* Predictors:

  * Age
  * Sex
  * Body Mass Percentile (BMP)
  * FEV1 (lung function)
  * Residual Volume (RV)

### Model Selection

* High collinearity identified between height and age (VIF > 7)
* Height removed to improve model stability
* Final model selected based on interpretability and diagnostics

### Diagnostics Performed

* Residual vs fitted plots
* Q-Q plots
* Scale-location plots
* Residuals vs leverage
* Variance Inflation Factors (VIF)

---

### Results

In the final multivariable linear regression model, both FEV1 and age were significantly positively associated with maximum expiratory pressure (PEmax). Specifically, higher FEV1 was associated with increased PEmax, indicating that better pulmonary function is linked to greater respiratory muscle strength. Age was also positively associated with PEmax, suggesting increased respiratory muscle strength with increasing age in this sample.

Residual volume (RV) showed a positive but non-significant association with PEmax. Body mass percentile (BMP) and sex were not significantly associated with PEmax.

Confidence intervals supported these findings, with statistically significant predictors demonstrating intervals that did not cross zero. Overall, the model demonstrated acceptable fit and stability, with no evidence of multicollinearity.

---

## 🧠 Interpretation

These results suggest that pulmonary function plays a central role in respiratory muscle strength in cystic fibrosis. The findings support the clinical importance of maintaining lung function to preserve respiratory mechanics.

---

## 🛠️ Tools Used

* R (base, stats)
* `broom`, `dplyr`
* `car` (VIF diagnostics)

---

## 📂 Output

* Regression results table (CSV)
* Diagnostic plots
* Reproducible R code

---

## 🚀 Next Steps

* Apply survey-weighted models (NHANES extension)
* Explore interaction effects (e.g., sex × lung function)
* Expand to longitudinal analysis

---

## 👩‍⚕️ Author

Tamara Harness
Public Health | Epidemiology | Data Analysis

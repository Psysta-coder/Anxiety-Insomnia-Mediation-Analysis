# Anxiety, Insomnia, and Rumination: A Mediation Analysis

This repository contains a Python Jupyter notebook that performs a mediation analysis to examine whether **rumination** mediates the relationship between **anxiety** and **insomnia**.

---

## 📊 Key Findings

- **Anxiety has a significant direct effect on insomnia** (β = 0.396, p < 0.001).
- **Rumination does NOT significantly mediate** this relationship:
  - Indirect effect = 0.028
  - 95% Bootstrap CI = [-0.001, 0.064] → contains zero
  - Sobel test: Z = 1.72, p = 0.086
- The direct effect remains strong after controlling for rumination (β = 0.396, p < 0.001).

> ⚠️ **The mediation hypothesis is rejected.** Rumination is not a significant mediator between anxiety and insomnia.

---

## 📁 Files

- `khab.ipynb` – Jupyter notebook with the full analysis (data cleaning, scoring, descriptive statistics, Pearson correlations, mediation analysis with Baron & Kenny + Sobel test + Bootstrap)

---

## 🛠️ Tools Used

- Python 3
- pandas, numpy – data manipulation
- statsmodels – OLS regression
- scipy – correlations & Sobel test
- Jupyter Notebook

---

## 🚀 How to Run

1. Clone this repository:
```bash
git clone https://github.com/Psysta-coder/Anxiety-Insomnia-Mediation-Analysis.git

bash

pip install pandas numpy statsmodels scipy openpyxl jupyter

bash

jupyter notebook khab.ipynb

Results Summary
Path                                          | Coefficient | p-value
----------------------------------------------|-------------|---------
a (Anxiety → Rumination)                      | 0.266       | < 0.001
b (Rumination → Insomnia | Anxiety)           | 0.104       | 0.052
c (Total: Anxiety → Insomnia)                 | 0.424       | < 0.001
c' (Direct: Anxiety → Insomnia | Rumination)  | 0.396       | < 0.001
Indirect effect (a × b)                       | 0.028       | Sobel p = 0.086
Bootstrap 95% CI for indirect                 | [-0.001, 0.064] | Not significant

📝 Notes

Data is anonymized. Raw survey responses are not shared to protect participant privacy.

Cronbach's alpha: ISI = 0.66, GAD-7 = 0.88, Rumination = 0.71.

The ISI reliability is slightly below the conventional 0.70 threshold — this is acknowledged as a limitation.

All analyses are reproducible using the provided notebook.




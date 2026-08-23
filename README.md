# Anxiety, Insomnia, and Rumination: A Mediation Analysis

This repository contains a Python Jupyter notebook that performs a mediation analysis to examine whether **rumination** mediates the relationship between **anxiety** and **insomnia**.

---

## 📊 Key Findings
- Anxiety has a **significant direct effect** on insomnia (β = 0.187, p < 0.001).
- Rumination **does NOT significantly mediate** this relationship:
  - Indirect effect = -0.017
  - 95% Bootstrap CI = [-0.042, 0.002]
- The direct effect remains significant after controlling for rumination (β = 0.205, p < 0.001).

> ⚠️ The mediation hypothesis is **rejected**. Rumination is not a significant mediator.

---

## 📁 Files
- `mediation_analysis_anxiety_insomnia.ipynb` – Jupyter notebook with all analyses (data cleaning, coding, regression, Sobel test, bootstrapping, tables)

---

## 🛠️ Tools Used
- Python 3
- pandas, numpy, statsmodels, scipy, pingouin, matplotlib

---

## 🚀 How to Run

1. Clone this repository:
```bash
git clone https://github.com/Psysta-coder/Anxiety-Insomnia-Mediation-Analysis.git
    Install the required libraries:

bash

pip install pandas numpy statsmodels scipy pingouin matplotlib openpyxl
    Open the notebook and run all cells:

bash

jupyter notebook mediation_analysis_anxiety_insomnia.ipynb
Results Summary
Path	Coefficient	p-value
Anxiety → Rumination (a)	0.176	< 0.001
Rumination → Insomnia (b)	-0.097	0.042
Total effect (c)	0.187	< 0.001
Direct effect (c')	0.205	< 0.001
Indirect effect (Sobel)	-0.017	0.079
Indirect effect (Bootstrap CI)	-0.017	[-0.042, 0.002]
📝 Notes

    Data is anonymized.

    All analyses are reproducible.

# Data-Science-Analyst-Portfolio

Hi, I'm Rifdah Salsabila! You can call me Rifdah. I'm a fresh mathemathics graduate from University of Indonesia. Currently I have serious interest in Data Analytics and Data Science. I'm also looking for any internship or entry level jobs related to data analytics/data science. This repository showcases my data science and machine learning projects, tracking my progress and skills in the field.

My CV in Bahasa Indonesia: [Click here](https://github.com/rifdahsalsabila-git/Data-Science-Analyst-Portfolio/blob/main/CV_Rifdah%20Salsabila.pdf)

## Table of Contents

- [Portfolio Projects](#portfolio-projects)
  - Python
    - [Mpox Classification](#mpox-classification)
- [Education](#education)
- [Contact](#contact)

## Portfolio Projects

In this section I list my data science / machine learning projects, briefly describing the problem, approach, and results.

### Mpox Classification

**Code:** [`Mpox_Classification.ipynb`](https://github.com/rifdahsalsabila-n109zone/Mpox-Classification)

**Goal:** To classify patient into positive or negative Mpox based on clinical features and and laboratory data.

**Skills:** data cleaning, exploratory data analysis, feature selection, ensemble modeling, model evaluation.

**Library:** Python, Pandas, NumPy, Scikit-learn, Seaborn, Matplotlib, Graphviz.

**Description:** The dataset contains 500 patient records with 50 raw features covering demographics, clinical symptoms, and lab test results. The project involved data cleaning, exploratory data analysis, manual feature selection (keeping necessary features based on papers), and training a Bagging ensemble model with 50 Decision Trees, validated across 3 random seeds (0, 1, 42) for robustness.

**Results:** The model achieved an average test accuracy of 98.3% and recall of 99.4% across 3 random seeds. Platelet count emerged as the dominant predictive feature (67% importance), followed by ALT level and sore throat symptoms. Notable finding: although training accuracy reached 100%, the test accuracy doesn't fall off way too far from train accuracy. Meaning that the model doesn't ovefit/underfit. The high accuracy might've been due to the combinations of features in the decision tree that could identify a positive/negative patient.

## Education

`University of Indonesia`:
`Mathemathics`
`(2021-2026)`


## Contact

- LinkedIn: `linkedin.com/in/rifdah-salsabila732998218`
- Email: `rifdahdjamaan@gmail.com`
- Phone: `+62-812-1244-1448`

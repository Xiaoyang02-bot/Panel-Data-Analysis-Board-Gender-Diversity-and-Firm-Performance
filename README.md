# Panel Data Analysis: Board Gender Diversity and Firm Performance (Stata to Python)

**Author:** Xiaoyang Ma  
**GitHub Profile:** https://github.com/Xiaoyang02-bot

## Academic Integrity and Project Context

This project is a **personal Python implementation** of an econometric analysis assignment for the "Applied Econometrics I (ECON2005)" module at the University of Nottingham.

* **Original Assignment:** The original coursework was a **group project** completed using **Stata**, as per the module requirements.
* **Personal Contribution:** All Python code, analysis, and visualizations in the `.ipynb` notebook are my **sole, original work**. This was an independent, self-directed project undertaken *in addition* to the group assignment to demonstrate my proficiency in the Python data science ecosystem.
* **Disclaimer:** To maintain strict academic integrity, the original university course requirements, official assignment brief, the original group's Stata report, and the private dataset are **not** included in this repository.

## Project Goal

This analysis investigates the question: "Do female directors improve the financial performance of companies?".

The workflow involves a rigorous, multi-stage regression analysis:
1.  **Data Preparation:** Loading data and engineering key features (e.g., `pfdir`, `lnsize`).
2.  **Baseline Modeling:** Building OLS models with two different performance metrics (Return on Assets and Tobin's Q).
3.  **Diagnostics & Robustness:** Conducting White's tests for heteroscedasticity and re-estimating all models with robust (HC3) standard errors.
4.  **Advanced Modeling (Non-Linearity):** Testing for complex, non-linear (quadratic) relationships using F-tests.
5.  **Advanced Modeling (Interaction Effects):** Investigating moderation by testing if the diversity-performance relationship varies by company size.
6.  **Advanced Visualization:** Replicating Stata's `marginsplot` functionality to plot predicted outcomes for clear interpretation.

## Skills & Tools Used

* **Python 3**
* **Pandas:** For data loading, manipulation, and feature engineering.
* **Statsmodels:** For OLS regression, robust standard error (HC3) estimation, and F-tests.
* **Matplotlib & Seaborn:** For all data visualization, especially plotting predicted marginal effects.
* **Jupyter Notebook:** As the environment for analysis and presentation.

## Data Source and Availability

* The analysis methodology is based on the `GenderDirectorsData2.dta` dataset, a panel dataset of UK-registered companies (2008-2016) provided by the university for the ECON2005 module.
* **Note on Data Availability:** This dataset was proprietary to the module. To respect academic policy and data licensing, the raw `.dta` file is **not included** in this public repository. The Jupyter notebook is provided to showcase the complete analytical method.

## How to Run This Project

1.  Ensure you have Anaconda or Python installed with the libraries listed above.
2.  Clone or download this repository.
3.  Open the `.ipynb` notebook in Jupyter Lab or Jupyter Notebook.
4.  **Note:** As the data file (`GenderDirectorsData2.dta`) is not provided, the notebook cannot be run from top to bottom. However, all code cells are complete and serve as a demonstration of the full analytical workflow.

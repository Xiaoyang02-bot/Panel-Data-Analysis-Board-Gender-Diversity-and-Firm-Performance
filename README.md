# Panel Data Analysis: Board Gender Diversity and Firm Performance

**Author:** Xiaoyang Ma  
**GitHub Profile:** https://github.com/Xiaoyang02-bot

---

### Academic Integrity and Project Context

This project is a personal Python implementation of an econometric analysis assignment for the "Applied Econometrics I (ECON2005)" module
The original assignment was completed using Stata. The purpose of this repository is to:

* **Demonstrate Technical Proficiency:** Showcase my ability to independently replicate a complex econometric workflow using the Python (Pandas, Statsmodels, Matplotlib) ecosystem.
* **Create a Portfolio Piece:** Translate academic coursework into a practical, well-documented data science project.

All Python code in the `.ipynb` notebook is my original work.

---

### Project Goal

This analysis investigates the question: "Do female directors improve the financial performance of companies?".

The workflow involves a rigorous, multi-stage regression analysis:

1.  **Data Preparation:** Loading data and engineering key features, such as the share of female directors (`pfdir`) and log-transformed company size (`lnsize`)
2.  **Baseline Modeling:** Building OLS models with two different performance metrics (Return on Assets and Tobin's Q) and multiple control variables.
3.  **Diagnostics & Robustness:** Conducting White's tests for heteroscedasticity and re-estimating all models with robust (HC3) standard errors to ensure valid inference.
4.  **Advanced Modeling (Non-Linearity):** Extending the models to test for complex, non-linear (quadratic) relationships, using F-tests for joint significance.
5.  **Advanced Modeling (Interaction Effects):** Investigating moderation by testing if the relationship between diversity and performance *varies depending on company size*.
6.  **Advanced Visualization:** Replicating Stata's `marginsplot` functionality to generate and plot predicted outcomes, allowing for clear interpretation of the complex non-linear and interaction models.

---

### Skills & Tools Used

* **Python 3**
* **Pandas:** For data loading (from `.dta`), manipulation, and feature engineering.
* **Statsmodels:** For OLS regression, robust standard error (HC3) estimation, and F-tests.
* **Matplotlib & Seaborn:** For all data visualization, especially for plotting predicted marginal effects from the regression models.
* **Jupyter Notebook:** As the environment for analysis and presentation.

---

### Data Source

The analysis uses the `GenderDirectorsData2.dta` dataset, a panel dataset of UK-registered companies covering the period 2008-2016.

**Note on Data Availability:** This dataset was provided by the university exclusively for the ECON2005 module. Due to unconfirmed data licensing and to respect academic policy, the raw `.dta` file is **not included** in this public repository. The Jupyter notebook is provided to showcase the complete analytical method.

---

### How to Run This Project

1.  Ensure you have Anaconda or Python installed with the libraries listed above (pandas, statsmodels, matplotlib, seaborn).
2.  Clone or download this repository.
3.  Open the `.ipynb` notebook in Jupyter Lab or Jupyter Notebook.
4.  **Note:** As the data file (`GenderDirectorsData2.dta`) is not provided, the notebook cannot be run from top to bottom. However, the code is complete and serves as a demonstration of the full analytical workflow.

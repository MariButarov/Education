# Educational Inequality in U.S. High Schools: The Influence of Socioeconomic and Geographic Factors

Analyzing the relationship between socioeconomic factors and ACT scores across 7,227 U.S. high schools using statistical analysis and linear regression to explore educational inequality and differences between states.

---

## Project Overview

This project explores educational inequality in U.S. high schools by examining how socioeconomic factors relate to average ACT scores. Using data from 7,227 schools across 20 states, the analysis investigates the relationships between ACT performance, household income, unemployment, education levels, and free or reduced-price lunch eligibility. Multiple linear regression showed that socioeconomic characteristics were significantly associated with ACT scores. Adding state information improved the model's R² from 0.628 to 0.679, suggesting that geographic differences also play an important role.

- **Objective:** Investigate how socioeconomic characteristics are associated with ACT scores and compare academic performance across states.
- **Domain:** Education / Social Inequality
- **Key Techniques:** Exploratory Data Analysis (EDA), Data Cleaning, Missing Value Imputation, Multiple Linear Regression, Feature Scaling, and ANOVA.

---

## Project Structure

```
├── data/                 # Raw and processed data
├── code/                 # Jupyter notebooks and Python scripts
├── reports/              # Generated reports and visualizations
├── requirements.txt      # Dependencies
└── README.md             # Project documentation
```

---

## Data

- **Source:** EdGap Dataset: edgap.org/#5/37.579/-95.998
- National Center for Education Statistics (NCES): https://nces.ed.gov/ccd/pubschuniv.asp 
- **Description:** Brief overview of the dataset features, size, and format
- **License:** 

---

## Analysis

The analysis was conducted in **`Education.ipynb`**, a Jupyter Notebook containing the complete workflow, from data preparation to statistical modeling.

To reproduce the results, run the notebook cells in order, starting with importing the required Python libraries and loading the EdGap and NCES datasets. The notebook then explores the original data, selects relevant variables, merges the datasets, handles missing values, and exports the cleaned dataset as `education_clean.csv`.

The next sections load the cleaned data, perform exploratory data analysis, and build simple and multiple linear regression models. These are followed by state comparisons, model evaluation using R² and MAE, ANOVA tests, and standardization of selected predictors.

**Note:** The original file paths in the notebook must be updated to match the location of the datasets on your computer before running the code.

---
## Analysis File

The data cleaning and analysis are performed in:

Education.ipynb

---

## Clean Data File

The cleaned dataset used for the analysis is:

education_clean.csv

## Results

The analysis found that socioeconomic characteristics are significantly associated with average ACT scores in U.S. high schools. Free or reduced-price lunch eligibility showed a strong negative relationship with ACT scores, while higher levels of college education were associated with better performance. Unemployment also showed a negative association, although its relationship was weaker.

The multiple linear regression model explained 62.8% of the variation in ACT scores. After including state as a categorical variable, this increased to 67.9%. An ANOVA test confirmed that adding state significantly improved the model (p < 0.001).

When comparing states after accounting for socioeconomic characteristics, Ohio, Wisconsin, and Washington had some of the highest predicted ACT scores, while Delaware and Wyoming had the lowest.

Overall, the findings suggest that both socioeconomic conditions and differences between states are important when examining educational inequality. However, these relationships do not necessarily indicate causation, and differences in ACT participation rates may influence state comparisons.

---

## Authors

- Mariana Butarov - [@MariButarov](https://github.com/MariButarov)

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Acknowledgements

- Tools/libraries used: The analysis was conducted in Python using Pandas and NumPy for data preparation, Matplotlib and Seaborn for visualization, Statsmodels for regression and statistical testing, and Scikit-learn for data preprocessing and model evaluation.
- Tutorials or papers referenced:The analysis was guided by tutorials and course materials provided by my Data Science professor, which helped me apply statistical methods, data preprocessing techniques, and regression analysis using Python.
- Inspiration or collaborators: The main inspiration for this project was an interest in understanding how socioeconomic differences relate to educational opportunities and academic performance, and how data analysis can help identify inequalities in education.

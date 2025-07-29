# Medical Insurance Statistical Modeling

## Overview

This project analyzes a medical insurance dataset ([medical_insurance.csv](medical_insurance.csv)) using Python for data cleaning, exploration,
visualization, and statistical modeling. 
The workflow is documented in [statistical_modelling.ipynb](statistical_modelling.ipynb).

## Workflow

### 1. Data Loading & Preparation

- Loaded the dataset using pandas.
- Checked for missing values and duplicates; duplicates were removed.
- Inspected data types and summarized the dataset.

### 2. Exploratory Data Analysis

- **Region Analysis:**  
  - Counted records per region.
  - Analyzed total premium paid by region.
  - Visualized premium distribution across regions.

- **Generation Analysis:**  
  - Segmented ages into generations (Child, Gen Z, Millennial, Gen X, Baby Boomer, Silent Generation).
  - Analyzed and visualized total premium paid by generation.

- **Correlation Analysis:**  
  - Generated a correlation matrix for numeric columns (`age`, `bmi`, `children`, `premium`).
  - Visualized correlations using a heatmap.

- **Pairplot Visualization:**  
  - Explored relationships between `age`, `bmi`, `children`, and `premium` across regions.

### 3. Statistical Modeling

- Built an Ordinary Least Squares (OLS) regression model to predict insurance premium based on `age`, `bmi`, and `children`.
- Displayed model summary for interpretation.

## Key Findings & Insights

1. **Regional Premium Distribution:**  
   - Certain regions contribute more to total premiums, indicating possible regional differences in insurance costs or population.

2. **Generational Premium Trends:**  
   - Premium payments vary significantly by generation, with some age groups (e.g., Millennials, Gen X) paying higher total premiums.

3. **Correlation Insights:**  
   - `age`, `bmi`, and `children` show varying degrees of correlation with `premium`.
   - `bmi` and `age` are positively correlated with premium, suggesting older individuals and those with higher BMI tend to pay more.

4. **Regression Model Results:**  
   - The OLS model confirms that `age`, `bmi`, and `children` are significant predictors of insurance premium.
   - The model summary provides coefficients and statistical significance for each variable.

## Recommendations

- **Targeted Insurance Products:**  
  - Develop region-specific insurance products to address regional premium disparities.
  - Tailor offerings for generations with higher premium payments.

- **Health & Wellness Initiatives:**  
  - Encourage wellness programs targeting BMI reduction, especially for age groups with higher premiums.

- **Further Analysis:**  
  - Incorporate additional variables (e.g., smoking status, medical history) for more accurate premium prediction.
  - Explore machine learning models for improved forecasting of future trends.

- **Data Quality:**  
  - Continue monitoring for missing values and duplicates to maintain data integrity.

## How to Run

1. Install required packages:
    ```sh
    pip install pandas numpy plotly matplotlib seaborn statsmodels
    ```
2. Open [statistical_modelling.ipynb](statistical_modelling.ipynb) in Jupyter or VS Code.
3. Run cells sequentially to reproduce the analysis and visualizations.

---

*Author: Awal Alier*

*Reading between the data*

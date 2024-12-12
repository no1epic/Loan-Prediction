# Loan Prediction Project

## Overview
This project, titled "Loan Prediction," focuses on analyzing and predicting loan repayment outcomes using a dataset from LendingClub. The primary objective is to determine the likelihood of loans being fully paid or charged off using various predictive models. The project was executed as part of the ALY6110: Big Data and Data Management course at Northeastern University.

## Dataset
The dataset, sourced from LendingClub and also available on Kaggle, contains information on loans issued between 2007 and 2017. It includes 1.6 million rows and 150 variables, with a size of 1.8 GB.

### Key Features:
- **Loan Amount:** Amount borrowed by the applicant.
- **Loan Term:** Loan duration in months (36 or 60).
- **Grade/Subgrade:** LendingClub's risk assessment score.
- **Interest Rate:** Annual interest rate for the loan.
- **Employment Length:** Borrower’s work experience in years.
- **Annual Income:** Borrower’s reported annual income.
- **Debt-to-Income Ratio (DTI):** Ratio of borrower’s debt obligations to income.

## Tools and Technologies
- **Databricks Platform:** For handling large datasets and executing computations.
- **Python:** Core programming language for data processing and modeling.
- **Matplotlib/Seaborn:** Libraries for visualization.
- **Machine Learning Models:** Logistic Regression, Decision Tree, and Random Forest.

## Process
### 1. Data Input
- Import the dataset into Databricks.
- Create a cluster for computation and run the notebook to analyze the data.

### 2. Data Cleaning
- Removed features with >40% missing values.
- Checked and ensured no duplicate values.
- Selected 28 key features for analysis.
- Corrected data types to match feature properties.

### 3. Exploratory Analysis
Analyzed the relationships between various features and loan repayment outcomes:
- **Loan Amount:** Higher loan amounts correlated with a higher likelihood of being charged off.
- **Term:** Five-year loans were over twice as likely to be charged off compared to three-year loans.
- **Interest Rate:** Higher interest rates were associated with higher charge-off probabilities.
- **Other Features:** Renters and individuals with less employment experience had higher charge-off rates.

### 4. Predictive Analysis
- **Feature Engineering:** Transformed categorical variables into dummy variables and normalized numerical data.
- **Models Used:**
  - Logistic Regression
  - Decision Tree
  - Random Forest
- **Model Performance:**
  - Logistic Regression had the highest precision and accuracy for predicting charge-offs.

## Results
- Logistic Regression emerged as the most effective model for loan prediction.
- Debt-to-Income Ratio, Interest Rate, and Revolving Balance were identified as key predictors.

## Insights
- Charged-off loans tend to have higher loan amounts, interest rates, and DTI.
- Loans with a five-year term are riskier than three-year loans.
- Borrowers with low annual income or limited work experience are more prone to defaults.

## Challenges
- Platform limitations for handling large datasets.
- Visualization constraints in Databricks.
- Balancing feature selection with business relevance.

## Future Enhancements
- Incorporate additional predictive models like XGBoost or Neural Networks.
- Expand the dataset with external economic indicators.
- Develop an interactive dashboard for real-time analysis.

## Team Members
- **Yiwei Wei** (wei.yiw@northeastern.edu)
- **Jiaming Ma** (ma.jianm@northeastern.edu)
- **Sahil Gawande** (gawande.s@northeastern.edu)

## License
This project is licensed under the MIT License. See the LICENSE file for details.

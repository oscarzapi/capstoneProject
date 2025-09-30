### Project Title
capstone Project

**OSCAR ZAMORA**

#### Executive summary
This notebook performs exploratory data analysis (EDA), missing value analysis, data cleaning, feature engineering. It addresses class imbalance using SMOTE, missing value handling, engineered features on the dataset that can be found at https://www.kaggle.com/code/igorvolianiuk/loan-approval-eda-catboost-optuna/input

#### Rationale
To optimize the processing time of a loan approval and predict upcoming loan requests status based on a selected number of input features in the banking / financial sector. The analysis will serve as a backup information for the real decisions taken by an entity.

#### Research Question
Who is eligible for a loan approval?

#### Data Sources
- **train.csv** - the training dataset; loan_status is the binary target
- **test.csv** - the test dataset; the objective is to predict probability of the target loan_status for each row.

#### Methodology
Will cover the following sections: 
- Missing Value Analysis: No missing values detected (per error), indicating clean datasets.
- Data Cleaning: Post-Cleaning Missing Values: 0
- Feature Engineering: New features (income_to_loan_ratio, debt_to_income_ratio, loan_interest_burden, etc.) capture affordability, risk, and stability.
- Exploratory Data Analysis: Imbalanced loan_status (~70–80% approved) addressed by SMOTE, improving minority class prediction.
- Data Clustering: Three clusters are detected depending on the age, income and employment length.
- Dimensionality Reduction with PCA: 8 components explain ~95% variance.
- Modelling with different Regression and classifier models

#### Results
Comparison table between all models' performance to detect the best models to be used.
How providing a test dataset we can detect whether new loan requests will be approved based on the input features and the best model selected.
The best model is XGBoost. It had the lowest total cost for the business: $1,835,102.90. It also had the highest accuracy of 95% and a strong F1 score of 0.805.


#### Next steps
- Tuning XGBoost (e.g., max_depth, learning_rate) to further minimize FP costs.
- Considering cost-sensitive learning to prioritize FP reduction.
- Exploring stacking XGBoost and Logistic Regression for better cost-performance trade-off.
- Monitoring SMOTE overfitting; if F1 plateaus, try undersampling or class weights.


#### Outline of project

- https://github.com/oscarzapi/capstoneProject/blob/main/capstoneProject.ipynb


##### Contact and Further Information

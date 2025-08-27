# Loan Approval Prediction Model
## Objective

This project predicts loan approval status based on applicant details such as income, education, employment type, credit score, and asset values. The objective is to assist financial institutions in making data-driven lending decisions and reduce risks of default.

## Dataset

The dataset contains applicant and financial details:

loan_id, no_of_dependents, education, self_employed

income_annum, loan_amount, loan_term, cibil_score

residential_assets_value, commercial_assets_value, luxury_assets_value, bank_asset_value

Target → loan_status (Approved / Rejected)

## Methodology

Data Preprocessing: Handled missing values, outliers, and encoded categorical variables.

Feature Engineering: Generated polynomial features to capture non-linear relationships.

Modeling: Tested Logistic Regression, Random Forest, and XGBoost.

Evaluation: Measured Accuracy, Precision, Recall, F1-score, and ROC-AUC.

## Results

Random Forest Classifier gave the best accuracy and generalization.

Top predictive features: CIBIL score, income, loan amount, and education level.

## Insights

Higher CIBIL scores and income strongly increase approval chances.

Asset values and loan size significantly influence decisions.

Employment and education have smaller but noticeable impact.

## Future Improvements

Add cross-validation for robust validation.

Deploy via Streamlit/Flask for real-time loan eligibility checking.

Train with real-world datasets for production-level accuracy.


## Installation & Setup
## Clone the Repository
git clone https://github.com/your-username/loan-approval-prediction.git
cd loan-approval-prediction

## Create Virtual Environment (Optional but Recommended)
python -m venv venv
source venv/bin/activate   # On Linux/Mac
venv\Scripts\activate      # On Windows

## Install Dependencies
pip install -r requirements.txt

## Contributing

Contributions are welcome! Feel free to fork this repo and submit a pull request.

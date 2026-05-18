# EasyVisa Approval Prediction

## Project Overview
This project predicts whether a visa application will be Certified or Denied using machine learning classification techniques. The goal is to support decision-making by identifying important applicant, employer, and job-related factors that influence visa approval outcomes.

## Business Problem
Visa application review can be time-consuming. This project uses historical visa application data to build a predictive model that helps identify profiles with higher or lower chances of approval.

## Dataset
The dataset contains structured visa application records with features related to:
- Employee education
- Job experience
- Job training requirement
- Region of employment
- Prevailing wage
- Wage unit
- Full-time position
- Employer details

Target variable:
- `case_status`: Certified or Denied

Note: Dataset is not included due to privacy/license restrictions.

## Tools and Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost

## Project Workflow
1. Data understanding
2. Exploratory Data Analysis
3. Data preprocessing
4. Feature encoding
5. Train-validation-test split
6. Model building
7. Model comparison
8. Hyperparameter tuning using GridSearchCV
9. Model evaluation
10. Feature importance analysis
11. Business recommendations

## Models Used
- Decision Tree
- Bagging Classifier
- Random Forest
- AdaBoost
- Gradient Boosting
- XGBoost

## Evaluation Metrics
The models were evaluated using:
- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

F1 Score was important because the dataset had class imbalance and both false positives and false negatives were meaningful.

## Key Findings
- Education level was one of the strongest predictors.
- Job experience positively influenced approval likelihood.
- Higher education levels such as Master's and Doctorate were associated with stronger certification outcomes.
- High School education appeared as a strong denial signal.
- Tuned XGBoost showed stable generalization.

## Business Recommendation
The model should be used as a decision-support tool, not as a fully automated decision system. Human review is important because visa decisions involve legal, ethical, and fairness considerations.

## Future Improvements
- Add fairness and bias evaluation
- Deploy model using Flask or FastAPI
- Track experiments using MLflow
- Add model monitoring for data drift
- Build a dashboard for stakeholder reporting

# Data

The dataset used for this project is publicly available on Kaggle as the EasyVisa dataset.

To run the notebook:
1. Download the dataset from Kaggle.
2. Place the CSV file in this `data/` folder.
3. Update the notebook file path if needed.

The raw dataset is not included in this repository to keep the project lightweight.

# Lead-Scoring-Case-Study

## Summary of Logistic Regression Lead Scoring Model

### Objective:
The goal of this case study was to construct a logistic regression model for assigning lead scores between 0 and 100, aiding the company in targeting potential leads with a conversion probability exceeding 80%.

## Methodology:

#### Data Preprocessing:
-> Analyzed dataset variables, checked for duplicates (none found).
-> Performed exploratory data analysis (EDA), handling missing values, and addressing outliers.
-> Investigated data distributions using count plots.
-> Explored numerical variables' correlations with the target variable.

#### Train-Test Split and Scaling:
-> Split the dataset into a 70:30 train-test ratio with a random state of 100.
-> Standardized numerical features.

#### Model Building:
-> Employed Recursive Feature Elimination (RFE) to select the top 15 most relevant variables.
-> Constructed a logistic regression model.
-> Evaluated model parameters like Variance Inflation Factor (VIF) and p-values, dropping variables with p-values > 0.05 or VIF > 5.
-> Attained an optimal model with VIF < 5 and p-values < 0.05 for all variables.

#### Model Evaluation:
-> Assessed model performance metrics, including accuracy, sensitivity, specificity, precision, recall, and F1-score.
-> Utilized the ROC curve to determine an ideal threshold (0.3) for classification.

#### Results (Train Set - Ideal Cutoff 0.3):
Accuracy: 92.6%
Sensitivity: 91.8%
Specificity: 93.1%
Precision: 89.3%
Recall: 91.8%
F1_score: 90.5%

#### Results (Test Set - Ideal Cutoff 0.3):
Accuracy: 91.4%
Sensitivity: 89.8%
Specificity: 92.2%
Precision: 86.8%
Recall: 89.8%
F1_score: 88.3%

#### Conclusion:
Focus on features like "Tags_Closed by Horizon," "Tags_Lost," and "Tags_Will revert after reading the email" to enhance lead conversion rates.
Improve the user interface (UI) of the app to provide a seamless experience, increasing user engagement.
Prioritize leads from the 'Welingak Website' as they exhibit higher conversion potential.
This model and analysis provide valuable insights to optimize lead conversion strategies and target potential leads more effectively.

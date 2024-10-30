
# Customer Churn Prediction Project

This project aims to predict customer churn using machine learning models with a focus on model evaluation techniques, data preprocessing, and feature engineering. The dataset used includes customer information such as monthly charges, tenure, and service usage patterns, along with churn labels.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Feature Engineering and Preprocessing](#feature-engineering-and-preprocessing)
4. [Modeling and Evaluation](#modeling-and-evaluation)
5. [Results](#results)
6. [License](#license)

---

### Project Overview

The primary objective of this project is to predict whether a customer is likely to churn using machine learning algorithms. The project includes preprocessing, feature engineering, model training, and evaluation steps, with particular attention to model interpretability through confusion matrices, and classification reports.



### Dataset

The dataset includes the following columns:

- **Customer Attributes**: Gender, SeniorCitizen status, Partner, Dependents.
- **Service Information**: MonthlyCharges, TotalCharges, Contract, PaperlessBilling, PaymentMethod.
- **Churn**: Binary indicator of customer churn.

Ensure the dataset is in the correct format and has no missing values for essential columns. Some preprocessing steps are applied to handle missing data and format inconsistencies.

### Feature Engineering and Preprocessing

1. **Data Cleaning**:
   - Converted categorical features to numerical using one-hot encoding.

2. **Feature Scaling**:
   - Used `StandardScaler` to normalize numerical features.

3. **Class Balancing**:
   - Used RandomOverSampler to balance classes due to an imbalance in the churn classes.

4. **Train-Test Split**:
   - Splits the dataset into training and testing sets with an 80-20 split.

### Modeling and Evaluation

The models used in this project include:
1. **XGBoost Classifier**: The primary model for churn prediction.
2. **Alternative Models**: Random Forest Classifier, Decision Tree Classifier.

**Model Evaluation**:
   - Confusion Matrix: Plots True Negatives, False Positives, False Negatives, and True Positives.
   - Classification Report: Displays precision, recall, and F1-score.

Key Code Snippets:
- **Confusion Matrix**: Displays predicted vs. actual values for model interpretation.
- **Classification Report**: Helps identify recall and precision for each class.

### Results

- **Model Performance**: Achieved an overall accuracy of approximately 70-81%, depending on the classifier.
- **Recall and Precision Analysis**: Class imbalance addressed, but precision and recall vary, with higher recall on churned customers.
- **Feature Importance**: Highlights impactful features like `Contract`, `MonthlyCharges`, and `OnlineSecurity`.

### License

This project is licensed under the MIT License.


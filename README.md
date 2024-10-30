
# Customer Churn and Profit Analysis

This project analyzes customer churn data to build predictive models and calculate net profits associated with different customer retention strategies. Using machine learning and financial analysis, it aims to provide actionable insights into reducing customer churn and optimizing profit through realistic retention strategies.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Project Structure](#project-structure)
4. [Machine Learning Models](#machine-learning-models)
5. [Financial Analysis](#financial-analysis)
6. [Setup and Usage](#setup-and-usage)
7. [Dependencies](#dependencies)
8. [Results](#results)

---

### Project Overview

The main goal of this project is to predict customer churn and evaluate the financial impact of customer retention strategies. We use customer behavioral and demographic data to create machine learning models that predict whether a customer will churn and perform a profit analysis based on potential retention strategies and costs.

### Dataset

The dataset includes the following main columns:

- **Demographic data:** `gender`, `SeniorCitizen`, `Partner`, `Dependents`
- **Service usage data:** `PhoneService`, `MultipleLines`, `InternetService`, `OnlineSecurity`, `OnlineBackup`, `DeviceProtection`, `TechSupport`, `StreamingTV`, `StreamingMovies`
- **Account information:** `Contract`, `PaperlessBilling`, `PaymentMethod`, `MonthlyCharges`, `TotalCharges`
- **Target:** `Churn` (whether the customer left)

### Project Structure

The project includes the following stages:

1. **Data Preprocessing:** Cleaning and encoding data, handling missing values, and preparing data for modeling.
2. **Feature Engineering:** Selecting and creating new features to enhance model accuracy.
3. **Machine Learning Modeling:** Training multiple models to predict churn.
4. **Financial Analysis:** Evaluating profit based on churn predictions and calculating net profit under different retention strategies.

### Machine Learning Models

Several machine learning models were developed and evaluated using metrics such as ROC-AUC and accuracy. Key models include:

- **Random Forest Classifier**
- **Decision Tree Classifier**
- **XGBoost Classifier**

The best-performing model was chosen for the final churn predictions.

### Financial Analysis

A detailed financial analysis was added to calculate the **net profit** for different customer retention strategies. This includes:

1. **Average Monthly Revenue Calculation:** Using actual customer `MonthlyCharges` data to calculate potential yearly revenue per customer.
2. **Retention Scenarios:** Simulating revenue based on different customer retention rates (20%, 50%, 100%).
3. **Retention Costs:** Assessing the net profit associated with various retention costs per customer (e.g., $50, $100, up to $300).
4. **Visualization:** Plotting net profit outcomes across various retention rates and costs to provide a realistic financial outlook.

### Setup and Usage

1. **Clone the repository:**
   ```bash
   git clone https://github.com/adamw80/Customer-Churn-and-Profit-Analysis.git
   cd Customer-Churn-and-Profit-Analysis
   ```

2. **Install dependencies:**
   Ensure you have Python 3.6+ and install required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the analysis:**
   Open and run the Jupyter Notebook:
   ```bash
   jupyter notebook Customer\ Churn\ and\ Profit\ Analysis.ipynb
   ```

### Dependencies

The project relies on the following packages:

- **Pandas:** Data manipulation
- **NumPy:** Numerical computations
- **Scikit-Learn:** Machine learning model building
- **XGBoost:** Gradient boosting model
- **Matplotlib/Seaborn:** Data visualization
- **Imbalanced-learn:** Handling imbalanced datasets for model training

### Results

The analysis shows that specific retention strategies can significantly affect net profit, depending on the retention cost and targeted retention rate. Key findings include:

- **Churn Prediction:** The model provided accurate predictions for customer churn, enabling targeted retention.
- **Financial Impact:** Retention costs have a critical threshold beyond which net profit decreases. Visualizations provide insights into optimal retention costs per customer to maximize profitability.

### Author

Adam Rivard-Walter  
For further questions or inquiries, please reach out on LinkedIn or GitHub.


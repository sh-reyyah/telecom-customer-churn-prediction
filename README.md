# Customer Churn Prediction

This project aims to predict customer churn using machine learning models. The dataset used is the "customer_churn.csv" file, which contains various features related to customer behavior and demographics. The goal is to build and compare the performance of Logistic Regression and XGBoost models in predicting customer churn.

## Table of Contents

- [Dataset](#dataset)
- [Preprocessing](#preprocessing)
- [Model Training](#model-training)
- [Evaluation](#evaluation)
- [Visualization](#visualization)
- [Usage](#usage)
- [Dependencies](#dependencies)
- [Contributing](#contributing)

## Dataset

The dataset used in this project is the "customer_churn.csv" file, which contains the following columns:
- `customerID`: Unique identifier for each customer.
- `gender`: Gender of the customer.
- `SeniorCitizen`: Whether the customer is a senior citizen (0 or 1).
- `Partner`: Whether the customer has a partner (0 or 1).
- `Dependents`: Whether the customer has dependents (0 or 1).
- `tenure`: Number of months the customer has stayed with the company.
- `PhoneService`: Whether the customer has a phone service (0 or 1).
- `MultipleLines`: Whether the customer has multiple lines (0 or 1).
- `InternetService`: Type of internet service (0: No, 1: DSL, 2: Fiber optic).
- `OnlineSecurity`: Whether the customer has online security (0 or 1).
- `OnlineBackup`: Whether the customer has online backup (0 or 1).
- `DeviceProtection`: Whether the customer has device protection (0 or 1).
- `TechSupport`: Whether the customer has tech support (0 or 1).
- `StreamingTV`: Whether the customer has streaming TV (0 or 1).
- `StreamingMovies`: Whether the customer has streaming movies (0 or 1).
- `Contract`: Type of contract (0: Month-to-month, 1: One year, 2: Two year).
- `PaperlessBilling`: Whether the customer has paperless billing (0 or 1).
- `PaymentMethod`: Payment method (0: Bank transfer (automatic), 1: Credit card (automatic), 2: Electronic check, 3: Mailed check).
- `MonthlyCharges`: Monthly charges for the customer.
- `TotalCharges`: Total charges for the customer.
- `Churn`: Whether the customer has churned (0 or 1).

## Preprocessing

The preprocessing steps include:
- Converting `TotalCharges` to numeric and handling missing values.
- Encoding categorical variables using `LabelEncoder`.
- Dropping the `customerID` column.
- Splitting the data into training and testing sets.
- Scaling the features using `StandardScaler`.

## Model Training

Two models are trained and evaluated:
- **Logistic Regression**: A simple and interpretable model.
- **XGBoost**: A powerful ensemble model.

## Evaluation

The models are evaluated using the following metrics:
- Accuracy
- AUC (Area Under the ROC Curve)

The evaluation results are compared using bar charts and ROC curves.

## Visualization

The project includes visualizations for:
- Model performance comparison (accuracy and AUC).
- Confusion matrices for both models.
- ROC curves for both models.
- Prediction visualization for new data.

## Usage

To run the project, follow these steps:
1. Clone the repository.
2. Install the required dependencies (see below).
3. Run the `main.py` script.

```bash
git clone https://github.com/your-username/customer-churn-prediction.git
cd customer-churn-prediction
pip install -r requirements.txt
python main.py

Contributing
Contributions are welcome! Please open an issue or submit a pull request with your changes.

Note: This project is for educational purposes only. The dataset and models are simplified for demonstration purposes.
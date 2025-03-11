#  Credit-Risk
A machine learning project to assess credit risk based on customer data. The goal is to predict credit risk by analyzing historical data using various machine learning models.

---

##  Folder Structure
- `data/`: Contains raw data files (CSV format).
- `notebooks/`: Jupyter Notebooks for different stages:
   - `data_preprocessing/`: EDA and data cleaning steps.
   - `model_building/`: Model training and evaluation.
- `src/`: Optional scripts for data processing and models.

---

##  Data Disclaimer
The dataset included in this repository is anonymized and does not contain any personally identifiable information (PII). It is shared for educational and research purposes only.

---

##  Dataset Description
| **Column Name** | **Description**                                                                                     |
|-----------------|-----------------------------------------------------------------------------------------------------|
| `X1`            | Aggregate risk indicator score.                                                                      |
| `X2`            | Months since the oldest account was opened.                                                          |
| `X3`            | Months since the newest account was opened.                                                          |
| `X4`            | Average number of months since all accounts were opened.                                             |
| `X5`            | Number of accounts with a positive payment history.                                                  |
| `X6`            | Number of accounts overdue by at least 60 days.                                                      |
| `X7`            | Number of accounts overdue by at least 90 days.                                                      |
| `X8`            | Percentage of accounts that have never had late payments.                                            |
| `X9`            | Months since the last overdue payment.                                                               |
| `X10`           | Most significant delay or registry entry in the last 12 months.                                      |
| `X11`           | Most significant delay in account history.                                                           |
| `X12`           | Total number of credit accounts.                                                                     |
| `X13`           | Number of accounts opened in the last 12 months.                                                     |
| `X14`           | Percentage of revolving accounts (e.g., credit cards).                                               |
| `X15`           | Months since the last credit inquiry (excluding inquiries from the last 7 days).                     |
| `X16`           | Number of credit inquiries in the last 6 months.                                                     |
| `X17`           | Number of credit inquiries in the last 6 months (excluding those from the last 7 days).               |
| `X18`           | Percentage of available limit utilization on revolving accounts (balance divided by credit limit).   |
| `X19`           | Percentage of revolving credit repayment (balance divided by original loan amount).                  |
| `X20`           | Number of revolving accounts with a negative balance.                                                |
| `X21`           | Number of installment accounts with a negative balance.                                              |
| `X22`           | Number of bank accounts with a high utilization ratio.                                               |
| `X23`           | Percentage of accounts with a negative balance.                                                      |
| `Target`        | Credit risk (0 = Low, 1 = High).                                                                    |

---

## Data Preprocessing
- **Handling Missing Values:** 
  - Imputed using median for numerical features.
  - Mode for categorical features.

- **Encoding:**
  - One-Hot Encoding for `X10` and `X11`.

- **Feature Scaling:**
  - Standardization for numerical features.

---

## Exploratory Data Analysis (EDA)
- **Key Insights:**
   - Distribution analysis for numerical features.
   - Correlation heatmap to identify relationships.
   - Box plots to detect outliers.

---

## Models Used
The following models were trained and evaluated:
- **Random Forest Classifier**
- **Bagging Classifier**
- **Extra Trees Classifier**
- **Gradient Boosting Classifier**
- **Logistic Regression**
- **Support Vector Machine (SVM)**
- **Naive Bayes Classifier**
- **Decision Tree Classifier**

```

## How to Use
1. Run `model_building.ipynb` to train and save the models.
2. Run `model_evaluation.ipynb` to evaluate and compare models.

## Evaluation Metrics
Each model is evaluated using:
- **Accuracy**
- **Precision, Recall, F1-score**
- **Confusion Matrix**
- **ROC Curve and AUC Score**

## Installation
To clone and run the project locally:
```bash
git clone https://github.com/gondeka03/Credit-Risk.git
cd Credit-Risk
pip install -r requirements.txt

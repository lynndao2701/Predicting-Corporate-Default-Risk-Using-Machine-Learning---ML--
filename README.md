# 📉 Predicting Corporate Default Risk Using Machine Learning

## 📌 Overview
This project builds machine learning models to predict **corporate default risk** using firm-level financial ratios, cash flow indicators, ESG scores, and industry data. The primary model used is a **Decision Tree classifier**, supported by comparative analysis with **Logistic Regression, Random Forest, and Support Vector Classifier (SVC)**.
The project demonstrates how financial indicators and non-financial factors contribute to default probability, and how model tuning improves prediction accuracy.

## 🎯 Objectives
* Identify key determinants of corporate default risk
* Build and interpret a Decision Tree model
* Compare model performance across multiple ML algorithms
* Use scaling, parameter tuning, and robustness checks to improve accuracy
* Provide insights and recommendations for risk assessment

## 🧰 Dataset & Processing
* **100,000 simulated firm-level observations**
* Variables include:
  * Debt-to-Asset Ratio
  * Current Ratio
  * ROA (Return on Assets)
  * Firm Size (log assets)
  * Cash Flow to Debt
  * ESG Score
  * Industry Sector
* Simulated data allows consistency, avoids confidentiality issues, and removes missing/noisy values.
* Data scaling applied to improve model performance.

## 📊 Key Models
### **Decision Tree (Main Model)**
* Baseline Accuracy: **88%**
* After tuning (entropy, depth=15, min_leaf=10): **91% accuracy**
* Balanced precision & recall for both default and non-default classes

### **Comparison Models**
| Model               | Accuracy  | Notes                                             |
| ------------------- | --------- | ------------------------------------------------- |
| Logistic Regression | **92%**   | Stable, interpretable, strong probability outputs |
| Random Forest       | **91.5%** | Handles nonlinearity, reduces overfitting         |
| SVC (RBF kernel)    | **92%**   | Captures complex boundaries                       |

## 📈 Key Insights
* Higher **leverage** significantly increases default probability
* Stronger **liquidity**, **profitability (ROA)**, and **cash flow** reduce risk
* **Larger firms** show lower default likelihood
* Poor **ESG performance** has a small but meaningful positive effect on default risk
* Model tuning and scaling improve Decision Tree performance by ~3%

## 🧪 Methods Applied
* Data generation & preprocessing
* Variable justification using financial theory
* Correlation analysis
* Decision Tree construction & tuning
* Model comparison (Logistic Regression, Random Forest, SVC)
* Performance metrics: Accuracy, Precision, Recall, F1, ROC curve

## ⚠️ Limitations
* Simulated data does not capture real-world volatility
* High variable correlations may increase overfitting
* Limited macroeconomic factors reduce predictive power

## ➕ Recommendations
* Add macroeconomic indicators (GDP growth, interest rates, volatility)
* Use advanced ensemble methods (Gradient Boosting, XGBoost)
* Incorporate real ESG & transaction data for early warning signals

## 📜 Purpose
This project demonstrates how machine learning can support **credit risk assessment**, helping investors and financial institutions better understand default probabilities using interpretable and comparative modelling.

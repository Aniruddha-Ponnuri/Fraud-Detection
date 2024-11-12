
# 📈 Credit Card Fraud Detection Using Machine Learning

---

🚀 **Welcome to the Credit Card Fraud Detection Project!**

In today's digital age, protecting against fraudulent transactions is more crucial than ever. This project leverages machine learning to help financial institutions quickly and accurately identify fraud, enhancing security and user trust. Let’s dive into how we built this robust fraud detection system!

---

## 💾 Dataset Overview
The dataset contains European credit card transactions from **September 2013** with a total of **284,807 records**:
- **Legitimate Transactions:** 284,315 (99.83%)
- **Fraudulent Transactions:** 492 (0.17%)

💡 **Challenge:** The dataset is highly imbalanced, typical of real-world fraud detection problems.

### Features
- **Anonymized Features:** V1 to V28 (due to privacy concerns)
- **Transaction Amount:** Provides context on the scale of the transaction
- **Class:** Target variable where:
  - **0:** Legitimate transaction
  - **1:** Fraudulent transaction

---

## 🛠️ How We Tackled It

### 1️⃣ **Data Preprocessing**
- **Scaling:** Standardized the features using `StandardScaler`.
- **Missing Values:** Handled appropriately to maintain data integrity.
- **Visualization:** Explored data patterns using histograms and correlation heatmaps.

### 2️⃣ **Handling Imbalanced Data**
- **SMOTE:** Synthetic Minority Over-sampling Technique for generating synthetic fraud samples.
- **Random Under-sampling:** Reduced the majority class (legitimate transactions) for a balanced dataset.

### 3️⃣ **Model Selection**
We experimented with multiple algorithms to find the best fit:
- **Logistic Regression:** As a baseline model
- **Decision Trees & KNN:** To capture non-linear patterns
- **Random Forest & Gradient Boosting:** Ensemble methods for improved performance on imbalanced data

🏆 **Best Model:** Random Forest with hyperparameter tuning

---

## 📊 Evaluation Metrics

Given the class imbalance, accuracy alone isn’t sufficient. We focused on:
- **Precision:** To minimize false positives (incorrectly flagged transactions)
- **Recall:** To catch as many fraudulent transactions as possible
- **F1-Score:** Balance between precision and recall
- **AUC-ROC:** Measures the model's ability to distinguish between classes

| Metric       | Value     |
|--------------|-----------|
| Precision    | 0.92      |
| Recall       | 0.94      |
| F1-Score     | 0.93      |
| AUC-ROC      | 0.98      |

---

## 🌐 Web Application Integration

We integrated our model into a sleek **web application**:
- **Frontend:** Simple, user-friendly interface in `FraudDetection.html`
- **Real-time Predictions:** The model processes transactions in real-time and provides immediate feedback.

🖥️ **How to Run the App:**
1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```
2. Open `FraudDetection.html` in your browser.

Enjoy an intuitive interface that flags fraudulent transactions with clear visual indicators!

---

## 🔮 Future Enhancements
- **Continuous Learning:** Implement adaptive retraining to handle evolving fraud tactics.
- **Advanced Feature Engineering:** Explore time-series analysis for better insights.

---

## 🙋‍♂️ Meet the Team
- **Ponnuri Aniruddha (RA2112704010015)**
- Faculty Guide: **Dr. K. Shantha Kumari**, Associate Professor, SRMIST

🎓 This project was developed as part of the Financial Machine Learning coursework (Subject Code: 21CSC426T).

# 🏦 Bank Churn Prediction (Dự Đoán Khách Hàng Rời Bỏ Ngân Hàng)

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Data-Science](https://img.shields.io/badge/Domain-Banking%20%26%20Finance-orange.svg)
![Machine-Learning](https://img.shields.io/badge/Framework-Scikit--Learn%20%7C%20Gradio-green.svg)

## 📌 Project Overview (Tổng Quan Dự Án)
In the banking sector, retaining existing customers is often far more cost-effective than acquiring new ones. This project focuses on building an end-to-end Machine Learning pipeline to predict customer churn (the probability of a customer leaving the bank). By identifying high-risk customers early, the bank's marketing and CRM departments can proactively deploy targeted retention strategies (e.g., tailored financial products, loyalty rewards).

*Trong ngành ngân hàng, việc giữ chân khách hàng cũ hiệu quả hơn nhiều so với tìm kiếm khách hàng mới. Dự án này xây dựng một pipeline Học máy toàn diện nhằm dự đoán khả năng rời bỏ dịch vụ của khách hàng, giúp ngân hàng đưa ra các chiến lược giữ chân kịp thời.*

---

## 💼 Business Problem & Impact (Bài Toán Kinh Doanh)
* **Problem:** Customer attrition directly affects the bank's total assets, transaction volume, and interest income.
* **Goal:** Develop a highly accurate classification model to detect churn signals based on demographics, credit scores, account balances, and activity history.
* **Actionable Insight:** Group customers by risk levels to optimize marketing costs for retention campaigns.

---

## 📊 Dataset Description (Tổng Quan Dữ Liệu)
The dataset contains historical customer profiles with features including:
* **Demographics:** Age, Gender, Geography.
* **Financial Profile:** Credit Score, Balance, Estimated Salary, Number of Products used.
* **Engagement:** Tenure, Is Active Member, Has Credit Card.
* **Target Variable:** `Exited` (1: Churned, 0: Retained).

---

## 🛠️ Tech Stack & Architecture (Công Nghệ Sử Dụng)
* **Data Processing & EDA:** `Python`, `Pandas`, `NumPy`, `Matplotlib`, `Seaborn`.
* **Machine Learning:** `Scikit-Learn` (utilizing **Support Vector Classifier - SVC**, Hyperparameter Tuning).
* **Model Deployment (UI):** `Gradio` for building a web-based interactive interface for real-time prediction.

---

## 🚀 Machine Learning Pipeline (Quy Trình Triển Khai)

### 1. Exploratory Data Analysis (EDA)
* Analyzed the distribution of financial behavior between active and inactive members.
* Handled class imbalance (since churned customers typically account for a minority of the banking dataset).

### 2. Data Preprocessing & Feature Engineering
* Handled categorical variables using One-Hot Encoding (for `Geography`, `Gender`).
* Applied **Feature Scaling** using `StandardScaler` to optimize distance-based algorithms like Support Vector Machines (SVM).

### 3. Model Training & Evaluation
* Implemented **Support Vector Classifier (SVC)** to capture complex non-linear relationships in customer profiles.
* **Evaluation Metrics:** Evaluated using Confusion Matrix, Precision, Recall, and F1-Score to ensure the model performs well on the minority class (Churned).

### 4. Interactive Interface (Gradio Deployment)
* Developed a user-friendly UI where credit officers or relationship managers can input custom parameters (Credit Score, Age, Balance, etc.) and get an instant risk assessment probability.

---

## 🖥️ User Interface Preview (Giao Diện Ứng Dụng)
<img width="1860" height="859" alt="image" src="https://github.com/user-attachments/assets/a9fd9b4a-8930-4ab6-a620-6796f0ac7777" />

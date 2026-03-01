# ✈️ Customer Booking Prediction using Machine Learning

## 📌 Project Overview

In today’s competitive airline industry, customers make booking decisions long before arriving at the airport. 

This project builds a Machine Learning model to predict whether a customer will complete a holiday booking.

The goal is to help airlines:
- Identify high-potential customers
- Improve marketing strategies
- Increase booking conversion rates


---

## 🎯 Business Objective

- Predict whether a customer will complete a booking (`booking_complete`)
- Identify key factors influencing booking decisions
- Provide actionable business insights


---

## 📊 Dataset Information

- Total Records: 10,000
- Target Variable: `booking_complete`
  - 0 = No Booking
  - 1 = Booking Completed

### Key Features:
- Number of passengers
- Sales channel
- Trip type
- Purchase lead time
- Length of stay
- Flight hour & day
- Booking origin
- Extra baggage selection
- Preferred seat selection
- In-flight meal selection
- Flight duration

⚠ Dataset is imbalanced:
- No Booking: 8,520
- Booking: 1,480


---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook


---

## ⚙ Project Workflow

### 1️⃣ Data Exploration
- Checked missing values
- Analyzed data types
- Reviewed class distribution

### 2️⃣ Data Preprocessing
- One-hot encoding for categorical variables
- Feature engineering (e.g., weekend feature)
- Train-test split (80% training, 20% testing)

### 3️⃣ Model Building
Model Used:
Random Forest Classifier

Why Random Forest?
- Handles mixed data types
- Reduces overfitting
- Provides feature importance


---

## 📈 Model Evaluation

### Accuracy: 85%

### Classification Report

Class 0 (No Booking):
- Precision: 0.87
- Recall: 0.98
- F1-score: 0.92

Class 1 (Booking):
- Precision: 0.51
- Recall: 0.13
- F1-score: 0.21

### Confusion Matrix

[[8336  184]  
 [1286  194]]


---

## 🔍 Key Findings

- Model predicts non-bookings very well.
- Model struggles to detect actual bookings (low recall for class 1).
- Important predictors include:
  - Purchase lead time
  - Flight duration
  - Length of stay
  - Add-on selections
  - Booking origin


---

## 💡 Business Insights

- Customers selecting add-ons (baggage, meals, seats) show higher purchase intent.
- Early planners are more likely to complete bookings.
- Model accuracy is high, but booking detection needs improvement.


---

## 🚀 Recommendations

- Apply class balancing techniques (SMOTE)
- Optimize model for Recall instead of Accuracy
- Perform hyperparameter tuning
- Test advanced models like XGBoost or Gradient Boosting


---


## 👨‍💻 Author

UZAIR KHAN THE DATA ANALYST 
Python | Machine Learning | Data Analysis  


---

## ⭐ Conclusion

This project demonstrates:
- Data cleaning
- Feature engineering
- Machine learning modeling
- Model evaluation
- Business interpretation

The model shows strong overall performance but requires improvement in detecting actual booking customers before production deployment.

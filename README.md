# Ad Click Prediction Analysis

## 📌 Project Overview
This project uses **Logistic Regression** to predict whether a user will click on an advertisement based on their demographics and internet usage patterns. The goal is to help businesses target the right audience effectively.

## 📊 Dataset Features
The dataset contains information about 1,000 users, including:
* **Daily Time Spent on Site:** Time in minutes.
* **Age:** User age in years.
* **Area Income:** Average income of the user's geographical area.
* **Daily Internet Usage:** Average minutes per day spent on the internet.
* **Clicked on Ad:** The target variable (0 = No, 1 = Yes).

## 🛠️ Key Steps Taken
1. **Data Cleaning:** Removed non-predictive columns (Timestamp, City, Country, Ad Topic).
2. **Feature Engineering:** Split the data into training (70%) and testing (30%) sets.
3. **Feature Scaling:** Applied `StandardScaler` to normalize the data for better model performance.
4. **Modeling:** Trained a Logistic Regression model to classify user behavior.

## 🚀 Technologies Used
* **Python**
* **Pandas & NumPy** (Data Manipulation)
* **Matplotlib & Seaborn** (Data Visualization)
* **Scikit-Learn** (Machine Learning)

## 📈 Results
* The model successfully predicts ad clicks with high precision and recall.
* Visual analysis shows that younger users with high internet usage are less likely to click, while specific demographics show higher engagement.

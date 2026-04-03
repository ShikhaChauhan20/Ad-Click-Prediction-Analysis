# 🎯 ConnectSphere: Advanced Ad-Click Prediction & Self-Correcting AI

This project implements an end-to-end Machine Learning pipeline to predict advertisement engagement. Beyond standard classification, this system incorporates **Semi-Supervised Self-Learning** and **Reinforcement Learning** to optimize ad delivery and "self-correct" targeting failures in real-time.

---

## 🚀 Key Technical Innovations

### 1. Semi-Supervised Self-Learning
In real-world digital marketing, we often have massive amounts of user data but limited "labels" (knowing if they clicked or not). 
* **Implementation:** Used `SelfTrainingClassifier` with a **Logistic Regression** base.
* **Impact:** The model "teaches itself" by assigning pseudo-labels to unlabeled data where it has >80% confidence, improving accuracy to **97%**.

### 2. Reinforcement Learning (Failure Correction)
Traditional models are static. To make ConnectSphere dynamic, I implemented an **Epsilon-Greedy RL Agent**.
* **The Problem:** Showing expensive ads to "heavy" internet users who have developed "ad blindness."
* **The Solution:** The RL Agent treats ad delivery as a **Multi-Armed Bandit** problem. It identifies low-performing ads (failures) and automatically shifts the budget toward high-CTR (Click-Through Rate) designs.

### 3. Feature Intelligence & Decision Mapping
Using **StandardScaler** and coefficient analysis, the model identified that **Daily Internet Usage** is the strongest predictor of engagement.

---

## 📊 Visualizing the "Targeting Sweet Spot"

The following map shows the **Learned Decision Boundary**. The green shaded region represents the "Optimized Targeting Zone" where the model has self-corrected to focus ad spend.

![Model Intelligence Map](model_intelligence_map.png)

* **Red Zone (Failures):** High-usage users identified as non-converters.
* **Green Zone (Success):** The behavioral "sweet spot" for maximum ROI.

---

## 🛠️ Tech Stack & Tools
* **Language:** Python 3.10
* **Libraries:** Scikit-Learn, Pandas, NumPy, Seaborn, Matplotlib
* **Environment:** Google Colab / Jupyter Notebook
* **Algorithm:** Logistic Regression (Wrapper: Self-Training) + RL (Epsilon-Greedy)

---

## 📈 Business Impact
By deploying this self-correcting logic, ConnectSphere can:
1. **Reduce Ad Waste:** Automatically filter out segments with low engagement probability.
2. **Maximize ROAS:** Allocate budget to high-performing user clusters identified by the RL agent.
3. **Scale with Less Data:** Use self-learning to maintain high accuracy even with incomplete datasets.

---

### 🎓 Academic Context
**Author:** Shikha Chauhan Mantasha Fatima Archie Chauhan Riddhi Dayani
**University:** DIT University, Dehradun  
**Course:** B.Tech CSE (4th Semester)  
**Project Category:** AI / Machine Learning Portfolio

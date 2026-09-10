# 🎥 YouTube Category Predictor (Machine Learning)

## 📌 Description
This project is an end-to-end Machine Learning pipeline designed to predict the category of a YouTube channel based on its performance metrics (Views, Subscribers, and Country). The model classifies channels into three main categories: **Lifestyle**, **Entertainment**, and **Education**.

## 🛠️ Technologies Used
*   **Python 3**
*   **Jupyter Notebook**
*   **Data Manipulation:** Pandas, NumPy
*   **Machine Learning:** Scikit-learn (KNN, Decision Tree, Naive Bayes, Random Forest), XGBoost
*   **Data Visualization:** Matplotlib, Seaborn
*   **Data Preprocessing:** RobustScaler, LabelEncoder, SelectKBest (ANOVA)

## ✨ Key Features
*   **Data Exploration & Cleaning:** Handled missing values, analyzed distributions, and detected outliers using the IQR method.
*   **Feature Engineering:** Applied `RobustScaler` to handle right-skewed data and `SelectKBest` (ANOVA F-score) to identify the most impactful features (Views was found to be the most significant).
*   **Multi-class Classification:** Trained and evaluated 5 different models:
    1. K-Nearest Neighbors (KNN)
    2. Decision Tree
    3. Naive Bayes
    4. Random Forest
    5. XGBoost (Best Performer with ~61.5% accuracy)
*   **Model Evaluation:** Utilized Confusion Matrices, Classification Reports, and Micro-averaged ROC-AUC curves to compare model performance.
*   **Real-time Prediction:** The model accepts custom user inputs (e.g., 1,000,000 Views, 50,000 Subscribers, US) and predicts the likely channel category.

## 🚀 How to Run
1. Clone this repository.
2. Install the required Python libraries:
   ```bash
   pip install pandas numpy scikit-learn xgboost matplotlib seaborn

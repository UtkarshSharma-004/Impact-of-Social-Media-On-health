# 🧠 Social Media Mental Health Prediction Using Machine Learning

## 📌 Project Overview

This project focuses on analyzing the impact of social media usage on mental health using Machine Learning techniques. The system predicts the overall impact of social media usage on students/users based on several behavioral and lifestyle-related factors.

The project includes:

* Data preprocessing and cleaning
* Exploratory Data Analysis (EDA)
* Multiple Machine Learning algorithms
* Comparative model analysis
* Clustering techniques
* Feature importance analysis
* Streamlit web application deployment

---

# 🎯 Problem Statement

The rapid growth of social media platforms has significantly influenced users' mental health, sleep patterns, and academic performance. This project aims to predict whether the overall impact of social media usage is:

* Positive
* Neutral
* Negative

using Machine Learning models trained on behavioral and social media usage data.

---

# 📂 Dataset

Dataset Used:

* Impact of Social Media on Health Dataset

Features used in the project:

* Age
* Gender
* Academic_Level
* Avg_Daily_Usage_Hours
* Most_Used_Platform
* Affects_Academic_Performance
* Sleep_Hours_Per_Night

Target Variable:

* Overall_Impact

---

# ⚙️ Technologies Used

## Programming Language

* Python

## Libraries and Frameworks

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* XGBoost
* Streamlit
* Pickle

---

# 📊 Exploratory Data Analysis (EDA)

EDA was performed to understand the dataset and identify relationships between features.

Key analysis included:

* Correlation Heatmap
* Feature Distribution Analysis
* Target Variable Distribution
* Sleep Hours vs Mental Health Analysis
* Social Media Usage vs Mental Health Analysis

### Important Observation

A strong correlation was observed between:

* Sleep_Hours_Per_Night
* Mental_Health_Score

Since users may not directly know their mental health score during deployment, the feature was removed from the final deployed model to improve practical usability.

---

# 🤖 Machine Learning Models Used

The following Machine Learning algorithms were implemented and evaluated:

| Algorithm                    | Purpose                       |
| ---------------------------- | ----------------------------- |
| Logistic Regression          | Baseline Classification Model |
| Decision Tree                | Rule-Based Classification     |
| Random Forest                | Ensemble Learning             |
| K-Nearest Neighbors (KNN)    | Distance-Based Classification |
| Naive Bayes                  | Probabilistic Classification  |
| Support Vector Machine (SVM) | Margin-Based Classification   |
| XGBoost                      | Boosting Ensemble Technique   |
| K-Means Clustering           | User Behavior Clustering      |
| DBSCAN                       | Density-Based Clustering      |

---

# 📈 Model Comparison

The performance of all classification algorithms was compared using accuracy scores.

| Model               | Accuracy |
| ------------------- | -------- |
| Logistic Regression | 90.02%   |
| Decision Tree       | 97.65%   |
| Random Forest       | 98.82%   |
| KNN                 | 93.55%   |
| Naive Bayes         | 90.32%   |
| SVM                 | 95.89%   |
| XGBoost             | 98.82%   |

---

# 🏆 Best Model Selection

Both Random Forest and XGBoost achieved the highest accuracy of 98.82%.

However, Random Forest was selected as the final deployment model because:

* High prediction accuracy
* Better interpretability
* Lower complexity compared to XGBoost
* Reduced overfitting risk
* Easier deployment workflow

---

# 🔍 Clustering Analysis

Two clustering algorithms were implemented:

## 1. K-Means Clustering

K-Means was used to identify hidden behavioral groups among users.

### Techniques Used

* Elbow Method
* Cluster Visualization

## 2. DBSCAN

DBSCAN was used for density-based clustering and outlier detection.

### Advantages

* Handles noise and outliers
* Does not require predefined cluster count

---

# 📌 Feature Importance Analysis

Feature importance analysis was performed using Random Forest.

Most influential features:

* Avg_Daily_Usage_Hours
* Sleep_Hours_Per_Night
* Affects_Academic_Performance

This helped identify which factors contribute most toward predicting mental health impact.

---

# 🚀 Deployment

The final model was deployed using Streamlit.

## Deployment Features

The web application allows users to:

* Enter social media usage details
* Provide sleep and academic information
* Predict overall mental health impact instantly

## Deployment Workflow

1. User enters input data
2. Input is encoded and processed
3. Pipeline model performs prediction
4. Predicted result is displayed

---

# 🧩 Pipeline Implementation

A Scikit-learn Pipeline was used to combine:

* Feature Scaling
* Model Training

Benefits of using Pipeline:

* Cleaner workflow
* Automated preprocessing
* Consistent deployment
* Reduced preprocessing errors

---

# 📁 Project Structure

```
project/
│
├── app.py
├── best_pipeline.pkl
├── requirements.txt
├── cleaned_dataset.csv
├── notebooks/
│   ├── EDA.ipynb
│   └── Model_Training.ipynb
└── README.md
```

---

# ▶️ Run the Project

## Install Dependencies

```bash
pip install -r requirements.txt
```

## Run Streamlit App

```bash
streamlit run app.py
```

---

# 📌 Future Scope

Future improvements that can be added:

* Deep Learning models
* Real-time mental health monitoring
* Sentiment analysis integration
* Mobile application deployment
* Personalized recommendations for users

---

# 📖 Conclusion

This project successfully demonstrated how Machine Learning can be used to analyze and predict the impact of social media on mental health.

Multiple classification and clustering algorithms were implemented and compared. Random Forest achieved the best overall performance and was deployed using Streamlit.

The project highlights the practical application of Machine Learning in mental health awareness and behavioral analysis.

---

# 👨‍💻 Contributors

* Utkarsh Sharma
* Team Members

---

# 📜 License

This project is created for academic and educational purp

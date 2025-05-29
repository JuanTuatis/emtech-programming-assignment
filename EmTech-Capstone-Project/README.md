# 📘 Lifestyle and Learning – Predicting Student Performance

**Emerging Technology Track | Capstone Project by AJ Dave Obis and Juan Francis Tuatis**  

***Video Presentation YouTube Lnk: https://youtu.be/r20fxU2oxPE📼***

##  Project Overview 🧠

This project investigates how students' lifestyle habits influence academic performance using a simulated dataset of 1,000 students. By analyzing screen time, study and sleep patterns, mental health, and other lifestyle variables, we explore how these factors relate to final exam scores.

The Researech Question:  
**Which type of screen time (Netflix vs. social media) is more harmful to student performance?**

## 🎯 Project Goals

- Identify key lifestyle factors affecting student exam scores.
- Use clustering to group students with similar habits.
- Build predictive models for academic performance.
- Deliver actionable insights through data storytelling.

## 🛠️ Methods and Workflow

### 🔍 1. Data Preparation
- Dataset: Sourced from Kaggle, 1,000 student records.
- Cleaned and encoded categorical variables (label/ordinal encoding).
- Added engineered features:
  - `total_screen_time`, `netflix_social_ratio`
  - `screen_study_ratio`, `screen_sleep_ratio`
- Standardized numeric features for training models.

### 📊 2. Exploratory Data Analysis (EDA)
- Histograms and scatter plots for lifestyle vs. exam score.
- Correlation heatmap revealed top factors:
  - `study_hours_per_day`, `screen_study_ratio`, `mental_health_rating`, `screen_sleep_ratio`

### 🧩 3. Clustering (Unsupervised Learning)
- Used K-Means and Silhouette Score to determine optimal clusters (K=6).
- Cluster profiles revealed distinct student lifestyles with varying academic outcomes.

### 📈 4. Regression Models (Supervised Learning)
Predicted final exam scores using:
- **Linear Regression**
  - R²: 0.90 | MAE: 4.23
- **Random Forest Regressor**
  - R²: 0.84 | MAE: 5.14
- **Decision Tree Regressor**
  - R²: 0.75 | MAE: 6.52

**Linear Regression performed best**, providing strong accuracy and interpretability.

### 🧠 5. Classification (Optional)
- Labeled scores into: `Low`, `Average`, `High`
- Models:
  - Logistic Regression (Accuracy: 86%)
  - Decision Tree Classifier (Accuracy: 74%)

## 📌 Key Findings

- ***Social media use is more harmful than Netflix to academic performance.***
- Top features: `study_hours_per_day`, `screen_study_ratio`, `mental_health_rating`
- Balanced habits (study, sleep, and attendance) mitigate the negative effects of screen time.
- **Clusters** exposed distinct profiles, such as:
  - High-performers: Study consistently, attend class, balanced screen time
  - Low-performers: Zero study hours, high screen usage

## 🔎 Visuals and Interpretations

- 📊 Correlation Heatmap
- 📉 Elbow & Silhouette Score for Clustering
- 🧠 Feature Importance (Random Forest vs Linear Regression)
- 🧮 Confusion Matrices for Classification Models

## 📚 Technologies Used

- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Scikit-learn (Regression, Classification, Clustering)
- Jupyter Notebook

## 🧾 Conclusion

This analysis reveals actionable insights for students and educators:
- Prioritize consistent study habits and sleep routines.
- Monitor and manage screen time, especially on social media.
- Encourage attendance and mental well-being for better performance.


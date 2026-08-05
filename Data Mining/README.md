# Healthcare Data Mining & Machine Learning Pipeline
A end-to-end data mining and machine learning workflow applied to a healthcare dataset using Python. This project covers comprehensive data preprocessing, exploratory data analysis (EDA), supervised classification via Decision Trees, and unsupervised clustering using K-Means.
# 📌 Project Overview
Healthcare datasets often contain complex, high-dimensional data that require systematic processing before predictive modeling can take place.
This repository demonstrates:
Data Preprocessing & Cleaning: Handling missing values, encoding categorical variables, and scaling feature sets.
Supervised Learning: Building and evaluating a Decision Tree Classifier to predict healthcare outcomes.Unsupervised Learning: Segmenting patient/healthcare data using K-Means Clustering.
Visualization: Visualizing feature distributions, cluster formations, and model decisions.
# 🛠️ Tech Stack & Libraries
Language: Python 3.x
Data Manipulation: pandas, numpy
Machine Learning: scikit-learn
Data Visualization: matplotlib, seaborn
# 📊 Workflow & Methodology
Data Ingestion ➔ Preprocessing & EDA ➔ Model Training (Supervised & Unsupervised) ➔ Evaluation & Visualization

1. Data Preprocessing & EDA
  Cleaned missing, null, or inconsistent records across dataset features.
  Applied feature scaling (StandardScaler / MinMaxScaler) to ensure parity across numerical attributes.
  Performed exploratory data analysis using distribution plots and correlation heatmaps to extract key data insights.

2. Supervised Learning: Decision Tree Classifier
   Split dataset into training and testing subsets ($80/20$ split).
   Trained a Decision Tree Classifier to categorize target health metrics/outcomes.
   Evaluated performance using key metrics: Accuracy, Precision, Recall, F1-Score, and Confusion Matrix.

   3. Unsupervised Learning: K-Means Clustering
      Utilized the Elbow Method (Sum of Squared Errors) to determine the optimal number of clusters ($K$).
      Trained a K-Means Model to discover underlying patterns and group similar patient profiles.
      Visualized cluster separations using 2D feature projection plots.

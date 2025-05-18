🧠 Adult Census Income Classification Using Machine Learning
This project uses supervised machine learning techniques to classify individuals' income brackets (above or below $50K/year) based on census data. The analysis includes full preprocessing, class balancing, training using XGBoost, and performance evaluation with visualizations.

📁 Project Structure
adult_income_ML_model.ipynb: Main notebook for data processing, training, and evaluation

README.md: Project documentation

adult.csv: Dataset file (must be downloaded from Kaggle)

📊 Dataset Overview
Dataset Name: Adult Census Income

Source: UCI via Kaggle

Description: Predict whether an individual earns more than $50K/year based on census features.

Target Variable: income

Values: <=50K, >50K

Key Features:

Age, Workclass, Education, Marital Status, Occupation, Relationship, Race, Sex, Capital Gain, Capital Loss, Hours per Week, Native Country

🧹 Data Preprocessing
Replaced ? with NaN and removed missing records

One-hot encoded categorical variables

Scaled numerical features using StandardScaler

Converted target labels to binary format (0 for <=50K, 1 for >50K)

⚖️ Class Imbalance Handling
Used SMOTEENN, a hybrid approach combining oversampling (SMOTE) and undersampling (Edited Nearest Neighbors), to handle class imbalance effectively.

🧠 Model: XGBoost Classifier
Model: XGBClassifier

Parameters:

n_estimators=100, learning_rate=0.1, max_depth=6

Data split: 80% train / 20% test

📈 Evaluation Metrics
Accuracy, Precision, Recall, F1-score

Confusion Matrix (visualized with heatmap)

ROC Curve and AUC Score

Feature Importance: Displayed in a vertical bar chart

📊 Visualizations
Target class distribution (before and after balancing)

ROC Curve

Confusion Matrix

Top feature importance (vertical bar plot with readable labels)


Download the dataset from Kaggle:
👉 https://www.kaggle.com/datasets/uciml/adult-census-income

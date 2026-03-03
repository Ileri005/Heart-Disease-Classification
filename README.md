# 🏥 Heart Disease Classification
> **Focus:** Evaluating Binary Classification Performance and Feature Importance in Clinical Diagnostics.

This project investigates the application of supervised machine learning to predict the presence of heart disease based on clinical parameters. The primary objective was to move beyond simple accuracy and focus on **model reliability** through comprehensive evaluation metrics like precision, recall, and F1-score.

## 🚀 The Challenge
In medical diagnostics, the cost of a "False Negative" (missing a sick patient) is much higher than a "False Positive." This project explores how to optimize a classification model to prioritize **Recall** while maintaining a robust **ROC-AUC** curve.

## 🛠️ Technical Implementation
* **Frameworks:** Scikit-learn, NumPy, Pandas, Matplotlib, Seaborn.
* **Models Tested:** Logistic Regression, K-Nearest Neighbors (KNN), and Random Forest.
* **Pipeline:** * Exploratory Data Analysis (EDA) to identify correlations between age, cholesterol, and heart rate.
    * Feature importance analysis to determine which clinical markers (e.g., `cp` - chest pain type) were the strongest predictors.
    * Hyperparameter tuning using **RandomizedSearchCV** and **GridSearchCV** to squeeze maximum performance from the models.

## 🎯 Results & Metrics
* **Model Performance:** Achieved a high-accuracy baseline with Random Forest, but fine-tuned **Logistic Regression** for better interpretability and clinical application.
* **Evaluation:** Utilized a confusion matrix to visualize error types and analyzed the ROC curve to determine the model's sensitivity vs. specificity.
* **Feature Importance:** Identified that 'Max Heart Rate' and 'Chest Pain Type' were the most significant features for predicting heart disease in this dataset.

## 📂 Project Workflow
1. **Data Exploration:** Visualizing age vs. heart rate distributions.
2. **Preprocessing:** Handling categorical variables and splitting data for training and testing.
3. **Model Fitting:** Training multiple classifiers to find the optimal baseline.
4. **Evaluation:** Detailed analysis using Cross-Validation to ensure the results aren't due to luck.

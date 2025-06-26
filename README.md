# Breast-Cancer-Detection
________________________________________
## Objective of the Analysis
The primary objective of this analysis is to predict whether a tumor is malignant or benign using patient diagnostic data. We aim to select a classification model that balances accuracy and interpretability, enabling healthcare professionals to make informed decisions quickly. The ultimate goal is to build a robust, trustworthy model that can be used in early detection efforts and assist oncologists in prioritizing medical intervention.
________________________________________
## Dataset Description
The dataset used is the Breast Cancer Wisconsin (Diagnostic) Data Set from Kaggle. It consists of 569 rows and 32 columns, including diagnostic information about cell nuclei from breast cancer biopsies.
Key features:
•	Target Variable: diagnosis (M for malignant, B for benign)
•	Feature Columns: 30 real-valued attributes such as radius, texture, perimeter, area, smoothness, compactness, concavity, etc.
•	ID Column: Dropped from analysis
•	Missing Values: One unnamed column with missing values was dropped
________________________________________
## Data Cleaning & Feature Engineering
•	Removed the unnamed column with missing values
•	Dropped the id column as it carries no predictive value
•	Encoded the target column diagnosis:
o	M → 1 (Malignant)
o	B → 0 (Benign)
•	Split data: 75% training, 25% test
•	Scaled features using StandardScaler
________________________________________
## Classifier Models & Performance Comparison
We trained three different classifiers:
a. **Logistic Regression (Baseline Model)**
•	Accuracy: 96.5%
•	Pros: Highly interpretable (feature coefficients), fast training
•	Cons: Assumes linear decision boundary
b. **Random Forest Classifier**
•	Accuracy: 94.4%
•	Pros: Handles feature interactions well, provides feature importance
•	Cons: Less interpretable than logistic regression
c. **Support Vector Machine (SVM)**
•	Accuracy: 94.4%
•	Pros: High accuracy, especially in high-dimensional space
•	Cons: Limited interpretability, more computationally expensive
Evaluation Metric Used: Accuracy and confusion matrix (true positives vs false positives)




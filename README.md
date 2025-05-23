# Graduate Admission Predictions
## Project Overview
This project builds a machine learning model to predict the chances of admission to graduate programs based on various student academic metrics. It follows a complete data science workflow from data exploration to making predictions.

## Technology Stack Used
Programming Language: Python
Libraries:
pandas: For data manipulation and analysis
numpy: For numerical operations
matplotlib: For data visualization
scikit-learn: For machine learning model development

## Process and Methodology
1. Data Acquisition and Exploration
Loaded the dataset (admission_predict.csv) with 500 student profiles
Explored basic dataset information (shape, data types, statistical summary)
Confirmed dataset has 500 rows with 9 columns and no missing values
2. Data Preprocessing
Renamed columns for better readability (e.g., 'GRE Score' → 'GRE')
Removed unnecessary columns (Serial No.)
Created a copy of the dataframe and replaced zeros with NaN values where appropriate
3. Data Visualization
Created histograms for each feature:
GRE scores
TOEFL scores
University Rating
SOP (Statement of Purpose) ratings
LOR (Letter of Recommendation) ratings
CGPA values
Research experience
4. Model Development
Split data into features (X) and target variable (y)
Used GridSearchCV to compare 6 different regression algorithms:
Linear Regression
Lasso Regression
Support Vector Regression (SVR)
Decision Tree Regression
Random Forest Regression
K-Nearest Neighbors (KNN)
Found Linear Regression performed best (81% accuracy with cross-validation)
Split data into training (80%) and testing (20%) sets
Built and trained the final Linear Regression model
Evaluated model on test data (achieved 82.1% accuracy)
5. Making Predictions
Used the trained model to predict admission chances for sample student profiles
Example predictions:
Student with strong profile: 92.855% chance of admission
Student with average profile: 73.627% chance of admission

## Machine Learning Concepts Used

Supervised Learning (Regression)
Model Selection and Hyperparameter Tuning
Cross-validation (5-fold)
Train-test splitting
Model evaluation metrics
Feature importance analysis (implicit in linear regression)
This project follows standard machine learning practices and successfully demonstrates how to build a regression model for educational predictions with good accuracy.

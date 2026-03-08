# Diabetes Prediction using SVM

<a href="https://colab.research.google.com/github/AbderraoufBelaiouar/Diabetes_Prediction_usnig_svm/blob/main/Project_3_Diabetes_Prediction.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>

This project implements a Support Vector Machine (SVM) classifier to predict diabetes using the PIMA Diabetes Dataset. It covers data preprocessing, model training, evaluation, and a predictive system for individual patient data.

## Dataset

The PIMA Diabetes Dataset is used, which contains diagnostic measurements from female patients of Pima Indian heritage. The dataset includes features such as:

- Pregnancies
- Glucose
- BloodPressure
- SkinThickness
- Insulin
- BMI
- DiabetesPedigreeFunction
- Age
- Outcome (0: Non-Diabetic, 1: Diabetic)

## Preprocessing

- Data is loaded from a CSV file.
- Statistical analysis and value counts are performed.
- Features are separated from the target variable.
- Data is standardized using `StandardScaler` to normalize the features.

## Model

A Support Vector Classifier (`SVC`) with a linear kernel is used for binary classification.

## Training and Evaluation

- The dataset is split into training and testing sets (80% train, 20% test) with stratification.
- The SVM model is trained on the standardized training data.
- Accuracy is evaluated on both training and test sets.
- The model achieves high accuracy in predicting diabetes status.

## Predictive System

A sample input data is provided to demonstrate prediction for a single patient. The system standardizes the input and outputs whether the person is diabetic or not.

## Requirements

- Python 3
- Libraries: `numpy`, `pandas`, `scikit-learn`

## Usage

1. Ensure the required libraries are installed.
2. Load the dataset (update the file path if necessary).
3. Run the notebook cells sequentially.
4. View the accuracy scores and test the predictive system.

## Notes

This is a baseline implementation for educational purposes. Further improvements could include hyperparameter tuning, cross-validation, and additional evaluation metrics like precision, recall, and F1-score.
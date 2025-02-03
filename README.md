# Diabetes Prediction using Machine Learning

## Overview

This project implements a machine learning model to predict diabetes based on various health parameters. The dataset used for this project is the **Pima Indians Diabetes Dataset**.

## Dependencies

Ensure you have the following libraries installed before running the script:

```bash
pip install numpy pandas scikit-learn
```

## Dataset

The dataset consists of 768 samples with 8 health-related features and an outcome variable:

- **Pregnancies**: Number of pregnancies
- **Glucose**: Plasma glucose concentration
- **BloodPressure**: Diastolic blood pressure (mm Hg)
- **SkinThickness**: Triceps skinfold thickness (mm)
- **Insulin**: 2-Hour serum insulin (mu U/ml)
- **BMI**: Body mass index (weight in kg/height in m^2)
- **DiabetesPedigreeFunction**: Diabetes pedigree function (family history influence)
- **Age**: Age of the person
- **Outcome**: (0 - Non-Diabetic, 1 - Diabetic)

## Steps in Implementation

### 1. Data Preprocessing

- Load the dataset into a Pandas DataFrame.
- Display the first few rows for initial inspection.
- Check the shape of the dataset.
- Get statistical insights using `.describe()`.
- Separate the features (`X`) and target variable (`y`).

### 2. Standardization

- Standardize the feature set using `StandardScaler` to normalize the data for better model performance.

### 3. Train-Test Split

- Split the dataset into **training (80%)** and **testing (20%)** sets while maintaining class distribution (`stratify=y`).

### 4. Model Training

- Train a **Support Vector Machine (SVM) classifier** with a linear kernel on the training dataset.

### 5. Model Evaluation

- Compute accuracy scores for both training and test sets.
- Training Accuracy: **78.66%**
- Testing Accuracy: **77.27%**

### 6. Prediction System

- Take a sample input and standardize it.
- Use the trained SVM model to predict diabetes status.
- Output the result: `Diabetic` or `Non-Diabetic`.

## How to Use

1. **Run the script** in a Jupyter Notebook or Google Colab.
2. **Modify the input data** in the prediction section to test different cases.
3. **Train with different classifiers** (e.g., Decision Trees, Random Forest, etc.) to compare performance.

## Future Enhancements

- Implement deep learning models for improved accuracy.
- Add more health parameters for better predictions.
- Deploy as a web-based application.

## Acknowledgments

This project is inspired by the Pima Indians Diabetes dataset and serves as an introductory exploration of machine learning in healthcare analytics.

## License

This project is open-source and available for educational purposes. Modify and improve it as needed!

---

Thank you for exploring this project! 🚀


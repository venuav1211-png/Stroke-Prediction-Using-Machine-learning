# Stroke-Prediction-Using-Machine-learning

## 1. Project Overview

The **Stroke Prediction Using Machine Learning** project aims to predict whether a person belongs to the stroke or no-stroke class based on selected health and demographic information.

This project uses machine learning classification algorithms to analyze patient-related data and make predictions.

A Gradio web interface is developed to allow users to enter patient information and view the model's prediction.

**Note:** This project is developed for educational purposes only. It is not a medical diagnostic tool and should not be used for clinical decisions.

## 2. Problem Statement

Stroke is a serious health condition that can affect a person's quality of life. Identifying patterns in health-related data using machine learning can help demonstrate how predictive models classify individuals based on different features.

The objective of this project is to build a machine learning classification model that predicts the stroke class using patient information.

## 3. Dataset Information

- **Dataset Name:** Stroke Prediction Dataset
- **Dataset Source:** Kaggle
- **Dataset Link:** https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset
- **Dataset File:** `healthcare-dataset-stroke-data.csv`
- **Target Variable:** `stroke`

The target variable contains two classes:

- `0` – No Stroke
- `1` – Stroke

### Features Used

| Feature | Description |
|---|---|
| gender | Gender of the individual |
| age | Age of the individual |
| hypertension | Whether the individual has hypertension |
| heart_disease | Whether the individual has heart disease |
| ever_married | Marital status |
| work_type | Type of employment |
| Residence_type | Urban or Rural residence |
| avg_glucose_level | Average glucose level |
| bmi | Body Mass Index |
| smoking_status | Smoking information |

## 4. Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib
- Gradio

## 5. Project Workflow

The project follows these six stages:

### Stage 1: Business Understanding and Problem Statement
- Understand the business problem.
- Define the project objective.
- Identify the target variable.

### Stage 2: Data Loading, Preprocessing, and EDA
- Load the dataset.
- Explore the dataset.
- Handle missing values.
- Remove unnecessary columns and duplicate records.
- Perform exploratory data analysis.
- Visualize important features.

### Stage 3: Feature Selection and Train-Test Split
- Separate input features and target variable.
- Select relevant features.
- Split the dataset into training and testing sets.

### Stage 4: Model Building, Evaluation, and Selection
- Build classification models.
- Train the models.
- Evaluate model performance.
- Compare evaluation metrics.
- Select a suitable model.

### Stage 5: Model Saving and Gradio Deployment
- Save the trained machine learning pipeline using Joblib.
- Load the saved model.
- Develop an interactive Gradio interface.
- Connect user inputs to the prediction function.

### Stage 6: Testing the Deployed Application
- Enter patient information.
- Click the Predict button.
- Display the predicted class.
- Display the model's stroke-class score.
- Test different input combinations.

## 6. Machine Learning Algorithms

The following classification algorithms are considered in this project:

1. Logistic Regression
2. Decision Tree Classifier
3. Random Forest Classifier

The models are evaluated using classification metrics such as:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion Matrix

Since the dataset contains imbalanced target classes, accuracy alone is not sufficient to evaluate model performance.

## 7. Project Folder Structure

Organize your project files as follows:

```text
Stroke-Prediction-Project/
│
├── healthcare-dataset-stroke-data.csv
│
├── Stroke_Prediction.ipynb
│
├── stroke_prediction_model.pkl
│
└── README.md
```

**Note:** The saved model file is generated after model training. Use your actual notebook filename if it is different.

## 8. Installation and Requirements

Install the required Python libraries in Jupyter Notebook:

```python
%pip install pandas numpy matplotlib seaborn scikit-learn joblib gradio
```

## 9. How to Run the Project

Follow these steps to execute the project:

**Step 1:** Download the dataset from Kaggle.

**Step 2:** Place `healthcare-dataset-stroke-data.csv` in your project folder.

**Step 3:** Open Jupyter Notebook.

**Step 4:** Open `Stroke_Prediction.ipynb`.

**Step 5:** Execute the notebook cells sequentially, from data loading through model training and evaluation.

**Step 6:** Save the trained model as:

```text
stroke_prediction_model.pkl
```

**Step 7:** Run the Gradio deployment cell in the same notebook.

**Step 8:** Open the local URL displayed by Gradio in your browser.

**Step 9:** Enter the required information and click **Predict** to view the result.

## 10. Gradio Web Application

The project uses Gradio to create an interactive web application.

Users can enter:

- Gender
- Age
- Hypertension
- Heart Disease
- Marital Status
- Work Type
- Residence Type
- Smoking Status
- Average Glucose Level
- BMI

After clicking the Predict button, the application displays:

- Predicted class: Stroke or No Stroke
- Model score for the stroke class

The application runs directly from the Jupyter Notebook without requiring a separate `app.py` file.

## 11. Expected Output

The application displays one of the following prediction classes:

- **Stroke class predicted**
- **No-stroke class predicted**

It also displays the model's estimated probability for the stroke class.

Actual predictions and model performance depend on the trained model and the input values.

## 12. Limitations

- The dataset contains imbalanced target classes.
- Model predictions depend on the quality of the training data.
- Prediction results may contain false positives and false negatives.
- The model is not clinically validated.
- The displayed probability is not an individual's medically established stroke risk.

## 13. Future Enhancements

- Improve model performance using suitable class-imbalance techniques.
- Perform hyperparameter tuning.
- Evaluate different classification algorithms.
- Improve the Gradio interface.
- Deploy the application to a cloud hosting platform.
- Perform additional validation using appropriate datasets.

## 14. Conclusion

This project demonstrates an end-to-end machine learning workflow using Python. It covers data preprocessing, exploratory data analysis, feature selection, model building, model evaluation, model saving, and Gradio deployment.

The project provides practical experience in developing and deploying a classification model through an interactive web application.

---

**Project Title:** Stroke Prediction Using Machine Learning

**Implementation:** Python – Jupyter Notebook

**Deployment:** Gradio Web Application

**Project Type:** Machine Learning – Classification

**Disclaimer:** This application is intended only for educational and learning purposes. It is not a substitute for professional medical advice, diagnosis, or treatment.

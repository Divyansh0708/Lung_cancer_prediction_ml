# Lung_cancer_prediction_ml
# LungCare AI – Lung Cancer Prediction Using Machine Learning

**An Intelligent Machine Learning-Based Lung Cancer Prediction System**

LungCare AI is a machine learning project designed to predict the likelihood of lung cancer based on health, lifestyle, and symptom-related survey information. The project uses a **Random Forest Classification Algorithm** to analyze input features and generate predictions.

The project also includes an interactive web dashboard developed using Streamlit, allowing users to explore model performance, analyze feature importance, generate predictions, and view prediction history.

> **Disclaimer:** This project is developed for academic and educational purposes only. It is not a medical diagnostic tool and must not be used as a substitute for professional medical advice.

---

## Project Overview

Lung cancer is one of the major health concerns worldwide. Early awareness of potential risk factors can play an important role in encouraging timely medical consultation.

This project demonstrates how Machine Learning can be applied to healthcare-related survey data to classify whether an input belongs to the YES or NO lung cancer category.

The system takes various patient-related inputs, processes them through a trained Random Forest model, and displays the predicted classification along with model-estimated probabilities.

## Project Objectives

- Develop a machine learning model for lung cancer classification.
- Analyze health and lifestyle-related factors.
- Perform predictions using a trained Random Forest model.
- Evaluate model performance using standard classification metrics.
- Develop an interactive Streamlit dashboard.
- Visualize model performance and feature importance.
- Maintain prediction history within the application session.

## Dataset Information

**Dataset:** Survey Lung Cancer Dataset

The dataset contains survey-based information related to individuals' health conditions, symptoms, and lifestyle habits.

| Dataset Information | Details |
|---|---|
| Total Records | 309 |
| Input Features | 15 |
| Target Variable | LUNG_CANCER |
| Problem Type | Binary Classification |
| Dataset Format | CSV |

### Input Features

1. Gender
2. Age
3. Smoking
4. Yellow Fingers
5. Anxiety
6. Peer Pressure
7. Chronic Disease
8. Fatigue
9. Allergy
10. Wheezing
11. Alcohol Consuming
12. Coughing
13. Shortness of Breath
14. Swallowing Difficulty
15. Chest Pain

**Target Variable:** `LUNG_CANCER`

- YES – Positive class
- NO – Negative class

## Machine Learning Algorithm

This project uses the **Random Forest Classifier**.

Random Forest is a supervised machine learning algorithm that combines multiple decision trees to generate a final prediction.

### Why Random Forest?

- Handles classification problems effectively.
- Combines multiple decision trees.
- Can capture complex relationships between features.
- Provides feature importance scores.
- Supports probability-based predictions.

## Model Performance

The trained Random Forest model achieved the following evaluation results:

| Evaluation Metric | Score |
|---|---:|
| Accuracy | 91.10% |
| Precision | 93.90% |
| Recall | 95.80% |
| F1 Score | 94.80% |
| Cross-Validation F1 | 93.80% |
| Cross-Validation Recall | 95.80% |

*These are the evaluation metrics recorded in the project's model metadata.*

## Technologies Used

| Technology | Purpose |
|---|---|
| Python | Programming Language |
| Pandas | Data Manipulation |
| NumPy | Numerical Operations |
| Scikit-learn | Machine Learning |
| Joblib | Model Serialization |
| Streamlit | Web Application |
| JSON | Model Metadata Storage |
| Matplotlib | Data Visualization |

## Application Features

### 1. Model Insights
- Displays model performance metrics.
- Visualizes Accuracy, Precision, Recall, and F1 Score.
- Shows dataset and model information.
- Displays input feature information.
- Provides feature importance analysis.
- Explains the machine learning workflow.

### 2. Prediction Studio
- Accepts gender and age as inputs.
- Collects health and lifestyle information.
- Generates predictions using the trained model.
- Displays YES and NO model probabilities.
- Provides a prediction explanation.

### 3. Prediction History
- Stores predictions during the current application session.
- Displays previous prediction records.
- Shows total YES and NO predictions.
- Allows users to download prediction history as a CSV file.
- Provides an option to clear prediction history.

## Project Structure

```text
machine_learning_pbl/
│
├── app.py
│
├── predict.py
│
├── test_model.py
│
├── survey_lungcancer.csv
│
├── lung_cancer_model.joblib
│
├── model_metadata.json
│
└── README.md
```

### File Description

- `app.py` – Main Streamlit web application.
- `predict.py` – Script for generating predictions using the trained model.
- `test_model.py` – Script for testing the saved model.
- `survey_lungcancer.csv` – Dataset used in the project.
- `lung_cancer_model.joblib` – Saved trained Random Forest model.
- `model_metadata.json` – Contains feature order, encoding information, and model evaluation metrics.
- `README.md` – Project documentation.

## Installation and Setup

Follow these steps to run the project locally.

### Step 1: Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
```

### Step 2: Navigate to the Project Directory

```bash
cd machine_learning_pbl
```

### Step 3: Install Required Libraries

```bash
pip install pandas numpy scikit-learn streamlit joblib
```

### Step 4: Run the Streamlit Application

```bash
streamlit run app.py
```

### Step 5: Open the Application

After running the command, Streamlit will provide a local URL.

Open the URL in your browser to access the LungCare AI dashboard.

## How the System Works

1. Dataset is loaded into the machine learning environment.
2. Health and lifestyle features are used as model inputs.
3. A trained Random Forest model is loaded using Joblib.
4. Users enter their information through the Streamlit interface.
5. The model processes the input features.
6. The application generates a YES or NO classification.
7. Model-estimated class probabilities and prediction history are displayed.

## Future Enhancements

- Integration with larger and more diverse datasets.
- Further model validation and performance comparison.
- Improved explainable AI techniques.
- Additional machine learning algorithms.
- Secure database integration for prediction history.
- Enhanced user interface and accessibility.
- Clinical validation before any real-world healthcare application.

## Project Information

**Project Title:** Lung Cancer Prediction Using Machine Learning

**Project Domain:** Artificial Intelligence & Machine Learning

**Algorithm:** Random Forest Classifier

**Application:** LungCare AI

**Project Type:** Academic Machine Learning Project

---


**Made with Python, Machine Learning & Streamlit.**

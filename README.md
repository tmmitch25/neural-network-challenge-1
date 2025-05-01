# Student Loan Repayment Prediction - Neural Network Model

## Overview

As part of my work at a company specializing in student loan refinancing, I was tasked with developing a machine learning model to predict whether student loan borrowers are likely to repay their loans. This model aims to help the business more accurately assess borrower risk and tailor interest rates accordingly.

Using a dataset of historical loan recipient data — including academic performance, financial metrics, and credit indicators — I built a deep neural network using TensorFlow and Keras to classify creditworthiness.

---

## Files Included

- `student_loans_with_deep_learning.ipynb`: My final Jupyter notebook with all code, preprocessing, model training, and evaluation.
- `student_loans.keras`: The saved Keras model file trained on the dataset.

---

## Technologies Used

- Python
- Pandas
- scikit-learn
- TensorFlow / Keras
- Google Colab
- Git & GitHub

---

## Project Workflow

### 🔹 Part 1: Data Preparation
- Loaded the dataset from the provided URL using Pandas.
- Defined the target variable `credit_ranking`.
- Created feature and target datasets (`X` and `y`).
- Performed a train/test split.
- Scaled the features using `StandardScaler`.

### 🔹 Part 2: Neural Network Model
- Built a deep neural network with two hidden layers using TensorFlow’s Keras API.
- First layer: 6 neurons, ReLU activation.
- Second layer: 3 neurons, ReLU activation.
- Output layer: 1 neuron, Sigmoid activation for binary classification.
- Compiled with `binary_crossentropy` loss and the `adam` optimizer.
- Trained over 100 epochs and evaluated accuracy and loss on test data.
- Saved the final trained model to `student_loans.keras`.

### 🔹 Part 3: Prediction
- Reloaded the saved model.
- Generated binary predictions on the test dataset.
- Evaluated the predictions using a classification report.

### 🔹 Part 4: Recommendation System Discussion
- Discussed the data required for building a recommendation system for student loans.
- Justified the use of a **content-based filtering** approach.
- Identified two major real-world challenges:
  - Ensuring data privacy and security
  - Avoiding bias in recommendations

---

## Key Results

- Successfully built a binary classification model to predict loan repayment likelihood.
- Achieved reasonable model accuracy and loss metrics using a lightweight neural network architecture.
- Outlined future potential for extending this work into a recommendation system.


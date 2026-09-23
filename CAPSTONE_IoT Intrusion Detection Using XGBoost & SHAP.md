# IoT Intrusion Detection Using XGBoost & SHAP

## Project Overview

This project focuses on developing a **machine learning-based Intrusion Detection System (IDS) for IoT networks** using the **UNSW-NB15 cybersecurity dataset**. The goal is to identify whether network traffic is **Normal or an Attack**, helping detect potentially malicious activity in IoT environments.

The project implements an end-to-end machine learning workflow, including **data preprocessing, categorical encoding, missing-value handling, outlier treatment, feature selection, model training, evaluation, and Explainable AI (XAI)**. An **XGBoost Classifier** is used as the primary machine learning model because of its ability to handle complex relationships within network traffic data and provide strong classification performance.

To improve interpretability, **SHAP (SHapley Additive exPlanations)** is incorporated to identify and visualize the features that contribute most to the model's predictions. The project also includes a simulated **real-time IoT intrusion detection system**, where network samples are classified as Normal or Attack for different simulated IoT devices.

## Key Features

* Preprocessed the **UNSW-NB15 network intrusion dataset**
* Handled missing and infinite values using appropriate data-cleaning techniques
* Encoded categorical network features using **Ordinal Encoding**
* Applied **outlier clipping** to reduce the impact of extreme values
* Performed **feature selection using XGBoost feature importance**
* Built an **XGBoost binary classification model**
* Compared baseline and optimized XGBoost configurations
* Evaluated performance using:

  * Accuracy
  * Precision
  * Recall
  * F1-score
  * Confusion Matrix
* Used **SHAP** for model interpretability and feature importance analysis
* Simulated real-time intrusion detection for multiple IoT devices
* Visualized the distribution of different attack categories

## Model Performance

The developed model achieved approximately **90.09% testing accuracy** on the UNSW-NB15 testing dataset.

| Metric    | Normal | Attack |
| --------- | -----: | -----: |
| Precision |   0.77 |   0.99 |
| Recall    |   0.98 |   0.86 |
| F1-Score  |   0.86 |   0.92 |

**Overall Testing Accuracy: 90.09%**

The model demonstrates strong detection capability, particularly in identifying attack traffic, while maintaining high recall for normal network traffic.

## Technologies & Tools

* **Python**
* **Pandas**
* **NumPy**
* **Scikit-learn**
* **XGBoost**
* **SHAP**
* **Matplotlib**
* **Seaborn**
* **Google Colab**
* **UNSW-NB15 Dataset**

## Machine Learning Workflow

UNSW-NB15 Dataset
        ↓
Data Cleaning
        ↓
Missing & Infinite Value Handling
        ↓
Categorical Feature Encoding
        ↓
Outlier Clipping
        ↓
XGBoost-Based Feature Selection
        ↓
XGBoost Classification
        ↓
Model Evaluation
        ↓
SHAP Explainability
        ↓
IoT Intrusion Detection Simulation


## Explainable AI

SHAP was used to make the XGBoost model more interpretable by analyzing how individual features influence the model's predictions.

This helps move beyond simply predicting **Normal/Attack** and provides insight into **which network characteristics contribute to the prediction**, which is particularly useful for cybersecurity applications where model transparency is important.

## Real-Time IoT Detection Simulation

The project includes a simulated real-time detection component representing different IoT devices such as:

* Temperature Sensor
* Smart Light
* Smart Camera
* Wearable Device
* IoT Gateway

For each simulated network sample, the trained model predicts whether the traffic is **Normal** or represents an **Attack**.

## Project Outcome

This project demonstrates the application of **machine learning, data preprocessing, feature engineering, classification, model evaluation, and Explainable AI** to a real-world cybersecurity problem.

It provides practical experience in building an end-to-end **IoT intrusion detection pipeline** and demonstrates how machine learning can be combined with model interpretability techniques such as SHAP to support cybersecurity analysis and decision-making.

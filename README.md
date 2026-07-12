# Network Anomaly Detection using Machine Learning

## Project Overview
This project demonstrates a comprehensive approach to detecting network anomalies and enhancing cybersecurity postures using Machine Learning. By utilizing a benchmark dataset, the project covers the full pipeline—from data acquisition and rigorous preprocessing to model training, evaluation, and persistence. The ultimate goal is to robustly classify network traffic as either "normal" or identify it as one of several "attack" categories (e.g., DoS, Probe, Privilege, Access).

## Tools Used
- Python
- Jupyter Notebook
- Git

## Tech Stack Used
- Machine Learning (Classification)
- Cybersecurity Threat Detection
- Data Engineering & Exploratory Data Analysis (EDA)

## Libraries Used
- **Pandas & NumPy**: For extensive data manipulation, structuring, and numerical analysis.
- **Scikit-Learn**: For dataset splitting (`train_test_split`), building the machine learning model (`RandomForestClassifier`), and calculating comprehensive evaluation metrics (`accuracy_score`, `precision_score`, `recall_score`, `f1_score`, `confusion_matrix`, `classification_report`).
- **Seaborn & Matplotlib**: For generating rich data visualizations, such as confusion matrices, to intuitively assess model performance.
- **Python Standard Libraries (`requests`, `zipfile`, `io`)**: For seamless, programmatic downloading and extraction of datasets directly from external sources.

## Techniques Used

### Data Acquisition & Preprocessing
- **Target Variable Definition**: Creation of complex targets including a binary classification flag (normal vs. attack) and a multi-class mapping to categorize specific threats (Normal, DoS, Probe, Privilege, Access).
- **Categorical Feature Encoding**: Conversion of categorical string data (e.g., protocols and services) into numerical formats using One-Hot Encoding (`pd.get_dummies`), a critical prerequisite for robust algorithm training.
- **Feature Selection**: Strategic aggregation of numeric and newly encoded categorical features into a cohesive training set.
- **Data Splitting Strategy**: Multi-tiered partitioning of the dataset into training, validation, and test subsets to guarantee unbiased model evaluation and prevent data leakage.

### Model Development & Evaluation
- **Model Training (Random Forest)**: Implementation of an ensemble learning method (Random Forest Classifier) chosen for its robustness, resistance to overfitting, and exceptional capability to handle high-dimensional network data.
- **Comprehensive Evaluation**: Extracting detailed metrics beyond standard accuracy—such as precision, recall, and F1-scores per class—paired with visualizations (Confusion Matrices) to diagnose specific misclassifications and assess performance across distinct anomaly types.

## Dataset Used
This project leverages the **NSL-KDD dataset**, a widely recognized benchmark for network intrusion detection. The dataset was obtained via the HackTheBox platform.

**Author:** Engr. Hammad Khurshid

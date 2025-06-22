# Tumor-Detection-project
🧠 Tumor Detection Using Machine Learning
📌 Project Overview
This project focuses on detecting the presence of a tumor (malignant or benign) using machine learning classification techniques. The primary objective is to build a model that accurately classifies tumors based on various medical features.

🧠 Problem Statement
Accurate early detection of tumors is critical for effective treatment. This project aims to develop a machine learning model using a labeled dataset of tumor characteristics to classify tumors as **benign (non-cancerous)** or **malignant (cancerous)**.
📁 Dataset
- **Target Variable**: `diagnosis`  
  - `M`: Malignant  
  - `B`: Benign
- **Features** (examples):
  - Radius, Texture, Perimeter, Area, Smoothness, etc. (mean, worst, and standard error measurements)

🔍 Methodology & Analysis Process
1. Data Preprocessing
- **Data Cleaning**:
  - Removed irrelevant columns (e.g., ID).
  - Converted diagnosis labels (`M`, `B`) into binary numeric values (1 and 0).
- **Data Normalization**:
  - Scaled features using standardization for better model performance.
- **Data Splitting**:
  - Split into training and testing sets (typically 80% train, 20% test).

2. Exploratory Data Analysis (EDA)
- **Class Distribution**:
  - Checked balance of benign vs. malignant cases.
- **Visualization**:
  - Used heatmaps and pairplots to observe feature correlations.
  - Identified top features impacting tumor classification.

3. Model Building
Implemented multiple classification models:
- Logistic Regression
- Support Vector Machine (SVM)
- Random Forest Classifier
- K-Nearest Neighbors (KNN)

4. Model Evaluation
- Evaluated models using:
  - **Accuracy**
  - **Confusion Matrix**
  - **Precision, Recall, F1-score**
  - ROC Curve & AUC (where applicable)

🧠 Key Findings
- **Random Forest Classifier** and **SVM** showed high classification accuracy and robust performance.
- Features like **radius_mean**, **texture_mean**, and **area_mean** had the highest impact on predictions.
- The dataset was slightly imbalanced, but performance remained stable across all models.
- With proper preprocessing and feature selection, machine learning can accurately assist in tumor detection and medical diagnosis.

🛠️ Technologies Used
- Python 3.x
- Jupyter Notebook
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn (classification, metrics)

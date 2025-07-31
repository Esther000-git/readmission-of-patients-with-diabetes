# Diabetes Readmission Prediction

This project analyzes the readmission of diabetic patients using predictive modeling techniques in Python. It is based on the **"Diabetes 130-US Hospitals for Years 1999-2008"** dataset, which includes 10 years of clinical care data across 130 hospitals and healthcare networks in the United States.

Each row in the dataset represents a patient encounter and contains 47 attributes with a total of **101,766 instances**. The primary goal is to predict patient readmission based on available clinical and demographic information.

---

## 📌 Objective

- Use Python and machine learning libraries such as **NumPy**, **Pandas**, and **Scikit-learn** to build predictive models.
- Evaluate model performance using the **Area Under the ROC Curve (AUC ROC)**.
- Apply **10-fold Cross Validation (10-CV)** to estimate model generalization.
- Predict the target variable `readmitted`, which includes 3 classes:  
  - `NO` (not readmitted)  
  - `<30` (readmitted in less than 30 days)  
  - `>30` (readmitted after more than 30 days)

---

## 🔬 Workflow Overview

1. **Exploratory Data Analysis**  
   - Identify missing values, variable types (numeric/categorical), and data distribution.
   - Evaluate class imbalance in the `readmitted` variable.
  
2. **Baseline Classifier**  
   - Use `sklearn.dummy.DummyClassifier` as a reference point to measure AUC.
  
3. **Model Selection & Hyperparameter Tuning**  
   - Train various classifiers and manually adjust hyperparameters.
   - Compare models based on AUC ROC scores.

4. **Feature Selection**  
   - Explore automated attribute selection methods.
  
5. **Statistical Comparison**  
   - Compare model performance using:
     - Arithmetic mean of AUCs
     - **Wilcoxon signed-rank test** for hypothesis testing
  
6. **Scalability Considerations**  
   - Address processing time due to the large size of the dataset.

---

## 🤝 Collaborators

This project was developed in collaboration with a classmate as part of a coursework assignment.

---

## 🔗 Google Colab Link

You can run and explore the notebook using the following link:  
👉 [Open in Google Colab]((https://colab.research.google.com/drive/1XjVEEZkiSToYtUdpDl_-NhkPkMNykomu?usp=drive_link)

---

## 📂 Dataset

- **Name**: Diabetes 130-US hospitals for years 1999–2008
- **Source**: UCI Machine Learning Repository  
  https://archive.ics.uci.edu/ml/datasets/diabetes+130-us+hospitals+for+years+1999-2008

---

## 🛠️ Technologies Used

- Python 3
- NumPy
- Pandas
- Scikit-learn
- Matplotlib / Seaborn (for visualizations)

---

## 📈 Example Outputs

- AUC ROC comparison plots
- Confusion matrices for different models
- Summary of Wilcoxon test results

---

## 📑 License

Academic project developed during the Bachelor's Degree in Biomedical Engineering.
Subject: Clinical data analysis



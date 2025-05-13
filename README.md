# 🧠 Parkinson's Disease Detection using Machine Learning

This project focuses on building a predictive machine learning model to detect **Parkinson's Disease** using biomedical voice measurements. Parkinson's is a progressive disorder of the nervous system that affects movement. Early and accurate detection can significantly improve treatment outcomes and quality of life.

---

## 📌 Table of Contents

- [Introduction](#introduction)
- [Project Insights](#project-insights)
- [Technologies Used](#technologies-used)
- [How to Run](#how-to-run)
- [Results](#results)
- [Conclusion](#conclusion)
- [References](#references)

---

## 🧬 Introduction

Parkinson’s Disease (PD) affects millions globally, primarily in the elderly population. A significant early symptom of Parkinson’s is a change in voice. Researchers have identified specific voice metrics such as jitter, shimmer, and pitch variation that differ in Parkinson’s patients compared to healthy individuals.

In this project, we use a publicly available dataset containing biomedical voice measurements to train a classification model that can predict the presence of Parkinson's disease. The goal is to support healthcare providers with a non-invasive, fast, and inexpensive tool to assist early diagnosis.

---

## 📊 Project Insights

### ✅ Dataset Overview
- **Source**: UCI Machine Learning Repository
- **Instances**: 195
- **Features**: 22 voice-related features such as MDVP jitter, shimmer, HNR, DFA, spread1/spread2, PPE
- **Target**: `status` (0 = healthy, 1 = Parkinson’s disease)

### ✅ Steps Performed
1. **Data Preprocessing**
   - Checked for null values
   - Removed unnecessary columns like `name`
   - Feature scaling using MinMaxScaler

2. **Exploratory Data Analysis**
   - Correlation matrix
   - Count plots of target variable
   - Pairplots of important features

3. **Model Building**
   - Split data into training and test sets
   - Used `Logistic Regression` as the baseline model
   - Achieved **95.57%** test accuracy

4. **Evaluation**
   - Confusion matrix
   - Classification report
   - ROC-AUC score

---

## 🛠️ Technologies Used

- Python 3
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 🧪 How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/parkinsons-disease-detection.git
   cd parkinsons-disease-detection
# 📈 Results
Test Accuracy: 95.57%

Precision: 100%

Recall: 91%

F1-Score: 95%

ROC AUC Score: 0.978

This model demonstrates excellent classification ability on the voice data and can act as a supportive screening tool in medical diagnosis.

# 🧾 Conclusion
This project showcases how machine learning, even with simple models like Logistic Regression, can provide strong diagnostic support for neurological diseases such as Parkinson’s. Voice data is non-invasive and easy to collect, making this method both cost-effective and scalable.

In future iterations, more complex models (like SVM, XGBoost, or Neural Networks) and larger datasets can be used for even better results. Deployment as a mobile or web-based diagnostic aid can also be explored.

# 📚 References
UCI Parkinson's Dataset

Little MA, McSharry PE, Roberts SJ, Costello DA, Moroz IM. "Exploiting Nonlinear Recurrence and Fractal Scaling Properties for Voice Disorder Detection". BioMedical Engineering OnLine. 2007.

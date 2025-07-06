# 🎓 Predicting Student Performance Using Machine Learning

## 📌 Overview

This project is a capstone submission for **CACIITG Summer Analytics 2025**, aimed at applying machine learning to predict whether a student will pass or fail based on academic and demographic data. It uses supervised learning models and demonstrates real-world applications of classification algorithms in the education sector.

---

## 🛠 Tech Stack

- **Programming Language**: Python
- **Data Analysis**: Pandas, NumPy
- **Data Visualization**: Matplotlib, Seaborn
- **Machine Learning Models**: Logistic Regression, Random Forest, SVM
- **Preprocessing**: Scikit-learn (LabelEncoder, StandardScaler)
- **Notebook Environment**: Jupyter Notebook / Google Colab

---

## 🧱 Project Architecture (Mermaid Diagram)

```mermaid
graph TD
    A[Raw Dataset (CSV)] --> B[Data Preprocessing]
    B --> C[Feature Engineering]
    C --> D[Train/Test Split]
    D --> E[Model Training]
    E --> F[Model Evaluation]
    F --> G[Final Model Selection]
    G --> H[Results & Insights]
```

---

## 🔍 Workflow & Architecture Details

1. **Data Loading**: The dataset is loaded from a CSV file containing students' demographics and exam scores.

2. **Preprocessing**:
   - Average score is calculated from Math, Reading, and Writing.
   - A binary target label is created: `Pass (1)` or `Fail (0)`.
   - Categorical variables are encoded using `LabelEncoder`.

3. **Feature Engineering**:
   - Features are standardized using `StandardScaler`.

4. **Model Training**:
   - Data is split (80% training / 20% testing).
   - Three ML models are trained: Logistic Regression, Random Forest, and SVM.

5. **Model Evaluation**:
   - Each model is evaluated using Accuracy, Precision, Recall, and F1-Score.
   - Confusion matrices and classification reports are generated.

6. **Model Selection & Results**:
   - Random Forest outperformed others in terms of accuracy and generalization.
   - Most important features: parental education level, test preparation course.

---

## 📁 Repository Structure

```
├── Student_Performance_Capstone_Formatted.ipynb   # Main Jupyter Notebook
├── StudentsPerformance.csv                         # Input dataset (to be uploaded manually)
├── README.md                                       # Project overview and structure
└── Student_Performance_Capstone_Report.pdf         # (Optional) Report version of the notebook
```

---

## 📄 Report

A summarized PDF report is available:
- [Student_Performance_Capstone_Report.pdf](./Student_Performance_Capstone_Report.pdf)

---

## 🚀 How to Run

1. Clone this repository.
2. Make sure you have Python 3.7+ installed.
3. Install dependencies:
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn
   ```
4. Place `StudentsPerformance.csv` in the same directory.
5. Open and run `Student_Performance_Capstone_Formatted.ipynb` in Jupyter or Colab.

---

## 🙌 Acknowledgment

Thanks to **CACIITG IIT Guwahati** for providing this valuable learning opportunity through the Summer Analytics 2025 program.

---
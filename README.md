# Breast Cancer Diagnostic Classification 🧬💻

## Project Overview
This project applies machine learning techniques to classify breast cancer tumors as **Malignant (M)** or **Benign (B)** based on 30 clinical features derived from digitized images of fine needle aspirates (FNA) of breast masses.

The goal was to build an end-to-end pipeline from Exploratory Data Analysis (EDA) to Dimensionality Reduction and Model Evaluation to identify the most accurate diagnostic tool for clinical support.

## 🛠 Tech Stack
- **Language:** Python 3.x
- **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
- **Environment:** Jupyter Notebook / Google Colab

## 📈 Methodology

### 1. Exploratory Data Analysis (EDA)
- Analyzed 569 instances with features such as `radius_mean`, `texture_mean`, and `concavity_mean`.
- Visualized feature distributions and correlations to identify high-variance predictors.
- Handled data cleaning and verified class balance between Benign (62.7%) and Malignant (37.3%) cases.

### 2. Data Pre-processing & Feature Engineering
- **Feature Scaling:** Applied `StandardScaler` to ensure distance-based algorithms (like KNN) were not biased by feature magnitude.
- **Dimensionality Reduction:** Utilized **Principal Component Analysis (PCA)** to reduce the 30 features into principal components while retaining over 95% of the variance.

### 3. Model Implementation
I evaluated and compared both supervised and unsupervised learning approaches:
- **Unsupervised:** K-Means Clustering to identify natural groupings.
- **Supervised:** Random Forest Classifier and K-Nearest Neighbors (KNN).

## 🏆 Key Results
| Model | Performance Highlight |
| :--- | :--- |
| **Random Forest** | Highest overall accuracy and robust against overfitting. |
| **KNN** | Strong performance following proper feature scaling. |
| **PCA** | Successfully reduced noise while maintaining predictive power. |

## ⚖️ Ethical Considerations
In medical AI, "Explainability" is vital. While these models show high accuracy, they are intended to be **Decision Support Systems**, not replacements for clinical professionals. Considerations include ensuring dataset diversity to avoid diagnostic bias across different demographics.

## 📂 Repository Structure
```text
├── data/               # Cancer_Dataset.csv
├── notebooks/          # ML project.ipynb (Main Analysis)
└── README.md           # Project documentation

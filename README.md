# 🧠 Heart Stroke Prediction

A machine learning project to predict the likelihood of a stroke based on patient health data using the **Random Forest** classifier.

---

## 📌 Project Overview

Stroke is one of the leading causes of death and disability worldwide. This project builds a predictive model using patient demographic and clinical data to identify individuals at high risk of stroke — enabling early intervention.

---

## 📂 Dataset

- **Source:** [Kaggle — Healthcare Dataset Stroke Data](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset)
- **File:** `healthcare-dataset-stroke-data.csv`
- **Size:** ~5,000 rows, 12 columns
- **Target Variable:** `stroke` (0 = No Stroke, 1 = Stroke)

### Features:
| Feature | Description |
|---|---|
| `age` | Age of the patient |
| `gender` | Male / Female |
| `hypertension` | 0 = No, 1 = Yes |
| `heart_disease` | 0 = No, 1 = Yes |
| `ever_married` | Yes / No |
| `work_type` | Type of employment |
| `Residence_type` | Urban / Rural |
| `avg_glucose_level` | Average blood glucose level |
| `bmi` | Body Mass Index |
| `smoking_status` | Smoking history |

---

## 🔄 Project Workflow

1. **Data Loading** — Load dataset using pandas
2. **Exploratory Data Analysis (EDA)** — 10 visualizations including distributions, correlation heatmap, pairplot, and 3D scatter
3. **Data Preprocessing & Cleaning**
   - KNN Imputation for missing values
   - Outlier detection using IQR method
   - Log transformation to reduce skewness
   - One-Hot Encoding for categorical variables
4. **Feature Engineering** — Created BMI category and Age category features
5. **Model Training** — Random Forest Classifier
6. **Model Evaluation** — Accuracy, F1-Score, AUC, Cross-Validation
7. **Model Comparison** — Random Forest vs other classifiers

---

## ✅ Results

- **Model Used:** Random Forest Classifier
- **Top Features:** Age, Average Glucose Level, BMI
- **Evaluation Metrics:** Accuracy, AUC Score, F1-Score
- Model was validated using cross-validation to confirm stability

---

## 🛠️ Tech Stack

- Python 3.x
- pandas, numpy
- matplotlib, seaborn
- scikit-learn
- Jupyter Notebook

---

## 🚀 How to Run

```bash
# 1. Clone the repository
git clone https://github.com/your-username/Heart-Stroke-Prediction.git

# 2. Navigate into the folder
cd Heart-Stroke-Prediction

# 3. Install dependencies
pip install -r requirements.txt

# 4. Open the notebook
jupyter notebook Heart_Stroke_Prediction.ipynb
```

> ⚠️ Make sure `healthcare-dataset-stroke-data.csv` is in the same folder as the notebook.

---

## 📁 Repository Structure

```
Heart-Stroke-Prediction/
│
├── Heart_Stroke_Prediction.ipynb   ← Main project notebook
├── healthcare-dataset-stroke-data.csv ← Dataset
├── requirements.txt                ← Python dependencies
├── .gitignore                      ← Files to ignore
└── README.md                       ← Project documentation
```

---

## 📃 License

This project is licensed under the MIT License.

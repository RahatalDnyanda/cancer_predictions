<!-- PROJECT LOGO -->
<h1 align="center">
  🚀 Breast Cancer Classification
</h1>
<p align="center">
  A comprehensive pipeline for analyzing and classifying tumors using the Wisconsin Breast Cancer Dataset.
</p>

---

## 📖 Table of Contents
- [✨ Features](#✨-features)
- [📁 Project Structure](#📁-project-structure)
- [🛠️ Prerequisites](#🛠️-prerequisites)
- [🏗️ Installation & Running](#🏗️-installation--running)
- [📓 Notebook Workflow](#📓-notebook-workflow)
- [📈 Results](#📈-results)
- [🚀 Next Steps](#🚀-next-steps)
- [📜 License](#📜-license)

---

## ✨ Features
- **Data Cleaning & Inspection**: Remove irrelevant columns and check for missing values.
- **Exploratory Visualization**: Diagnosis distribution, correlation heatmap, and feature pairplots.
- **Preprocessing**: Encode labels, split data, and scale features.
- **Baseline Model**: Logistic Regression with accuracy, confusion matrix, and classification report.
- **Feature Selection**: Top-K features using `SelectKBest`.
- **Model Comparison**: Evaluate Logistic Regression, Random Forest, and SVM.
- **Hyperparameter Tuning**: Grid search for optimal Random Forest parameters.

---

## 📁 Project Structure
```bash
├── Cancer_data.csv        # Raw dataset (Wisconsin Breast Cancer)
├── breast_cancer.ipynb    # Jupyter notebook with end-to-end pipeline
└── README.md              # This overview and instructions
````

---

## 🛠️ Prerequisites

* Python 3.7 or above
* Jupyter Notebook / JupyterLab

Install dependencies:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

## 🏗️ Installation & Running

1. **Clone the repository**:

   ```bash
   ```

git clone [https://github.com/RahatalDnyanda/cancer_predictions.git](https://github.com/RahatalDnyanda/cancer_predictions.git)
cd cancer_predictions

````
2. **Open and run the notebook**:
   ```bash
jupyter notebook breast_cancer.ipynb
````

3. Execute cells in order to reproduce the analysis.

---

## 📓 Notebook Workflow

1. **Data Loading & Exploration**

   * Load `Cancer_data.csv` into a DataFrame
   * Inspect shape, data types, summary statistics, and missing values

2. **Data Cleaning**

   * Drop the `id` column and unnamed index columns
   * Confirm no missing or inconsistent values

3. **Visualization**

   * Plot the distribution of benign vs. malignant diagnoses
   * Create a correlation heatmap of features
   * Generate pairplots for key feature relationships

4. **Preprocessing**

   * Encode diagnosis: Benign (B) → 0, Malignant (M) → 1
   * Perform an 80/20 train-test split
   * Scale features with `StandardScaler`

5. **Model Training & Evaluation**

   * Train a Logistic Regression model
   * Evaluate using accuracy, confusion matrix, and classification report

6. **Advanced Analysis**

   * **Feature Selection**: Identify top 10 features via `SelectKBest`
   * **Model Comparison**: Benchmark Logistic Regression, Random Forest, and SVM
   * **Hyperparameter Tuning**: Optimize Random Forest with `GridSearchCV`

---

## 📈 Results

* **Baseline Accuracy**: \~96.5% with Logistic Regression
* **Key Features**: Radius mean, Texture mean, Perimeter mean, etc.
* **Tuned Model**: Random Forest achieved improved performance after grid search.

---

## 🚀 Next Steps

* **Web Deployment**: Build a Flask/Django/Streamlit app for real-time predictions
* **Cross-Validation**: Implement k-fold validation to ensure model robustness
* **Advanced Models**: Experiment with XGBoost, LightGBM, and ensemble methods
* **Explainability**: Use SHAP or LIME to interpret model predictions

---
# ML_in_Drug_Discovery_using_SWISSADME_Properties
ML_in_Drug_Discovery_using_SWISSADME_Properties
# 💊 ML in Drug Discovery: Modeling with SWISSADME Properties

This repository contains a specialized **Jupyter Notebook** pipeline that demonstrates the use of **physicochemical properties** derived from the **SWISSADME** online tool for machine learning applications in drug discovery.

The workflow focuses on utilizing computed properties (which relate to Absorption, Distribution, Metabolism, Excretion, and Toxicity—**ADMET**) as features to build a predictive model for a target biological activity or property.

---

## 🚀 Key Features

* **ADMET-Focused Modeling:** Focuses on using crucial ADMET-related descriptors (e.g., Lipinski's Rule of Five, TPSA, LogP) as input features for machine learning.
* **Data Integration:** Designed to load a dataset where **SWISSADME properties have been pre-computed** and linked to a biological activity (e.g., pIC50, classification of active/inactive).
* **Predictive Modeling:** Implements a classification or regression model (e.g., Logistic Regression, Random Forest) to predict the target activity.
* **Exploratory Data Analysis (EDA):** Includes steps for inspecting the distribution and correlation of the ADMET descriptors.
* **Model Validation:** Splits data into training/testing sets and evaluates model performance using metrics suitable for the task (e.g., Accuracy, AUC, $R^2$).
* **Visualization:** Generates plots to visualize the model's performance and the chemical space defined by the SWISSADME features.

---

## 🔬 Analysis Overview

| Component | Method / Tool | Purpose |
| :--- | :--- | :--- |
| **Input Data** | SWISSADME Descriptors + Activity | Pre-calculated molecular properties linked to experimental bioactivity data. |
| **Modeling** | ML Model (Classification/Regression) | Builds a predictive model based on ADMET characteristics. |
| **Prediction Target** | Bioactivity or ADMET Property | Predicts a key output relevant to a compound's drug-likeness. |
| **Evaluation** | Standard ML Metrics (Accuracy, AUC, RMSE) | Quantifies the reliability of the predictive model. |

---

## 🛠️ Prerequisites and Setup

### 📦 Data Requirement

This notebook requires a **CSV file** (or similar) where the columns correspond to the output properties obtained from the SWISSADME tool (e.g., $\text{MW}$, $\text{LogP}$, $\text{HBA}$, $\text{HBD}$, TPSA) and includes a target variable (activity/inactivity).

### 🖥️ Requirements

This pipeline requires a Python environment with the following libraries installed:

* `pandas`
* `numpy`
* `matplotlib` / `seaborn`
* `scikit-learn` (sklearn)

### ⚙️ Execution

1.  **Download** the `ML_in_Drug_Discovery_using_SWISSADME_Properties.ipynb` file.
2.  **Ensure your dataset** containing the SWISSADME features is accessible by the notebook.
3.  Open and run the notebook in a Jupyter environment (e.g., JupyterLab or Google Colab) by executing all cells sequentially.

---

## 📊 Expected Output

The final output demonstrates the model's utility based on ADMET properties:

* **EDA Plots:** Visualizations showing the distribution of key ADMET features (e.g., TPSA, $\text{LogP}$).
* **Model Performance Metrics:** The final classification or regression scores (e.g., Confusion Matrix plot, Accuracy, or $R^2$).
* **Prediction Plot:** A plot showing the model's performance (e.g., ROC curve for classification or predicted vs. actual values for regression).

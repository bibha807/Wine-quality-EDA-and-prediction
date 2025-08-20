# Wine-quality-EDA-and-prediction
# 🍷 Red Wine Quality Prediction

## 📌 Project Overview
This project predicts the quality of Portuguese "Vinho Verde" red wine using **machine learning** techniques.  
The dataset contains **1599 samples**, each described by **11 physicochemical properties** (lab test results) and a **quality score** (0–10, given by wine experts).  

The goal is to build models that can classify or predict wine quality based on these chemical attributes.  

---

## 📝 Purpose of the Python Code
- Perform **exploratory data analysis (EDA)** to uncover insights into wine quality.  
- Preprocess and clean the dataset for modeling.  
- Train and evaluate **multiple machine learning models** (classification & regression).  
- Compare performance using appropriate metrics (Accuracy, F1-score, RMSE, R²).  
- Identify the **most important features** influencing wine quality.  

---

## 🔬 Dataset Information
**Input Features**:  
- Fixed acidity, Volatile acidity, Citric acid, Residual sugar  
- Chlorides, Free sulfur dioxide, Total sulfur dioxide  
- Density, pH, Sulphates, Alcohol  
  Here's how the dataset looks like - ![redwine-quality.csv](https://github.com/bibha807/Wine-quality-EDA-and-prediction/blob/main/winequality-red.csv)
  
**Target Variable**:  
- **Quality** (integer score 3–8, imbalanced around 5–7)

---

## 🔍 Exploratory Data Analysis (EDA)
- **Quality Distribution** → Majority of wines rated 5, 6, or 7.  
- **Correlations with Quality**:  
  - Alcohol → Strong positive correlation  
  - Volatile acidity → Strong negative correlation  
  - Sulphates, citric acid → Moderate positive correlation  
  - Density → Negative correlation  
- **Visualizations** → Histograms, boxplots, correlation heatmaps used to identify trends and outliers.  

---

## 🛠️ Workflow
1. **Data Loading & Cleaning**  
   - Loaded dataset (`;` separated CSV).  
   - Checked for missing/null values (none found).  
   - Stripped column names, standardized features.  

2. **Exploratory Data Analysis**  
   - Feature distributions  
   - Correlation heatmap  
   - Quality imbalance check  

3. **Modeling**  
   - **Classification**: Logistic Regression, Train Test split, Random Forest Classifier, Accuracy score  
   - **Regression**: Linear Regression, Random Forest Regressor  

4. **Evaluation**  
   - Classification: Accuracy, Precision, Recall, F1-score, Confusion Matrix  
   - Regression: RMSE, MAE, R² Score  
   - Cross-validation for robustness  

---

## 💻 Tech Stack
- **Programming Language**: Python  
- **Libraries Used**:  
  - Data Analysis → Pandas, NumPy  
  - Visualization → Matplotlib, Seaborn  
  - Machine Learning → Scikit-learn  
- **Environment**: Jupyter Notebook, Google Colaboratory  

---

## 📈 Results
- **Best Models**: Random Forest & Gradient Boosting (~70% accuracy). 
- **Baseline Model**: Logistic Regression (~55–60% accuracy).  
- **Regression R² Score**: ~0.35–0.40 (moderate predictability).  
- **Key Predictors**: Alcohol, volatile acidity, sulphates, citric acid.
  **Here's the .ipynb file: ![Python code]([https://github.com/bibha807/Wine-quality-EDA-and-prediction/blob/main/winequality-red.csv](https://github.com/bibha807/Wine-quality-EDA-and-prediction/blob/main/Wine%20quality%20EDA%20and%20prediction.ipynb))  

---

## 🚀 Conclusion
This project demonstrates how physicochemical tests can be used to predict wine quality with machine learning.  
While models show decent accuracy, results highlight the **subjective nature of wine ratings**.  
The study provides valuable insights into which chemical properties most influence wine quality, helping in **quality control and wine production**.  

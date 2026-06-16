# Minor Project: NHANES Body Measurements Analysis

## 📌 Project Overview
This project analyzes adult male and female body measurements from the **National Health and Nutrition Examination Survey (NHANES)** dataset.  
The goal is to explore anthropometric data, compute derived health indicators (BMI, waist-to-height ratio, waist-to-hip ratio), and compare distributions between genders using Python.

---

## 📂 Dataset Description
Two CSV files are used:
- `male_dataset.csv` → Adult male body measurements
- `female_dataset.csv` → Adult female body measurements

Each dataset contains **7 columns**:
1. Weight (kg)  
2. Standing height (cm)  
3. Upper arm length (cm)  
4. Upper leg length (cm)  
5. Arm circumference (cm)  
6. Hip circumference (cm)  
7. Waist circumference (cm)  

---

## ⚙️ Project Workflow
1. **Data Loading**  
   - Read CSV files into pandas DataFrames.  
   - Convert them into NumPy matrices (`male`, `female`).  

2. **Data Cleaning**  
   - Handle missing values and duplicates.  
   - Ensure numeric data types.  
   - Apply sanity checks (e.g., weight > 30 kg, height > 120 cm).  

3. **Exploratory Analysis**  
   - Histograms of male vs female weights.  
   - Boxplots comparing distributions.  
   - Descriptive statistics (mean, median, std, skewness, kurtosis).  

4. **Derived Metrics**  
   - Compute BMI for females.  
   - Standardize female dataset (`zfemale`) using z-scores.  
   - Add waist-to-height ratio (WHtR) and waist-to-hip ratio (WHR) for both genders.  

5. **Correlation & Visualization**  
   - Scatterplot matrix (pairplot) for selected variables.  
   - Pearson and Spearman correlation coefficients.  

6. **Comparative Analysis**  
   - Boxplots of WHtR and WHR across genders.  
   - Discussion of BMI, WHtR, WHR advantages and limitations.  
   - Identify individuals with lowest and highest BMI (standardized values).  

---

## 📊 Tools & Libraries
- **NumPy** → Matrix operations  
- **Pandas** → Data handling  
- **Matplotlib / Seaborn** → Visualization  
- **SciPy** → Statistical measures  

---

## Reference 
Kaggle: Referenced Kaggle programs and datasets for student performance analysis and predictive modeling.
GitHub: Utilized GitHub repositories on target prediction for deep learning implementation guidance.
Copilot: Applied Copilot support for code correction and EDA program refinement.

---

## 🧾 Key Insights
- Male participants generally have higher mean weight and greater dispersion.  
- BMI correlates strongly with waist and hip circumference, but less with height.  
- WHtR is a better predictor of cardiovascular risk compared to BMI alone.  
- WHR highlights gender differences in fat distribution.  

---

## 🚀 How to Run
1. Clone this repository.  
2. Place `male_dataset.csv` and `female_dataset.csv` in the project folder.  
3. Run the Jupyter Notebook:  
   ```bash
   jupyter notebook nhanes_analysis.ipynb


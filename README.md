# 🩺 Chronic Kidney Disease (CKD) EDA Analysis

## 🔍 Project Overview
This project focuses on performing Exploratory Data Analysis (EDA) on a Chronic Kidney Disease (CKD) dataset to identify important medical indicators, patient trends, and health patterns associated with kidney disease.

The main objective of this analysis is to uncover insights that can support early CKD detection and improve healthcare decision-making using data analytics techniques.

---

## 📁 Dataset Information
- Source: Kaggle – kidney_disease.csv  
- Total Patients: 400  
- Features: 25 Columns  

### Dataset Distribution
- CKD Positive Patients: 250  
- Healthy Patients: 150  

### Key Features Used
- Age  
- Blood Pressure  
- Blood Urea  
- Serum Creatinine  
- Haemoglobin  
- Blood Glucose Random  
- Sodium  
- Potassium  
- Hypertension  
- Diabetes Mellitus  
- Coronary Artery Disease  
- Anaemia  
- Appetite  

- Data Type: Mixed (Numerical + Categorical)  
- Nature: Real-world medical dataset with missing values and inconsistent entries  

---

## 🧹 Data Cleaning & Preprocessing

The dataset required extensive preprocessing before analysis:

- Removed unnecessary ID column  
- Renamed short column codes for better readability  
- Converted object columns into numerical format using:
```python
pd.to_numeric(errors='coerce')
```

- Cleaned inconsistent categorical values:
  - '\tyes' → yes  
  - '\tno' → no  

- Encoded target variable:
  - CKD → 1  
  - Not CKD → 0  

### Missing Value Handling
- Numerical columns → Median imputation  
- Categorical columns → Mode imputation  

💡 Median imputation was used to reduce the effect of outliers in medical data.

---

## 📊 Exploratory Data Analysis

### 🔹 Univariate Analysis
- CKD prevalence distribution  
- Age group analysis  
- Blood pressure trends  

### 🔹 Bivariate Analysis
- CKD vs Blood Urea  
- CKD vs Serum Creatinine  
- CKD vs Haemoglobin  
- Hypertension vs CKD  

### 🔹 Multivariate Analysis
- Correlation Heatmap  
- PairGrid Analysis  
- 3D Scatter Visualization  
- Feature relationship analysis  

---

## 📌 Key Insights

### 🩺 CKD Prevalence
- 62.5% patients in the dataset were CKD positive  
- Dataset is imbalanced and requires careful ML handling  

### 🩸 Strongest CKD Predictor
- Haemoglobin showed the strongest correlation with CKD:
```python
Correlation = -0.769
```

→ Lower haemoglobin strongly indicates CKD risk.

### 💉 Medical Risk Indicators
CKD patients generally showed:
- Higher Blood Urea  
- Higher Serum Creatinine  
- Higher Blood Glucose  
- Lower Haemoglobin  

🚨 Serum Creatinine > 1.2 mg/dL emerged as a major CKD indicator.

### 📈 Age & Hypertension
- Majority of patients belonged to the 41–60 age group  
- CKD risk increased with age and hypertension  

### 💊 Comorbidity Findings
Strong overlap found between CKD and:
- Hypertension  
- Diabetes Mellitus  
- Anaemia  

### 🔗 Correlation Analysis
Positive CKD correlations:
- Blood Glucose  
- Blood Urea  
- Serum Creatinine  

Negative CKD correlations:
- Haemoglobin  
- Sodium  
- Packed Cell Volume  

---

## 💡 Key Learnings

- Medical datasets require extensive preprocessing  
- Incorrect datatypes can completely distort analysis  
- Proper missing value handling is critical in healthcare analytics  
- Correlation analysis helps identify important predictive features  
- EDA is not just visualization — it helps uncover clinically meaningful patterns  

---

## 🛠️ Tools & Technologies Used
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Plotly  


Examples:
- Correlation Heatmap  
- PairGrid Analysis  
- CKD Distribution Plot  
- 3D Scatter Plot  

---

## 🚀 How to Run the Project

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/ckd-eda-analysis.git
```

### 2️⃣ Install Required Libraries
```bash
pip install pandas numpy matplotlib seaborn plotly
```

### 3️⃣ Run Jupyter Notebook
```bash
jupyter notebook
```

---

## 📌 Project Status
✅ Completed  
🔄 Open for improvements and feedback  

---

## 🤝 Connect With Me
I’m currently learning Data Analytics and building real-world projects.

- LinkedIn: (Add your LinkedIn profile)  
- GitHub: (https://github.com/Bhumika-kushwah)  

---

## ⭐ If You Found This Useful
Give this repository a star ⭐ and share your feedback!

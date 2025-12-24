# 📌 Task 1: Data Cleaning & Preprocessing

This project was completed as part of the Data Analyst Internship.  
The goal of this task was to clean a raw dataset by removing missing values, duplicates, formatting issues and preparing it for further analysis.

---

## 📁 Dataset Used
- **Dataset Name:** Netflix Movies & TV Shows
- **Source:** Kaggle
- **File Format:** CSV  
- **Raw File:** netflix_full.csv  

This dataset contains information like:  
- title  
- director  
- cast  
- country  
- date added  
- release year  
- rating  
- type  
- duration  

---

## 🔧 Steps Performed in Data Cleaning

### 1️⃣ Loading the Dataset  
- Imported the CSV file into Google Colab using Pandas.

### 2️⃣ Exploring the Data  
- Checked structure using `df.info()`
- Identified missing values using `df.isnull().sum()`
- Checked duplicate rows using `df.duplicated().sum()`

### 3️⃣ Handling Duplicates  
- Removed duplicate rows using `df.drop_duplicates()`

### 4️⃣ Handling Missing Values  
- Numerical columns → filled using **mean**  
- Text columns → filled using **mode**  
- Ensured there are **zero missing values** after cleaning

### 5️⃣ Standardizing Text  
- Converted all text columns to lowercase  
- Removed extra spaces using `.str.strip()`

### 6️⃣ Converting Date Format  
- Converted `date_added` to **datetime** format using `pd.to_datetime()`  
- Handled invalid dates using `errors='coerce'`

### 7️⃣ Cleaning Column Names  
- Converted all column names to lowercase  
- Replaced spaces with underscores for better readability

---

## 📦 Output Files

| File | Description |
|------|-------------|
| **netflix_full.csv** | Original raw dataset |
| **cleaned_netflix_data.csv** | Cleaned final dataset |
| **elevatelabs.ipynb** | Google Colab notebook with complete code |
| **README.md** | Documentation for the task |

---

## 🛠 Tools Used
- Python  
- Pandas  
- Google Colab  

---

## 🎯 What I Learned
- How to handle missing values  
- How to remove duplicates  
- How to standardize inconsistent data  
- How to format date columns properly  
- How to preprocess real-world datasets  
- How to export a cleaned dataset  

---

### ✅ Task Successfully Completed 🎉

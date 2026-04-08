# global-superstore-eda-cleaning
Data understanding, exploratory analysis, and cleaning of the Global Superstore dataset using Excel. Includes handling missing values, data type correction, and feature engineering for analysis.

# 📊 Project 2: Data Understanding & Cleaning — Superstore Dataset

---

## 📑 Table of Contents
- [📌 Project Overview](#-project-overview)
- [📂 Dataset Summary](#-dataset-summary)
- [🔍 Exploratory Data Analysis (EDA)](#-exploratory-data-analysis-eda)
- [🧹 Data Cleaning & Preprocessing](#-data-cleaning--preprocessing)
- [🧠 Decisions & Assumptions](#-decisions--assumptions)
- [⚠️ Challenges & Limitations](#️-challenges--limitations)
- [📊 Final Cleaned Dataset](#-final-cleaned-dataset)
- [🛠 Tools Used](#-tools-used)
- [✅ Conclusion](#-conclusion)
- [📁 Project Structure](#-project-structure)

---9

## 📌 Project Overview
This project focuses on understanding and preparing the Superstore dataset for analysis.  
The objective is to explore the dataset structure, identify data quality issues, and perform necessary cleaning to ensure it is suitable for further analysis and visualization.

---

## 📂 Dataset Summary
- **Dataset Name:** Global Superstore Dataset  
- **Total Rows:** 51,291  
- **Total Columns:** 24  
- **Data Type:** Retail transactional data  

---

## 🔍 Exploratory Data Analysis (EDA)

### 📊 Dataset Structure
The dataset contains transactional data including:
- Order details (Order ID, Order Date, Ship Date)
- Customer information
- Product details
- Sales, Profit, Quantity, Discount
- Geographic and regional data

📸 **Dataset Preview (First Rows)**  
<img width="1380" height="673" alt="Dataset Overview" src="https://github.com/user-attachments/assets/785bd326-df40-4625-b223-86b71415e80f" />

---

### 🔎 Data Types & Formatting
- Date columns were initially not in proper date format  
- Numeric columns were stored as **General format**

---

### ⚠️ Missing Values
- Missing values were identified in the **Postal Code** column  

📸 **Missing Values Evidence**  
<img width="272" height="810" alt="Missing Values" src="https://github.com/user-attachments/assets/f360e85a-79a6-4d4b-af67-a0a50f859bd3" />


---

### 🔁 Duplicate Records
- No duplicate records were found in the dataset  

📸 **Duplicate Check**  
<img width="1884" height="1001" alt="No Duplicate Confirmation" src="https://github.com/user-attachments/assets/073579fe-17ed-4c17-91f3-8ad2ea66cb7c" />


---

### 🔤 Unique Values (Categorical Insights)
Categorical columns such as:
- Country  
- Category  
- Segment  

Contain multiple unique values, making them useful for segmentation and analysis.

---

### 📉 Outliers & Unusual Trends
- Negative profit values were observed  
- Some transactions show unusually high or low values  

📸 **Outlier Detection (Profit Sorted)**  
<img width="90" height="805" alt="Outliers" src="https://github.com/user-attachments/assets/91243d5e-0c6f-449f-8560-038e409ac43b" />



👉 These indicate potential loss-making transactions and are important for business insights.

---

## 🧹 Data Cleaning & Preprocessing

### ✅ Steps Performed

1. Converted dataset into structured table format  
2. Checked and handled missing values  
3. Removed duplicates (none found)  
4. Corrected data types (dates & numeric fields)  
5. Standardized text fields  
6. Removed irrelevant columns (Row ID hidden)  
7. Created new calculated fields  

---

### ➕ New Features Created (Key Highlight 🚀)

#### 📅 Delivery Days
- Measures time between order and shipment  
- Helps evaluate delivery efficiency  


---

#### 💰 Profit Margin
- Measures profitability per transaction  
- Helps assess business performance  


---

## 🧠 Decisions & Assumptions

### 📌 Key Decisions
- Postal Code missing values were left unchanged to preserve data integrity  
- Negative profit values were retained as valid business outcomes  
- No rows were removed to avoid data loss  

---

### ⚖️ Assumptions
- All records represent valid transactions  
- Profit/loss values reflect real business performance  

---

## ⚠️ Challenges & Limitations

### 🚧 Challenges
- Difficulty handling blank Postal Code values due to formatting inconsistencies  
- Ensuring consistent data types across all columns  

### ⚠️ Limitations
- Missing Postal Codes limit geographic precision  
- No external validation for anomalies  

---

## 📊 Final Cleaned Dataset

The dataset is now:
- Structured and organized  
- Free from duplicates  
- Properly formatted  
- Enriched with new calculated fields  

📸 **Clean Dataset Preview**  
<img width="1892" height="816" alt="Final Clean Daaset" src="https://github.com/user-attachments/assets/35da2e8d-ff13-472b-ae09-cdfdf15fb400" />


---

## 🛠 Tools Used
- Microsoft Excel  

---

## ✅ Conclusion
The dataset has been successfully cleaned and prepared for analysis.  
Key data quality issues were addressed, and new features were created to enhance analytical capabilities.

The dataset is now ready for:
- Data visualization  
- KPI analysis  
- Dashboard development  

---

## 📁 Project Structure

📦 superstore-kpi-analysis
 ┣ 📂 images
 ┃ ┣ dataset_overview.png
 ┃ ┣ missing_values.png
 ┃ ┣ no_duplicates.png
 ┃ ┣ outliers.png
 ┃ ┗ final_clean_dataset.png
 ┣ 📄 Global_Superstore_cleaned.xlsx
 ┗ 📄 README.md

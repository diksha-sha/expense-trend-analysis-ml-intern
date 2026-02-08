# Purchase Expense Trend Analysis  
Data Science / ML Intern Technical Assignment  

## Project Overview
This project analyzes purchase invoice data to understand how expenses change over time and identify meaningful financial patterns.

The objective is to simulate real-world accounting analysis using structured invoice data and extract actionable insights relevant to budgeting and financial monitoring.

The analysis focuses on:
- Monitoring monthly expense trends  
- Identifying top expense categories  
- Detecting unusual spending spikes  
- Comparing GST contribution to base expense  
- Segmenting vendors using clustering  

---

## Dataset
A synthetic dataset containing 500 purchase invoice records was generated using Python.
Each record includes:
- Invoice Date  
- Vendor Name  
- Expense Category  
- Invoice Amount  
- GST Rate  
- GST Amount  
The dataset was programmatically generated to simulate realistic accounting patterns with multiple vendors, expense categories, and GST variations.
The dataset file included in the repository:
purchase_data.csv

---

## Steps Performed
1. Data Generation – Created synthetic invoice dataset.
2. Data Preparation – Converted date formats and ensured data consistency.
3. Feature Engineering – Extracted month and calculated expense without GST.
4. Monthly Expense Trend Analysis – Aggregated expenses by month.
5. Top Expense Category Analysis – Identified major cost drivers.
6. Unusual Expense Detection – Applied statistical threshold (Mean + 1.5 × Std).
7. GST vs Base Expense Analysis – Evaluated tax contribution.
8. Vendor Clustering – Applied K-Means clustering to segment vendors.

---

## Key Insights
- Monthly expenses show noticeable variation across the year.
- Certain months exceed statistical thresholds, indicating possible bulk procurement or high operational activity.
- A small number of expense categories contribute significantly to total spending.
- GST contributes approximately 11.54% of total expenditure.
- Vendors were segmented into three groups (Low, Medium, High spenders), which can assist in procurement strategy and vendor prioritization.

---

## Machine Learning Component
K-Means clustering was applied on vendor-level aggregated spending data.
This segmentation can help:
- Identify high-value vendors  
- Prioritize vendor negotiations  
- Monitor vendor concentration risk  
- Improve procurement decision-making  

---

## Technologies Used
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Scikit-learn  

---

## Limitation
Since the dataset is synthetically generated, real-world economic conditions, seasonality, and market fluctuations are not fully represented.

---

## Repository Structure
expense-trend-analysis-ml-intern/
│
├── ML_Intern_Expense_Analysis.ipynb
├── purchase_data.csv
├── README.md
├── THINKING.md
└── requirements.txt

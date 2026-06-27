# 🛒 RetailMart Smart ETL Pipeline

An end-to-end **Data Engineering** project that automates the **Extract, Transform, Load (ETL)** process for retail sales data using **Python, Pandas, NumPy, SQLite, SQL, and Matplotlib**.

## 📌 Project Overview

RetailMart Pvt. Ltd. generates large volumes of daily retail sales data from stores across India. Since the data contains missing values, duplicate records, and inconsistent formats, this project builds an automated ETL pipeline that cleans, transforms, stores, and analyzes retail data efficiently.

The pipeline enables:

- Data ingestion from multiple CSV files
- Data cleaning and validation
- Dataset integration and transformation
- Revenue calculation and analysis
- SQL-based reporting
- Business intelligence insights
- Data visualization

---

## 🚀 Features

✅ Automated ETL Workflow  
✅ Data Cleaning & Validation  
✅ Missing Value Handling  
✅ Duplicate Removal  
✅ Data Type Standardization  
✅ Dataset Merging  
✅ Revenue Calculation  
✅ SQLite Database Integration  
✅ SQL Analytics  
✅ Business Reports Generation  
✅ Data Visualization  
✅ Error Handling and Pipeline Automation  

---

## 🛠️ Technology Stack

| Technology | Purpose |
|------------|----------|
| Python | ETL Pipeline Development |
| Pandas | Data Processing & Cleaning |
| NumPy | Numerical Analysis |
| SQLite | Database Storage |
| SQL | Data Analytics |
| Matplotlib | Data Visualization |
| Jupyter Notebook | Development & Documentation |

---

## 📂 Project Structure

```text
RetailMart-ETL/
│
├── sales_data.csv
├── products.csv
├── stores.csv
├── RetailMart_Project.ipynb
├── RetailMart.db
├── README.md
│
└── outputs/
    ├── revenue_by_city.png
    └── top_products.png
```

---

## ⚙️ ETL Workflow

### 1️⃣ Extract

Load data from:

- sales_data.csv
- products.csv
- stores.csv

### 2️⃣ Transform

Perform:

- Missing value handling
- Duplicate removal
- Column standardization
- Data type conversion
- Dataset merging
- Revenue calculation

### 3️⃣ Load

Store processed data into:

```sql
SQLite Database → RetailMart.db
```

Table:

```sql
retail_sales
```

### 4️⃣ Analyze

Generate:

- Revenue by city
- Revenue per store
- Top-selling products
- Business summary reports
- Visualizations

---

## 📊 Sample Analytics

### Revenue Analysis

- Total Revenue Generated
- Mean Revenue
- Maximum Revenue
- Minimum Revenue

### Product Analysis

- Top 3 Best Selling Products
- Product-wise Quantity Sold

### Store Analysis

- Revenue Per Store
- Revenue Per Day

---

## 📈 Visualizations

The project generates:

### Revenue by City

<img width="1102" height="592" alt="image" src="https://github.com/user-attachments/assets/7def8ccd-1e11-4595-a0ac-297ca263f21d" />


### Top Selling Products

<img width="706" height="428" alt="image" src="https://github.com/user-attachments/assets/ef0ff06b-cf3b-40b7-87e0-c1d10a6cf452" />

---

## 🗄️ SQL Queries Included

### Top 3 Best Selling Products


```sql
SELECT
    product_name,
    SUM(quantity) AS total_quantity
FROM retail_sales
GROUP BY product_name
ORDER BY total_quantity DESC
LIMIT 3;
```


### Revenue Per Store Per Day

```sql
SELECT
    store_name,
    sale_date,
    SUM(total_revenue) AS total_revenue
FROM retail_sales
GROUP BY store_name, sale_date
ORDER BY sale_date;
```

---

## ▶️ How to Run

### Clone Repository

```bash
git clone https://github.com/your-username/RetailMart-ETL.git
cd RetailMart-ETL
```

### Install Dependencies

```bash
pip install pandas numpy matplotlib
```

### Run Jupyter Notebook

```bash
jupyter notebook RetailMart_Project.ipynb
```

---

## 📚 Learning Outcomes

This project demonstrates practical knowledge of:

- Data Engineering
- ETL Pipeline Development
- Data Cleaning Techniques
- Data Transformation
- Database Management
- SQL Analytics
- Business Intelligence
- Data Visualization


## 👩‍💻 Author

**Kashish Sharma**  
Master of Computer Applications (MCA)

---

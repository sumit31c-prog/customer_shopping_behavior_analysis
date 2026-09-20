# 📊 Data Analytics Project

## 📌 Overview

This project demonstrates an end-to-end **Data Analytics workflow**, starting from raw data and ending with an interactive **Power BI dashboard and business presentation**.

The project includes:

* Data exploration and analysis using Python
* Data cleaning and transformation
* SQL analysis using MySQL Workbench
* Interactive dashboard development using Power BI
* Business insights and report preparation
* AI-assisted presentation (PPT) creation

The goal is to transform raw customer shopping data into meaningful insights that can support data-driven business decisions.

---

## 📂 Dataset

**Dataset:** Customer Shopping Behavior

The dataset contains customer purchase information such as:

* Customer demographics
* Age and age groups
* Product categories
* Products purchased
* Purchase amount
* Purchase frequency
* Discount information
* Review ratings
* Payment methods
* Shopping-related attributes

The raw dataset was initially processed and cleaned before performing analysis.

---

## 🛠️ Tools & Technologies

| Tool                     | Purpose                                     |
| ------------------------ | ------------------------------------------- |
| **Python**               | Data analysis and preprocessing             |
| **Pandas**               | Data manipulation and cleaning              |
| **NumPy**                | Numerical operations                        |
| **Matplotlib / Seaborn** | Exploratory Data Analysis and visualization |
| **MySQL Workbench**      | SQL analysis and business queries           |
| **Power BI**             | Interactive dashboard                       |
| **PowerPoint**           | Business presentation                       |
| **AI Tools**             | Report and presentation assistance          |
| **Jupyter Notebook**     | Python development environment              |

---

## 🔄 Project Workflow

```text
Raw Dataset
     ↓
Python Data Loading
     ↓
Data Exploration
     ↓
Data Cleaning & Transformation
     ↓
EDA & Visualization
     ↓
MySQL Database
     ↓
SQL Analysis
     ↓
Power BI Dashboard
     ↓
Business Insights & Report
     ↓
AI-Assisted PPT Presentation
```

---

## 🐍 Step 1: Python – Data Loading & EDA

The dataset was imported into Python using Pandas.

Key activities included:

* Loading the dataset
* Understanding rows and columns
* Checking data types
* Checking missing values
* Identifying duplicate records
* Understanding numerical and categorical variables
* Generating descriptive statistics
* Exploring relationships between variables

Example:

```python
import pandas as pd

df = pd.read_csv("customer_shopping_behavior.csv")

df.head()
df.info()
df.describe()
df.isnull().sum()
df.duplicated().sum()
```

---

## 🧹 Step 2: Data Cleaning & Transformation

The dataset was cleaned to improve data quality and prepare it for analysis.

Key cleaning activities included:

* Handling missing values
* Removing duplicate records
* Correcting data types
* Standardizing column names
* Cleaning categorical values
* Creating calculated columns
* Transforming purchase frequency into numerical values
* Preparing the final dataset for SQL analysis

The cleaned dataset was then loaded into MySQL for further analysis.

---

## 🗄️ Step 3: SQL Analysis – MySQL Workbench

The cleaned data was imported into **MySQL Workbench**.

SQL was used to answer business-related questions and identify important patterns.

Examples of analysis include:

* Total revenue
* Revenue by age group
* Top-selling products
* Top products within each category
* Purchase behavior by customer segment
* Product category performance
* Customer purchasing frequency
* Revenue contribution
* Other business KPIs

Example SQL query:

```sql
SELECT 
    age_group,
    SUM(purchase_amount) AS total_revenue
FROM customer_shopping
GROUP BY age_group
ORDER BY total_revenue DESC;
```

SQL analysis helped convert the cleaned dataset into meaningful business insights.

---

## 📊 Step 4: Power BI Dashboard

The analyzed data was used to build an interactive **Power BI dashboard**.

### Dashboard Features

The dashboard includes KPIs and visualizations such as:

* Total Revenue
* Total Customers
* Total Purchases
* Average Purchase Amount
* Revenue by Age Group
* Revenue by Product Category
* Top Products
* Purchase Frequency
* Customer Segmentation
* Interactive filters and slicers

The dashboard allows users to explore customer behavior and business performance interactively.

### Dashboard Preview

> Add your Power BI dashboard screenshot here.

```text
![Power BI Dashboard](images/dashboard.png)
```

---

## 📈 Step 5: Business Insights & Results

The analysis helped identify important patterns in customer purchasing behavior.

Key areas analyzed include:

* Which customer groups contribute the most revenue
* Which product categories generate higher sales
* Which products are purchased most frequently
* Customer purchasing patterns
* Revenue distribution across different segments
* Relationship between customer characteristics and purchasing behavior

These findings can help businesses improve:

* Product strategy
* Customer segmentation
* Marketing campaigns
* Promotional offers
* Revenue optimization
* Inventory planning

---

## 📑 Step 6: Report

A business report was created to summarize the project findings.

The report includes:

1. Business objective
2. Dataset description
3. Data cleaning process
4. Exploratory analysis
5. SQL analysis
6. Power BI dashboard
7. Key insights
8. Business recommendations
9. Conclusion

---

## 🤖 Step 7: AI-Assisted PPT

An AI-assisted PowerPoint presentation was created to communicate the project findings clearly.

The presentation covers:

* Project objective
* Dataset overview
* Data preparation
* Analysis methodology
* SQL insights
* Power BI dashboard
* Key findings
* Business recommendations
* Conclusion

AI was used to assist with **presentation structure, content organization, and communication of analytical findings**.

---

## ▶️ How to Run the Project

### 1. Clone the Repository

```bash
git clone <your-github-repository-url>
```

### 2. Install Python Libraries

```bash
pip install pandas numpy matplotlib seaborn sqlalchemy pymysql jupyter
```

### 3. Open Jupyter Notebook

```bash
jupyter notebook
```

Open the project notebook and run the Python analysis step by step.

### 4. Set Up MySQL

Create a MySQL database and import the cleaned dataset.

Update your database connection details in Python:

```python
from sqlalchemy import create_engine
from urllib.parse import quote_plus

username = "root"
password = quote_plus("YOUR_PASSWORD")
host = "localhost"
port = 3306
database = "YOUR_DATABASE"

engine = create_engine(
    f"mysql+pymysql://{username}:{password}@{host}:{port}/{database}"
)
```

> Do not upload your actual MySQL password to GitHub.

### 5. Run SQL Analysis

Open **MySQL Workbench** and execute the SQL queries included in the project.

### 6. Open Power BI Dashboard

Open the `.pbix` file in Power BI Desktop.

If required, update the data source connection and refresh the dataset.

---

## 📁 Project Structure

```text
Data-Analytics-Project/
│
├── data/
│   └── customer_shopping_behavior.csv
│
├── notebooks/
│   └── data_analysis.ipynb
│
├── sql/
│   └── analysis_queries.sql
│
├── powerbi/
│   └── customer_behavior_dashboard.pbix
│
├── report/
│   └── project_report.pdf
│
├── presentation/
│   └── project_presentation.pptx
│
├── images/
│   └── dashboard.png
│
└── README.md
```

---

## 🎯 Key Skills Demonstrated

This project demonstrates practical experience in:

* Data Cleaning
* Exploratory Data Analysis
* Python
* Pandas
* NumPy
* Data Visualization
* SQL
* MySQL
* Business Analysis
* Power BI
* Dashboard Development
* Data Storytelling
* Report Writing
* AI-Assisted Presentation Creation

---

## 🚀 Conclusion

This project demonstrates a complete **end-to-end data analytics workflow**, from raw data preparation to business insights and visualization.

By combining **Python, SQL, Power BI, and AI-assisted reporting**, the project shows how raw customer data can be transformed into clear and actionable business information.

---

## 👤 Author

Sumit chauhan


Skills: Python | SQL | Pandas | NumPy | Power BI | Data Visualization | Excel

---

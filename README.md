# Customer Shopping Behaviour Analysis

## Overview
This project analyzes customer shopping behavior using a complete data analytics workflow.  
It covers loading and exploring the dataset in Python, cleaning and preparing the data, running analytical SQL queries in PostgreSQL/SQL Server, and visualizing insights through a Power BI dashboard.

The goal is to understand key customer trends such as spending behavior, product performance, discount usage, and demographic patterns.

---

## Dataset
The dataset "Customer_behaviour_raw.csv" has 3900 rows and 18 columns and it includes customer purchase details such as:

- Customer demographics (age, gender, age group)  
- Purchase details (item, category, amount, discount status)  
- Shipping preferences  
- Review ratings  
- Purchase frequency and subscription information  
- Previous purchases  

These fields enable both behavioral and business-level insights.

---

## Tools and Technologies
- Python (Pandas, NumPy, Matplotlib) — Data loading, EDA and cleaning  
- PostgreSQL / SQL Server — Querying cleaned data and answering business questions  
- Power BI — Building the dashboard and final visualizations  
- Jupyter Notebook — Documentation of steps and EDA  
- SQL Queries File: `customer_behavior.sql`  
- Notebook: `Customer_Shopping_Behaviour.ipynb`

---

## Project Steps

### 1. Data Loading (Python)
- Loaded the dataset using Pandas  
- Inspected structure (head, info, shape)

### 2. Exploratory Data Analysis
- Generated summary statistics for numerical and categorical fields  
- Analyzed distributions such as age, spending, and ratings  
- Checked missing values  
- Explored unique values for product, category, shipping type, etc.

### 3. Data Cleaning
- Imputed missing Review Rating using median by category  
- Standardized column names  
- Handled inconsistent or incorrect formats  
- Created new fields like Age Group and purchase frequency  
- Removed or treated outliers as needed

### 4. SQL Analysis (PostgreSQL / SQL Server)
Conducted multiple business-oriented queries, including:

- Revenue analysis by gender  
- Identifying discount users spending above average  
- Finding highest-rated products  
- Comparing purchase amounts between Standard and Express shipping  
- Subscriber vs non-subscriber spending and revenue  
- Products with highest discount usage  
- Customer segmentation into New, Returning, and Loyal groups  
- Relationship between repeat buyers and subscription  
- Revenue contribution by age group  

All queries are included in `customer_behavior.sql`.

---

## Dashboard (Power BI)
The Power BI dashboard displays:

- Total revenue and key KPIs  
- Top products and category performance  
- Customer segmentation and demographic trends  
- Revenue breakdown by discount usage, shipping type, and subscription status  
- Spending behavior across age groups  

These visualizations present actionable business insights.

<img width="1150" height="628" alt="image" src="https://github.com/user-attachments/assets/cf712c64-cbfa-4227-9cae-dc8c6dea146c" />


---

## Results and Insights
Key outcomes from the analysis include:

- Spending varies significantly across demographic segments  
- Discount usage does not always indicate low spending  
- Certain categories contain top-rated, high-demand products  
- Subscribers tend to spend more on average  
- Discount-heavy products contribute differently across categories  
- Loyal customers account for a substantial share of revenue  

---

## How to Run This Project

### 1. Clone the Repository
```bash
git clone <[repository-link](https://github.com/Priths264/customer_behaviour.git)>
cd <customer_behaviour>

### 2. Run the Python Notebook
- Open `Customer_Shopping_Behaviour.ipynb` using Jupyter Notebook or VS Code.

### 3. Load SQL into PostgreSQL / SQL Server
- Import the cleaned dataset into your database.
- Execute the queries in `customer_behavior.sql`.

### 4. Open the Power BI Dashboard
- Open the `.pbix` file in Power BI Desktop.
- Refresh the data source if required.
- Explore the interactive charts and insights.


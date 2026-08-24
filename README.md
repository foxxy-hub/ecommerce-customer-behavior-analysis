# E-Commerce Customer Behavior & Sales Analysis

## Project Overview

This project performs Exploratory Data Analysis (EDA) on an e-commerce customer behavior dataset containing 5,000 transactions.

The analysis explores sales performance, customer behavior, device usage, website engagement, discounts, delivery time, and customer satisfaction using Python.

The main goal was to transform raw transactional data into meaningful business-oriented insights.

## Dataset

* **Rows:** 5,000
* **Original Columns:** 18
* **Time Period:** 2023–2024
* **Missing Values:** None
* **Duplicate Rows:** None

### Main Features

* Order ID
* Customer ID
* Date
* Age
* Gender
* City
* Product Category
* Unit Price
* Quantity
* Discount Amount
* Total Amount
* Payment Method
* Device Type
* Session Duration
* Pages Viewed
* Returning Customer
* Delivery Time
* Customer Rating

## Tools & Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

## Project Workflow

### 1. Data Understanding

The dataset was explored using Pandas methods including:

* `head()`
* `tail()`
* `shape`
* `columns`
* `info()`
* `describe()`
* `value_counts()`

### 2. Data Quality Checks

The dataset was checked for:

* Missing values
* Duplicate records
* Data types
* Invalid numerical values
* Categorical values

No missing values or duplicate rows were identified.

The `Date` column was converted from object/string format to datetime format for time-based analysis.

### 3. Feature Engineering

The following features were created from the transaction date:

* Year
* Month
* Month Name

Customer age groups were also created for customer-segment analysis.

### 4. Sales Analysis

The analysis calculated:

* Total revenue
* Average transaction value
* Median transaction value
* Revenue by product category
* Quantity sold by product category
* Revenue by device type

### 5. Customer Behavior Analysis

The project compared:

* Returning vs. non-returning customers
* Average transaction values
* Average quantities purchased
* Device-level purchasing behavior
* Age-group purchasing behavior

### 6. Correlation Analysis

Correlation analysis was used to investigate relationships between:

* Unit Price
* Quantity
* Discount Amount
* Total Amount
* Session Duration
* Pages Viewed
* Delivery Time
* Customer Rating

## Key Findings

### Overall Sales

The dataset generated a total transaction value of **4,915,544.57**, with an average transaction value of **983.11** and a median transaction value of **337.91**.

The difference between the mean and median indicates that transaction values are distributed unevenly, with larger transactions influencing the average.

### Product Performance

Electronics was the strongest revenue-generating category with **2,328,806.81** in total revenue, representing approximately **47% of overall transaction value**.

Sports recorded the highest quantity sold with **1,519 units**, demonstrating that the category with the highest sales volume was not the same as the category generating the highest revenue.

### Returning Customers

Returning customers accounted for **2,990 transactions**, compared with **2,010 transactions** from non-returning customers.

The average transaction value was **985.96** for returning customers and **978.87** for non-returning customers, showing only a small difference in average spending.

### Device Performance

Mobile users generated **2,810,468.64** in transaction value across **2,795 transactions**, making mobile the strongest device category.

Mobile also had the highest average transaction value at approximately **1,005.53**, suggesting that mobile shopping represents an important part of the dataset's sales activity.

### Customer Engagement

Session duration showed almost no linear correlation with transaction value (**r = -0.004**).

Pages viewed also showed a negligible correlation with transaction value (**r = -0.012**).

This suggests that longer browsing activity alone was not strongly associated with higher transaction values in this dataset.

### Delivery & Customer Rating

Delivery time and customer rating showed an almost zero linear correlation (**r = -0.010**).

Therefore, this dataset does not provide evidence of a meaningful linear relationship between delivery duration and customer rating.

### Correlation Analysis

Unit price had the strongest relationship with total transaction value (**r = 0.791**).

Quantity showed a weaker positive relationship with total transaction value (**r = 0.329**).

Discount amount also showed a moderate positive relationship with total transaction value (**r = 0.348**).

Correlation should be interpreted as association rather than causation.

## Visualizations

The project includes visualizations for:

* Revenue by Product Category
* Monthly Revenue
* Returning vs. Non-returning Customers
* Revenue by Device Type
* Delivery Time vs. Customer Rating
* Session Duration vs. Total Spending
* Correlation Heatmap

## Key Learning Outcomes

Through this project, I practiced:

* Data loading with Pandas
* Data exploration
* Data cleaning and validation
* Datetime conversion
* Feature engineering
* GroupBy analysis
* Aggregation
* Statistical analysis
* Correlation analysis
* Data visualization
* Business-oriented interpretation

## Future Improvements

Possible next steps include:

* Building an interactive Power BI dashboard
* Performing statistical hypothesis testing
* Customer segmentation using clustering
* Developing predictive models
* Exploring customer lifetime value
* Creating an interactive sales dashboard

## Project Structure

```text
ecommerce-customer-behavior-analysis/
│
├── data/
│   └── ecommerce_cleaned.csv
│
├── images/
│   ├── revenue_by_category.png
│   ├── monthly_revenue.png
│   ├── customer_type.png
│   ├── device_revenue.png
│   ├── delivery_vs_rating.png
│   └── correlation_heatmap.png
│
├── ecommerce_analysis.ipynb
│
└── README.md
```

## Author

**Shafaat Zaman Khattak**

Data Science Student | Python | Data Analysis | Machine Learning


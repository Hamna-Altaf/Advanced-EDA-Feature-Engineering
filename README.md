# Advanced-EDA-Feature-Engineering

## Project Overview

This project is a part of my Data Science Virtual Internship with DecodeLabs.

The goal was to clean the raw dataset collected from the e-commerce website, preprocess it, prepare features and encode them into a machine learning-ready dataset through Exploratory Data Analysis (EDA), data preprocessing, feature engineering and categorical encoding.

---

## Objectives

Conduct Exploratory Data Analysis (EDA)
Deal with missing values appropriately using statistical techniques.
Identify and explain outliers using IQR method
- Develop new predictive capabilities
- Determine feature interactions and collinearity
Use One Hot Encoding for categorical variables
- Make predictions for future machine learning models

---

## Dataset

This data set includes information about e-commerce orders such as:

- Order ID
- Customer ID
- Product
- Quantity
- Unit Price
- Total Price
- Payment Method
- Coupon Code
- Referral Source
- Order Status
- Shipping Address
- Tracking Number

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Project Workflow

### 1. Data Loading & Exploration

- Used Pandas to load the data
- Examined data types
- Checked missing values
- Explored numerical and categorical variables

### 2. Missing Value Handling

Detected Data Integrity Errors on ‘CouponCode' column
- Missing values were filled with customers who didn't use a coupon
Filled in missing values with `"No Coupon"` to maintain the business meaning

### 3. Outlier Analysis

- Applied the Interquartile Range (IQR) method
Identified extreme values from the "TotalPrice" column
- Identified outlier values as valid high-value purchases and not data errors

### 4. Feature Engineering

Developed three new features:

OrderMonth – Derived from the order date.

CouponUsed – If a coupon has been used or not

IsWeekendOrder - returns True if an order was placed on a weekend, False if it was not placed on a weekend.

### 5. Correlation Analysis

Calculated and generated a correlation matrix.
- Checked for multicollinearity
- Verified no feature-pairs with correlation>0.9

### 6. One-Hot Encoding

Applied OHE to:

- Product
- PaymentMethod
- OrderStatus
- ReferralSource

Avoid dummy variable trap by using drop_first=True.

---

## Project Files

```
├── eda.ipynb
├── Cleaned_Dataset.csv
├── Encoded_Dataset.csv
├── report.pdf
└── README.md
```

---

## Key Skills Demonstrated

Exploratory Data Analysis (EDA)
- Data Cleaning
- Missing Value Treatment
- Outlier Detection
- Feature Engineering
- Correlation Analysis
- One-Hot Encoding
- Data Preprocessing
- Python Programming
- Pandas & NumPy

---

## Author

Hamna Altaf
Software Engineering Student

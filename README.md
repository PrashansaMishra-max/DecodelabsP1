# 📊 DecodeLabs Data Analytics Project

## 📌 Overview

This project is part of the DecodeLabs Data Analytics Assignment. It focuses on cleaning, preprocessing, exploring, and analyzing an e-commerce dataset using Python. The project demonstrates essential data analytics techniques such as data cleaning, missing value treatment, outlier detection, feature engineering, and exploratory data analysis (EDA) to derive meaningful business insights.



## 🎯 Objectives

- Perform data cleaning and preprocessing.
- Handle missing values appropriately.
- Detect and analyze outliers using the IQR method.
- Create new features through feature engineering.
- Perform Exploratory Data Analysis (EDA).
- Generate meaningful business insights from the dataset.
- Export the cleaned dataset for future analysis.



## 📂 Project Structure

```
DecodelabsP1/
│
├── cleaned_data/
│   └── cleaned_dataset.csv
│
├── data/
│   └── dataset.xlsx
│
├── notebooks/
│   └── project1.ipynb
│
├── images/
│
├── src/
│
├── requirements.txt
├── README.md
└── .gitignore
```



## 📁 Dataset Description

The dataset contains **1,200 e-commerce orders** with information including:

- Order ID
- Order Date
- Customer ID
- Product
- Quantity
- Unit Price
- Shipping Address
- Payment Method
- Order Status
- Tracking Number
- Items in Cart
- Coupon Code
- Referral Source
- Total Price



## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook



## 📈 Data Cleaning

The following preprocessing steps were performed:

- Checked dataset structure and data types.
- Identified missing values.
- Filled missing values in the `CouponCode` column with **"No Coupon"**.
- Checked for duplicate records.
- Verified data types.
- Exported the cleaned dataset.



## 📊 Outlier Detection

Outliers were detected using the **Interquartile Range (IQR)** method.

### Results

| Column | Outliers |
|---------|----------|
| Quantity | 0 |
| UnitPrice | 0 |
| ItemsInCart | 0 |
| TotalPrice | 8 |

The detected outliers in `TotalPrice` were retained because they represent genuine high-value customer purchases rather than data errors.



## ⚙️ Feature Engineering

The following new features were created:

- **CouponUsed**
- **OrderValueCategory**
- **AveragePricePerItem**
- **CartEfficiency**

These engineered features help improve business analysis and provide additional insights into customer purchasing behavior.



## 📉 Exploratory Data Analysis (EDA)

The notebook includes visualizations for:

- Product Distribution
- Order Status Distribution
- Payment Method Analysis
- Referral Source Analysis
- Quantity Distribution
- Unit Price Distribution
- Total Price Distribution
- Coupon Usage
- Order Value Categories
- Correlation Heatmap



## 💡 Key Business Insights

- The dataset contains 1,200 customer orders.
- Only the `CouponCode` column contained missing values, which were handled successfully.
- No duplicate records were found.
- Only the `TotalPrice` column contained a small number of outliers.
- Feature engineering provided additional insights into customer purchasing behavior.
- EDA helped identify customer preferences, payment trends, referral sources, and order value patterns.



## 🚀 How to Run

### 1. Clone the repository

```bash
git clone <repository-url>
```

### 2. Move into the project directory

```bash
cd DecodelabsP1
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

### 5. Open

```
notebooks/project1.ipynb
```



## 📦 Output

The cleaned dataset is available in:

```
cleaned_data/cleaned_dataset.csv
```



## 👩‍💻 Author

**Prashansa Mishra**

B.Tech Computer Science Engineering (2027)

Passionate about Data Analytics, Machine Learning, and Full-Stack Development.



## ⭐ Acknowledgement

This project was completed as part of the **DecodeLabs Data Analytics Assignment** to demonstrate practical skills in data preprocessing, feature engineering, and exploratory data analysis using Python.
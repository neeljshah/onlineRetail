# 🛍️ Online Retail Data Analysis

This project provides a comprehensive **analysis of the Online Retail Dataset**, focusing on **data cleaning**, **feature engineering**, and **exploratory data analysis (EDA)**. The goal is to uncover actionable insights related to sales trends, customer behavior, and product performance.

---

## 1. Data Cleaning and Preprocessing

The raw dataset contains inconsistencies such as missing values, duplicate entries, and invalid transactions. This step ensures the data is clean and reliable for analysis.

### Cleaning Steps:
- **Remove Duplicates:** Dropped duplicate records to avoid data redundancy.  
- **Handle Missing Values:**  
  - Dropped rows missing `CustomerID`.  
  - Filled missing product `Description` with `"Unknown"`.  
- **Filter Invalid Transactions:**  
  - Removed transactions with negative or zero `Quantity` and `UnitPrice`.  
- **Datetime Conversion:** Converted `InvoiceDate` to a datetime format for time-series analysis.  
- **New Feature:** Created `TotalPrice` = `Quantity * UnitPrice`.  

### Expected Outcome:
- A clean and consistent dataset ready for analysis.  
- Enhanced features for better insights.

### 📊 **Visualization 1:** Data Cleaning Summary  
![Figure_4](https://github.com/user-attachments/assets/869df959-de12-4f3e-b2db-3f40da5b4dd3)

---

## 2. Feature Engineering

New features were created to extract more insights and improve analysis.

### Engineered Features:
- **Total Transaction Amount (`TotalPrice`):** Multiplication of `Quantity` and `UnitPrice`.  
- **Date-Time Features:** Extracted `Month`, `Day`, `Hour`, and `Weekday` from `InvoiceDate`.  
- **Holiday Purchases:** Flagged transactions made on holidays.  
- **RFM Analysis:**  
  - **Recency:** Days since the last purchase.  
  - **Frequency:** Number of purchases.  
  - **Monetary:** Total spend.  

### Expected Outcome:
- New features that provide a deeper understanding of sales trends and customer behavior.

### 📊 **Visualization 2:** Monthly Sales Trend  
![Figure_1](https://github.com/user-attachments/assets/acea709e-e09e-43c0-8b47-cd8e0a093a9e)

---

## 3. Exploratory Data Analysis (EDA)

EDA helps to visualize and understand sales patterns, customer behavior, and product performance.

### Key Insights:
- **Monthly Sales Trends:** Identified peak sales months.  
- **Top 10 Best-Selling Products:** Highlighted products driving revenue.  
- **Geographic Sales Distribution:** Identified top-performing countries.  
- **RFM Analysis:** Segmented customers based on purchasing behavior.  

### Expected Outcome:
- Actionable insights into sales performance and customer segments.  
- Visual understanding of product and customer behavior.

### 📊 **Visualization 3:** Top 10 Best-Selling Products  
![Figure_2](https://github.com/user-attachments/assets/12adc2ab-74dd-4e90-b0ca-c2e5a38bdb2f)
![Figure_3](https://github.com/user-attachments/assets/49446a8a-1039-4df7-8e3d-a24b34aac0c3)


---

## 4. How to Run

1. **Clone** this repository.

   ```bash
   git clone https://github.com/yourusername/online-retail-analysis.git
   cd online-retail-analysis

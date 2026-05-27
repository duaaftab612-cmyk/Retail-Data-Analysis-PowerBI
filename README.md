# 📊 Retail Data Analysis using Power BI

## 📌 Project Overview

This project is based on a real-world retail data analysis scenario. After completing the data cleaning process, the dataset was enhanced by creating meaningful categories and key performance metrics to analyze business performance and ensure data accuracy.

---

## 🎯 Objectives

* Categorize sales into High and Low
* Identify discount usage in transactions
* Calculate key business metrics
* Validate results using reporting visuals

---

## 🛠️ Tools & Technologies

* Power BI
* DAX (Data Analysis Expressions)
* Microsoft Excel

---

## 📂 Dataset

The dataset contains 100 rows of retail sales data including:

* Order ID
* Sales
* Quantity
* Discount
* Profit

---

## 🔹 Calculated Columns

### 1. Sales Category

Classifies sales into High and Low:

```DAX
Sales Category = IF('Table'[Sales] > 100, "High", "Low")
```

### 2. Discount Category

Classifies discount usage:

```DAX
Discount Category = IF('Table'[Discount] = 0, "No Discount", "Discount Applied")
```

---

## 🔹 Calculated Measures

### Total Sales

```DAX
Total Sales = SUM('Table'[Sales])
```

### Quantity Sold

```DAX
Qty Sold = SUM('Table'[Quantity])
```

### Total Orders

```DAX
Total Orders = COUNT('Table'[Order ID])
```

### Total Profit (Using Iterator Function)

```DAX
Total Profit = SUMX('Table', 'Table'[Quantity] * 'Table'[Profit])
```

---

## ✅ Validation

All calculated measures were validated using a **Matrix Visual** in Power BI to ensure accuracy and consistency of results.

---


## 💡 Key Learnings

* Practical use of DAX formulas
* Data categorization and transformation
* Business performance analysis
* Data validation using visuals

---

## 🚀 Conclusion

This project demonstrates how raw data can be transformed into meaningful insights using Power BI and DAX, helping businesses make better decisions.

---

## 🔗 Author

**Dua Aftab**
BS Information Technology Student | Aspiring Data Analyst

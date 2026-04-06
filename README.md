# zepto_SQL_project
# 🛒 Zepto Product Data Analysis (SQL Project)

## 📌 Overview
This project focuses on analyzing a product dataset inspired by Zepto, a fast-growing quick-commerce platform that delivers groceries in minutes. The dataset contains 3,000+ products (SKUs) across multiple categories such as Fruits & Vegetables, Dairy, Beverages, and Packaged Foods.

The objective is to perform **data cleaning, exploration, and analysis using SQL** to extract meaningful business insights related to pricing, discounts, and inventory.

---

## 📂 Dataset Description
The dataset includes the following columns:

- `sku_id` – Unique product ID  
- `category` – Product category  
- `name` – Product name  
- `mrp` – Maximum Retail Price  
- `discountPercent` – Discount percentage  
- `discountedSellingPrice` – Final selling price  
- `availableQuantity` – Available stock quantity  
- `weightInGms` – Product weight (grams)  
- `outOfStock` – Stock status (TRUE/FALSE)  
- `quantity` – Units per product  

---

## 🎯 Objectives
- Analyze discount trends across categories  
- Identify best-value and highly discounted products  
- Evaluate inventory availability and stock-outs  
- Understand pricing strategies  
- Generate category-level insights  

---

## 🧹 Data Cleaning
- Removed rows with invalid pricing (`mrp = 0`)  
- Converted prices from paise to rupees  
- Checked for NULL values  
- Identified duplicate product entries  

---

## 🔍 Key Analysis

### 1. Top Discounted Products
Identified top 10 products with highest discount percentages.

### 2. High MRP but Out of Stock
Found expensive products that are currently unavailable.

### 3. Estimated Revenue by Category
Calculated total revenue using:
```sql
SUM(discountedSellingPrice * availableQuantity)4. Premium Low-Discount Products

Products with MRP > ₹500 and discount < 10%.

5. Category-wise Discounts

Top 5 categories with highest average discounts.

6. Price per Gram Analysis

Identified best-value products using:

discountedSellingPrice / weightInGms
7. Product Segmentation

Grouped products into:

Low (< 1kg)
Medium (1kg – 5kg)
Bulk (> 5kg)
8. Inventory Weight by Category

Calculated total inventory weight per category.

📊 Insights
Certain categories consistently offer higher discounts
High-priced products are often out of stock
Price-per-gram helps identify cost-efficient products
Inventory distribution varies across categories
🛠️ Tech Stack
SQL (MySQL)
MySQL Workbench
GitHub

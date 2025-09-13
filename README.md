# 🍽️ Restaurant Order Analysis  

![SQL](https://img.shields.io/badge/SQL-MySQL-blue)  
![Data Analysis](https://img.shields.io/badge/Focus-Data%20Analysis-brightgreen)  
![Status](https://img.shields.io/badge/Status-Completed-success)  

## 📌 Overview  
This project analyzes restaurant order data using **SQL**. By exploring two key tables — `menu_items` and `order_details` — the goal is to understand pricing, customer purchasing patterns, and high-value orders.  

The insights can help restaurants make data-driven decisions about menu optimization, pricing strategies, and peak order management.  

---

## 🗂️ Project Structure  

The repository contains three main SQL scripts:

1. **`menu_items_query.sql`**  
   Focused on analyzing the `menu_items` table:
   - Count of items on the menu  
   - Least & most expensive dishes overall and by category  
   - Number of dishes in each category  
   - Average dish price by category  

2. **`order_details_query.sql`**  
   Focused on analyzing the `order_details` table:
   - Date range of the dataset  
   - Total number of unique orders & items ordered  
   - Orders with the highest number of items  
   - Orders with more than 12 items  

3. **`joined_table_query.sql`**  
   Combines both tables to explore customer behavior:
   - Item popularity by category  
   - Top 5 orders with the highest spend  
   - Breakdown of items in the single highest-spend order  
   - Category distribution in the top 5 highest-spend orders  

---

## 🛠️ Data Schema  

**menu_items**  
- `menu_item_id` (PK)  
- `item_name`  
- `category`  
- `price`  

**order_details**  
- `order_details_id` (PK)  
- `order_id`  
- `order_date`  
- `item_id` (FK → menu_items.menu_item_id)  

---

## 🔍 Key Insights  

- Identified the **least and most expensive dishes** on the menu, both overall and within cuisines (e.g., Italian).  
- Determined the **date range** of the dataset and total orders placed.  
- Found orders with **12+ items**, representing unusually large group purchases.  
- Ranked the **top 5 spending orders**, with Order ID `440` being the highest spender, containing multiple categories.  
- Analyzed **most popular items and categories**, uncovering customer favorites.  

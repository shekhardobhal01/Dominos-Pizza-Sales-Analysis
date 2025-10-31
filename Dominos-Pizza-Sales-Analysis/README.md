
# 🍕 Domino’s Pizza Sales Analysis (Power BI Dashboard)

### 👨‍💻 Created by [Shekhar Dobhal](www.linkedin.com/in/shekhar001)

---

## 📊 Project Overview
This Power BI project provides a comprehensive analysis of Domino’s Pizza sales data for the year 2024.  
The goal is to derive actionable insights into sales performance, customer behavior, and business trends.

### 🎯 Objectives
- Analyze total revenue and monthly sales performance  
- Identify best-selling pizzas and their categories  
- Evaluate weekday vs weekend performance  
- Find peak sales hours and customer ordering patterns  

---

## 🧰 Tools & Technologies Used
- **Power BI Desktop** – Dashboard design and visualization  
- **Power Query** – Data cleaning and transformation  
- **DAX (Data Analysis Expressions)** – Measures and calculations  
- **CSV Dataset** – Raw data source  

---

## 📂 Dataset Description
The dataset contains detailed pizza order records with the following fields:

| Column Name | Description |
|--------------|-------------|
| `pizza_id` | Unique ID for each pizza |
| `order_id` | Order number identifier |
| `pizza_name_id` | Combined pizza name key |
| `quantity` | Quantity sold per order |
| `order_date` | Date of order |
| `order_time` | Time of order |
| `price` | Price of each pizza |
| `pizza_category` | Category (Classic, Supreme, Veggie, Chicken) |
| `pizza_ingredients` | Ingredients used |
| `pizza_name` | Full pizza name |

---

## ⚙️ DAX Measures Used

```DAX
Total Revenue = SUMX(Dataset, Dataset[quantity] * Dataset[price])
Total Orders = DISTINCTCOUNT(Dataset[order_id])
Total Quantity Sold = SUM(Dataset[quantity])
Average Order Value = DIVIDE([Total Revenue], [Total Orders])
Peak Hour = MAXX(FILTER(SalesByHour, [Total Revenue] = MAX([Total Revenue])), [Hour])
```

---

## 📈 Dashboard Insights

**Key Metrics**
- Total Revenue: ₹24.54M  
- Total Orders: 21K  
- Average Order Value: ₹1.15K  
- Total Quantity Sold: 50K  
- Peak Hour: 12 PM  

**Visuals Included**
- KPI Cards (Revenue, Orders, Quantity, AOV, Peak Hour)  
- Monthly Sales Trends  
- Hourly Order Distribution  
- Weekday vs Weekend Comparison  
- Sales by Category and Pizza Name  

---

## 💡 Insights & Business Takeaways
- Weekdays outperform weekends in total sales (₹18M vs ₹7M).  
- Peak demand occurs during lunch hours (11 AM – 2 PM).  
- “Classic” pizzas are top revenue generators.  
- “Thai Chicken” is the best-selling pizza overall.  
- Sales drop during September–October, indicating seasonal variation.  

---

## 🧩 Project Files
| File | Description |
|------|--------------|
| `Dataset.csv` | Raw sales data |
| `dominos_complete.pbix` | Power BI dashboard file |
| `Dominos_Pizza_Sales_Analysis_2024.pptx` | Presentation file |
| `dashboard_preview.png` | Dashboard snapshot |
| `Project_Report.pdf` | Summary document (optional) |

---

## 🚀 How to Use
1. Download the `.pbix` file and open in **Power BI Desktop**  
2. Load the provided `Dataset.csv` file if prompted  
3. Explore visuals, filters, and slicers interactively  

---

## 🌐 Connect With Me
📄 [LinkedIn – Shekhar Dobhal](www.linkedin.com/in/shekhar001)  
🐙 [GitHub – Coming Soon!](https://github.com/)  

---

⭐ **If you like this project, don’t forget to star the repository!**

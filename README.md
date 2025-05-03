# Power_BI_-AdventureWorks-Sales-Performance-Dashboard
Designed an interactive Power BI dashboard for AdventureWorks, analyzing 25K+ orders across $24M+ revenue. Performed data cleaning, transformation, and modeled a star schema with Sales, Customer, Product, and Calendar tables.

![Image](https://github.com/user-attachments/assets/719b875b-7dac-4747-926e-d8b102caac23)

![Image](https://github.com/user-attachments/assets/f1dbfd41-a4ba-44e5-9a14-a2bf0878a983)

![Image](https://github.com/user-attachments/assets/bd458fff-7eaa-4a93-9071-bf1be5fa6d21)

![Image](https://github.com/user-attachments/assets/1269d7f4-b677-4cc0-8970-cfb0deb29038)

Sure — here’s a clean, structured **Project Report** based on your Power BI AdventureWorks project:

---

## 📊 **AdventureWorks Sales Analysis — Project Report**

### **Project Overview**

This project involved analyzing sales, customer, and product performance data for **AdventureWorks**, a global e-commerce business dealing in bicycles, accessories, and clothing. The goal was to uncover insights about revenue trends, profitability, customer segmentation, and product performance using **Power BI** dashboards and reports.

---

### **Objectives**

* Track and visualize **total revenue**, **profit**, **orders**, and **returns**.
* Compare monthly sales performance against set targets.
* Identify the top-performing products and customers.
* Analyze customer orders by **income level** and **occupation**.
* Highlight sales trends over time and across different product categories.
* Provide actionable insights to support business decisions.

---

### **Data Sources**

* **Sales Data**
* **Product Data**
* **Customer Information**
* **Calendar Lookup Table**

---

### **Key Metrics**

| Metric                       | Value    |
| :--------------------------- | :------- |
| **Total Revenue**            | $ 24.91M |
| **Total Profit**             | $ 10M    |
| **Total Orders**             | 25,164   |
| **Total Returns**            | 1,809    |
| **Return Rate**              | 2.17%    |
| **Unique Customers**         | 17,000   |
| **Avg Revenue per Customer** | $ 1,431  |

---

### **Data Model Design**

* **Star Schema** implemented:

  * **Fact Table:** Sales transactions
  * **Dimension Tables:** Product, Customer, Calendar
* Related using primary keys (e.g., CustomerKey, ProductKey)
* Optimized for performance in **Power BI**

---

### **Key Dashboards and Visualizations**

1. **Revenue Trend Chart**

   * Monthly revenue trend from Jan 2020 to Jan 2022.
   * Highlighted growth phases and dips.

2. **Orders by Category**

   * Top product categories: **Accessories, Bikes, Clothing**
   * Highest number of orders in Accessories.

3. **Top 10 Products**

   * Metrics: Total Orders, Revenue, Return Rate
   * Example: *Water Bottle - 30 oz.* was the most ordered product.

4. **Performance vs Targets**

   * Revenue, Profit, and Orders compared against monthly targets using:

     * Gauges
     * Conditional formatting (Green/Red indicators based on gap to target)

5. **Customer Segmentation**

   * Orders by **Income Level** and **Occupation**
   * Top 30 Customers ranked by Revenue.

6. **Return Analysis**

   * Products with highest and lowest return rates.

---

### **Key Insights**

* **Tires & Tubes** were the most frequently ordered product type.
* **Shorts** had the highest return rate.
* Revenue consistently grew, with significant spikes in early 2021.
* Top customer **Mr. Maurice Shan** contributed ₹12.41K in revenue from 6 orders.
* Management and Skilled Manual occupations placed the most orders.

---

### **DAX Measures Implemented**

* `Total Revenue`
* `Total Profit`
* `Return Rate`
* `Previous Month Revenue`
* `90-day Rolling Profit`
* `Orders vs Target Gap`
* `Previous Year Orders`
* `Average Revenue per Customer`

---

### **Challenges Faced**

* Correct alignment of **Previous Year / Previous Month values** using `DATEADD()`
* Fixing gauge visual inaccuracies by adjusting filters and measure context.
* Managing **conditional formatting rules** for KPI indicators based on dynamic min/max values.

---




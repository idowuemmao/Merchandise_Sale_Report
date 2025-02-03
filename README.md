# **Merchandise Sales Analysis Report**  
### **Project Description**  

## **1. Project Overview**  
Lee Chatmen, a well-known influencer with over 7 million TikTok followers, launched his own line of merchandise in 2023. This Power BI report provides a **comprehensive analysis** of his merchandise sales, helping to identify trends, customer behavior, and key insights that drive business decisions.  

The report is structured to be **intuitive, interactive, and insightful**, allowing stakeholders to explore the data and derive meaningful conclusions regarding sales performance, customer demographics, product popularity, and shipping impact.  

---

## **2. Objectives**  
The primary objectives of this report are:  
✅ **Analyze overall sales trends** to identify growth patterns and seasonality.  
✅ **Identify best-performing product categories** and the most and least popular products.  
✅ **Understand geographical impact on sales** by analyzing location-based performance.  
✅ **Evaluate the influence of international shipping** on total revenue and cost structure.  
✅ **Assess buyer demographics** (age, gender) to understand customer segmentation.  
✅ **Examine the correlation between ratings, reviews, and sales performance.**  
✅ **Analyze trends in shipping charges** to optimize logistics and pricing strategies.  
✅ **Evaluate the impact of discounts and promotions** on purchasing behavior.  
✅ **Identify patterns in repeat purchases** for customer retention strategies.  

---

## **3. Data Sources & Structure**  
The dataset includes the following columns:  

| **Column Name**         | **Description** |
|-------------------------|---------------|
| Order ID               | Unique identifier for each purchase. |
| Order Date            | Date when the order was placed. |
| Product ID            | Unique identifier for each product. |
| Product Category      | Category of the product (Clothing, Ornaments, Other). |
| Buyer Gender         | Gender of the customer (Male, Female). |
| Buyer Age            | Age of the customer. |
| Order Location       | City from which the order was placed. |
| Latitude / Longitude | Geographical coordinates of the order location. |
| International Shipping | Indicates if the product was shipped internationally (Yes/No). |
| Sales Price          | Price per unit of the product. |
| Shipping Charges     | Extra charges for international shipments. |
| Sales per Unit       | Sales value including shipping charges. |
| Quantity            | Number of units purchased. |
| Total Sales         | Total revenue from the purchase. |
| Rating             | Customer rating for the product. |
| Review             | Customer review text. |

---

## **4. Report Structure & Pages**  
The report is divided into multiple pages, each focusing on different aspects of sales analysis.  

### **📌 Page 1: Executive Summary (Key Insights & KPIs)**  
**📊 Visuals:**  
- **KPI Cards**: Total Sales, Total Quantity Sold, Average Rating, Total Orders, Total Product, Average Age.
- **Map**: Sales Breakdown by Location.  
- **Column Chart**: Sales Trends over Time (Monthly).  
- **Pie Chart**: Sales Breakdown by Product Category.
- **Pie Chart**: Sales Breakdown by Gender.
- **Clustered Column Chart**: Sales and Quantity Breakdown by Product Category.  

**🔎 Key Insights:**  
- How is overall sales performance?  
- What are the highest and lowest selling product categories?
- Gender with the highest total sales

---

### **📌 Page 2: Product Performance Analysis**  
**📊 Visuals:**  
- **Column Chart**: Top 5 Best-Selling Products and bottom 5 selling products.  
- **Bar Chart**: Total Shipping Charges by Product Category and Product ID.  
- **Bar Chart**: Top 7 reviews with the highest no of orders.  
- **Matrix**: Total Product per Ratings in all locations

**🔎 Key Insights:**  
- Which products are driving the most revenue?  
- Are there products that should be discontinued or improved?  

---

### **📌 Page 3: Shipping Analysis**  
**📊 Visuals:**  
- **Map Visual**: Sales distribution across locations (using Latitude & Longitude).  
- **Bar Chart**: Sales by Country/City.  
- **Heatmap**: International vs. Domestic Sales Comparison.  

**🔎 Key Insights:**  
- Which locations contribute the most sales?  
- How does international shipping impact revenue?  

---

### **📌 Page 4: Customer Demographics & Behavior**  
**📊 Visuals:**  
- **Bar Chart**: Sales by Buyer Age Group.  
- **Pie Chart**: Sales by Buyer Gender.  
- **Stacked Column Chart**: Product Category vs. Gender.  
- **Line Chart**: Repeat Purchases Over Time.  

**🔎 Key Insights:**  
- What age group buys the most merchandise?  
- Are there gender-based buying preferences?  
- Do repeat customers show loyalty to specific products?  

---

### **📌 Page 5: Sentiment Analysis (Reviews & Ratings)**  
**📊 Visuals:**  
- **Word Cloud**: Common Words in High-Rating Reviews.  
- **Word Cloud**: Common Words in Low-Rating Reviews.  
- **Bar Chart**: Ratings Distribution.  
- **Scatter Plot**: Correlation between Ratings & Total Sales.  

**🔎 Key Insights:**  
- What words are frequently used in positive and negative reviews?  
- Do higher ratings lead to more sales?  

---

### **📌 Page 6: Pricing, Promotions & Discounts Impact**  
**📊 Visuals:**  
- **Line Chart**: Sales Trends Before & After Promotions.  
- **Stacked Column Chart**: Discount Levels vs. Sales Impact.  
- **Bar Chart**: Sales Revenue by Discounted vs. Non-Discounted Items.  

**🔎 Key Insights:**  
- How effective are discounts and promotions?  
- Do discounts attract repeat customers or just one-time buyers?  

---

## **5. Technical Implementation & Custom Visuals**  
- **ZoomCharts Drill Down Visuals**: Used on at least one report page for interactive exploration.  
- **Power Query**: Data cleansing, transformation, and preparation.  
- **DAX Measures**:  
  - `Total Sales = SUM('TableName'[Total Sales])`  
  - `Previous Month Sales = CALCULATE(SUM('TableName'[Total Sales]), SAMEPERIODLASTMONTH('TableName'[Order Date]))`  
  - `Repeat Customers = DISTINCTCOUNT('TableName'[Order ID]) - DISTINCTCOUNTNOBLANK('TableName'[Buyer ID])`  

---

## **6. Judging Criteria & Success Factors**  
The report is evaluated based on:  

✅ **Intuitiveness (15 pts)**:  
- Clear layout, readable fonts, and appropriate chart selection.  
- Effective storytelling through visual hierarchy and colors.  

✅ **Interactivity (15 pts)**:  
- Dynamic slicers, drill-through, and drill-down capabilities.  
- Cross-chart filtering and touch-friendly navigation.  

✅ **Insightfulness (15 pts)**:  
- Meaningful KPIs and deep analytical insights.  
- Accurate data representation and performance optimization.  

---

## **7. Expected Outcome & Business Impact**  
📌 **Optimized Marketing & Product Strategy**: Identify best-sellers and optimize inventory.  
📌 **Improved Customer Experience**: Leverage reviews to improve product quality.  
📌 **Better Pricing & Discounting Decisions**: Analyze the impact of promotions.  
📌 **Stronger Geographic Expansion**: Focus on high-performing cities/countries.  

This report will enable **Lee Chatmen’s team** to make **data-driven decisions** to boost merchandise sales and improve customer satisfaction. 🚀  

---

Would you like any refinements or additional sections? 😊

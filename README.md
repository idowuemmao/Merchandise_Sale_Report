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
- **Column Chart**: Shipping charges by month.
- **Column Chart**: Total Sales and total quantity by Internation or local shipping.   
- **Scatter plot**:  Correlation between Ratings & Total Sales.  
- **Matrix**: Insight into the sales, purchase per location.  

**🔎 Key Insights:**  
- Which locations contribute the most sales?  
- How does international shipping impact revenue?  

---

## **5. Technical Implementation & Custom Visuals**  
- **ZoomCharts Drill Down Visuals**: Used on at least one report page for interactive exploration.  
- **Power Query**: Data cleansing, transformation, and preparation.  
- **DAX Measures**:  
  - `Avg Rating = AVERAGE(Data[Rating])`
  - `Average Age = AVERAGE(Data[Buyer Age])`
  - `Average Shipping Charges = AVERAGE(Data[Shipping Charges])`  
  - `Avg Price of Product = AVERAGE(Data[Sales Price])`
  - `No of Orders = DISTINCTCOUNT(Data[Order ID])`
  - `No of Product = DISTINCTCOUNT(Data[Product ID])`
  - `Previous Month Sales = CALCULATE([Total Sales], SAMEPERIODLASTYEAR(Data[Order Date]))`
  - `Total International Sales = CALCULATE([Total Sales], Data[International Shipping] = "Yes")`
  - `Total Local Sales = CALCULATE([Total Sales], Data[International Shipping] = "No")`
  - `Total Quantity = SUM(Data[Quantity])`
  - `Total Sales = SUM(Data[Total Sales])`
  - `Total Shipping Charges = SUM(Data[Shipping Charges])`

---

## **7. Expected Outcome & Business Impact**  
📌 **Optimized Marketing & Product Strategy**: Identify best-sellers and optimize inventory.  
📌 **Improved Customer Experience**: Leverage reviews to improve product quality.  
📌 **Better Pricing & Discounting Decisions**: Analyze the impact of promotions.  
📌 **Stronger Geographic Expansion**: Focus on high-performing cities/countries.  

This report will enable **Lee Chatmen’s team** to make **data-driven decisions** to boost merchandise sales and improve customer satisfaction. 🚀  

---


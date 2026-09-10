# 📦 Supply Chain & Inventory Analytics

### An End-to-End Data Analytics Project using Python & Power BI

**By Rishab Das**

---

## 📌 Project Overview

This project analyzes **30,000 supply chain transactions** to identify business insights related to sales, profitability, inventory management, suppliers, warehouses, delivery performance, and product quality.

The project follows an end-to-end analytics workflow:

**Data → Cleaning → Analysis → Business Insights → Power BI Dashboard**

---

## 🎯 Project Objectives

The main objectives of this project are to analyze:

- 📦 Inventory problems
- 📈 Product demand patterns
- 💰 Revenue and profitability
- 🚚 Supplier performance
- 🏭 Warehouse efficiency
- ⚠️ Stockout and overstock situations
- 🚛 Delivery performance
- 🛒 Order status
- 🧪 Product quality and defective units
- 🌎 Regional and category performance

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| **Python** | Data analysis and processing |
| **Pandas** | Data cleaning and manipulation |
| **NumPy** | Numerical analysis |
| **Matplotlib** | Data visualization |
| **Seaborn** | Statistical visualization |
| **Jupyter Notebook** | Analysis environment |
| **Power BI** | Interactive dashboard and business reporting |
| **Git & GitHub** | Version control and project sharing |

---

# 📊 Dataset

The dataset contains **30,000 transactions** and **20 original columns** covering orders, products, suppliers, warehouses, inventory, delivery, costs, and quality.

### Main Columns

```text
Order_ID
Order_Date
Product_ID
Product_Name
Category
Supplier_ID
Supplier_Name
Warehouse
Region
Quantity_Ordered
Quantity_Sold
Unit_Cost
Unit_Price
Inventory_Level
Reorder_Level
Lead_Time_Days
Delivery_Days
Order_Status
Shipping_Cost
Defective_Units
Order_Status
Shipping_Cost
Defective_Units
🔍 Data Analysis Process
1. Data Loading

The dataset was loaded into Python using Pandas.

2. Data Cleaning

The analysis includes:

Checking dataset dimensions
Checking data types
Checking missing values
Checking duplicate records
Converting order dates into datetime format
Creating analytical variables

The dataset contained missing values in Delivery_Days, while no duplicate records were identified.

3. Feature Engineering

Important business metrics were calculated.

Revenue
Revenue = Quantity_Sold × Unit_Price
Product Cost
Product_Cost = Quantity_Sold × Unit_Cost
Profit
Profit = Revenue - Product_Cost - Shipping_Cost
Profit Margin
Profit_Margin = (Profit / Revenue) × 100
Delivery Delay
Delivery_Delay = Delivery_Days - Lead_Time_Days
📦 Inventory Analysis

Inventory was classified into:

Stockout
Low Stock
Normal
Overstock

The analysis identified:

Inventory Metric	Result
Low Stock Records	6,081
Low Stock Rate	20.27%
Overstock Records	4,543
Stockout Records	0
Stockout Rate	0.00%

The project defines overstock as inventory greater than 3× the reorder level.

📈 Product Analysis

Product performance was analyzed using:

Quantity Sold
Revenue
Profit
Demand
Inventory levels
Top Products by Quantity Sold
Notebook Pack
USB-C Cable
Ball Pen Pack
Water Bottle
Wireless Mouse
Printer Paper
Desk Organizer
Backpack
Desk Lamp
Laptop Sleeve
Top Products by Revenue

The highest-revenue products include:

LED Monitor
Office Chair
Running Shoes
Backpack
Mechanical Keyboard
Desk Lamp
Study Table
Bluetooth Speaker
Power Bank
Bookshelf
💰 Category Analysis

The project compares categories based on revenue, profit, quantity sold, inventory, and orders.

Revenue by Category
Category	Approx. Revenue
Electronics	₹106.66M
Furniture	₹86.36M
Accessories	₹50.87M
Sports	₹37.26M
Stationery	₹20.73M

Electronics is the highest-revenue and most-profitable category.

🚚 Supplier Analysis

Supplier performance was evaluated using:

Revenue
Profit
Quantity Sold
Average Delivery Days
Delivery Delay
Defective Units
Key Findings

Most profitable supplier:

TechSource India

Slowest supplier based on average delivery time:

National Distributors

Fastest supplier based on average delivery time:

Apex Supplies

🏭 Warehouse Analysis

The project evaluates warehouses using:

Revenue
Profit
Quantity Sold
Average Inventory
Number of Orders
Highest Revenue Warehouse

Hyderabad WH

🌎 Regional Analysis

Three regions were analyzed:

North
South
West
Revenue Performance
Region	Revenue
West	₹120.98M
South	₹120.56M
North	₹60.34M

West generated the highest revenue.

🚛 Delivery Performance

Delivery performance was analyzed by comparing actual delivery time with expected lead time.

Key Result

Delivery Delay Rate: 41.97%

This indicates that delivery performance is an important area for operational improvement.

🧪 Product Quality Analysis

The project also analyzes defective units.

Results
Quality Metric	Result
Total Defective Units	6,122
Defect Rate	1.77%

Supplier-level defective units were also analyzed to identify suppliers with higher defect counts.

📊 Power BI Dashboard

The Power BI dashboard provides an interactive view of the supply chain performance.

Dashboard Page 1 — Executive Overview

The dashboard includes:

Total Revenue
Total Profit
Total Orders
Units Sold
Profit Margin
Revenue by Category
Revenue by Month
Revenue by Region
Order Status
Main KPIs
KPI	Value
Total Revenue	₹301.88M
Total Profit	₹112.90M
Total Orders	30K
Units Sold	346K
Profit Margin	37.40%
Dashboard Page 2 — Inventory & Quality

The second dashboard page focuses on:

Inventory Status
Reorder Level
Inventory Level
Defective Units by Category
Monthly Defective Units
Category filtering
Order Status filtering
Region filtering
💡 Key Business Insights
1. Electronics is the strongest category

Electronics generates the highest revenue and profit among all categories.

2. Inventory requires monitoring

There are 6,081 low-stock records and 4,543 overstock records, showing opportunities to improve inventory balancing.

3. Delivery performance needs improvement

The delivery delay rate is 41.97%, making supplier and logistics performance an important area for improvement.

4. TechSource India is the most profitable supplier

TechSource India generated the highest supplier-level profit in the analysis.

5. Hyderabad WH leads warehouse revenue

Hyderabad WH generated the highest warehouse revenue.

6. Product quality is relatively important

The analysis identified 6,122 defective units, with a calculated defect rate of 1.77%.

📁 Project Structure
Supply_Chain_Inventory/
│
├── README.md
│
├── data/
│   ├── supply_chain_inventory_30000_transactions.csv
│   └── Supply_Chain_PowerBI_Final_dataset.csv
│
├── notebook/
│   └── Supply_Chain_Inventory_Analytics.ipynb
│
├── powerbi/
│   ├── Supply Chain Inventory.pbix
│   └── Supply Chain Inventory dashboard.pdf
│
└── docs/
    └── Supply_Chain_Inventory_Analytics.ml.pdf.pdf
🚀 How to Run the Project
Step 1 — Clone the repository
git clone https://github.com/YOUR-USERNAME/Supply_Chain_Inventory.git
Step 2 — Navigate to the project
cd Supply_Chain_Inventory
Step 3 — Install Python libraries
pip install pandas numpy matplotlib seaborn plotly openpyxl scikit-learn jupyter
Step 4 — Open Jupyter Notebook
jupyter notebook

Open:

notebook/Supply_Chain_Inventory_Analytics.ipynb
📊 Power BI

The Power BI report is available in:

powerbi/Supply Chain Inventory.pbix

Open the .pbix file using Power BI Desktop.

The dashboard PDF is also included for users who do not have Power BI Desktop.

📚 Project Deliverables

This repository contains:

✅ Raw supply chain dataset
✅ Final Power BI dataset
✅ Python analysis notebook
✅ Power BI .pbix dashboard
✅ Dashboard PDF
✅ Project analysis report
✅ Documentation
👨‍💻 Author
Rishab Das

Data Analytics | Python | Power BI | SQL | Tableau

⭐ Project Highlights
30,000 Transactions
₹301.88M Revenue
₹112.90M Profit
346K Units Sold
37.40% Profit Margin
41.97% Delivery Delay Rate
1.77% Defect Rate
⭐ If you find this project useful

Feel free to explore the analysis, dashboard, and datasets.

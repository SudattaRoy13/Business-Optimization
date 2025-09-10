
# 📊 Business Optimization – Power BI Project

I analyzed business inventory and demand data using **Power BI**, integrating both **SQL Server** database.  
The project demonstrates **real-world workflows** like transitioning reports from **test** to **production environments**, handling **data inconsistencies**, and building KPIs with **DAX** for better decision-making.  

---

## Introduction
The **Business Optimization** project focuses on analyzing **demand, availability, and profitability** to uncover supply chain inefficiencies.  
Built in **Power BI** with **6 KPIs across 2 pages**, the report highlights supply shortages, profits, and losses while demonstrating **environment transitions** (Test → Production).  

---

## Work Done
- **Data Cleaning & Transformation** with SQL (`LEFT JOIN`, `SELECT INTO`, `UPDATE`)  
- Created **calculated columns & DAX measures** (`SUM`, `SUMX`, `FILTER`, `DIVIDE`, `DISTINCTCOUNT`)  
- Detected & resolved **data inconsistencies** (extra product IDs) with SQL updates  
- Designed **interactive dashboards** with KPIs, cards, and slicers for better insights  

---

## Report Pages & Highlights
### Page 1 – Demand & Availability
- **Average Demand per Day** (`DIVIDE(SUM(Demand), DISTINCTCOUNT(OrderDate))`)  
- **Average Availability per Day** (`DIVIDE(SUM(Availability), DISTINCTCOUNT(OrderDate))`)  
- **Total Supply Shortage** (`SUM(Demand) - SUM(Availability)`)  
📸 *[Screenshot – Page 1](https://github.com/SudattaRoy13/Business-Optimization/blob/main/Business%201.png)*  

### Page 2 – Profit & Loss Analysis
- **Total Profit** (`SUMX(FILTER(…, Profit/Loss > 0), Profit/Loss * Unit Price)`)  
- **Total Loss** (`SUMX(FILTER(…, Profit/Loss < 0), Profit/Loss * Unit Price)`)  
- **Average Daily Loss** (`DIVIDE([Total Loss], [Total Number of Days])`)  
📸 *[Screenshot – Page 2](https://github.com/SudattaRoy13/Business-Optimization/blob/main/Business%202.png)*  

---

## Key Insights
- **Supply shortages** clearly identified with demand vs availability.  
- **Profit/Loss breakdown** shows true financial impact when tied to unit prices.  
- **Data validation in production** uncovered mismatched product IDs, resolved via SQL.  
- Seamless **test → production environment transitions** achieved without breaking DAX measures.  

---

## How to Use
1. Download the [`.pbix` file.](https://github.com/SudattaRoy13/Business-Optimization/blob/main/Data%20Visualization%20for%20Business.pbix)
2. Open in **Power BI Desktop**.  
3. Explore **2 interactive pages of KPIs & visuals**.  


---

## Author
**Sudatta Roy**  
*Data Analyst | Power BI Enthusiast*  
🔗 [LinkedIn](www.linkedin.com/in/sudatta-roy-261540262) | [GitHub](https://github.com/SudattaRoy13)

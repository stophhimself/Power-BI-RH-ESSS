# 💼 Sales Dashboard — PB13 (Power BI)

## 📌 Project Overview  
This project analyzes **global sales data for a retail company (Contoso)** using **Power BI**, with the objective of understanding **sales performance by store, product, region, category, and time period**.  

The dashboard is designed to showcase **data visualization, exploratory analysis, and business storytelling skills**, using real-world retail analytics data — perfect for demonstrating commercial insight in a multinational retail context.

---

## 👀 Dashboard Preview  
<img width="590" height="323" alt="pob 1" src="https://github.com/user-attachments/assets/ac5cd38c-f661-4548-8076-550246ab0399" />
<img width="576" height="318" alt="pob 2" src="https://github.com/user-attachments/assets/29677f09-7c8e-478d-b3d7-5a7d2f2ee5d8" />
<img width="572" height="322" alt="pob 3" src="https://github.com/user-attachments/assets/4d6473f6-e70b-4e13-8835-023fb0717530" />


*(Screenshot captured January 14, 2026)*

---

## 🎯 Objectives  
- Analyze **total stores, employees, products, and sales volume**  
- Compare **sales by country, store type, and status**  
- Understand **product categories and subcategories performance**  
- Visualize **sales trends over time (by year/month)**  
- Explore **revenue vs quantity sold per product**  
- Practice **dashboard design and analytical storytelling** in Power BI

---

## 📊 Dashboard Breakdown

### 🔹 Key Metrics (KPIs)
- **Total Stores**: 306  
- **Total Employees**: 11K  
- **Total Products**: 1,689  
- **Total Sales**: 68K units  
- **Revenue (Chiffre d’Affaires)**: €257,655,442,743.00  
- **Filters**: Country, Continent, Year, Month, Product Class, Brand

---

### 🔹 Pays & Boutiques (Stores by Country)  
- Filterable list of countries (Armenia, Australia, Canada, China, France, Germany, India, Italy, Japan, etc.)  
- Table showing:  
  - Country  
  - Store Name (e.g., *Contoso Albany Store*, *Contoso Amsterdam Store*)  
  - Employee Count  
  - Surface Area  
  - Type (Store / Online / Reseller / Catalog)  
  - Status (On / Off)  
→ Highlights **store distribution across continents**, with focus on USA, Netherlands, Turkmenistan

---

### 🔹 Nb Boutique par Type  
- Bar chart showing store types:  
  - Store: **3**  
  - Online: **1**  
  - Reseller: **0**  
  - Catalog: **0**  
→ Confirms **physical stores dominate**, with minimal online/reseller presence

---

### 🔹 Nb Boutique par Status  
- Donut chart showing:  
  - **On**: 294 stores  
  - **Off**: 12 stores  
→ Shows **high operational uptime** — only 4% of stores inactive

---

### 🔹 Carte (World Map)  
- Interactive map highlighting **sales regions** (Asia, Europe, North America)  
- Color-coded by continent → supports **geographic segmentation**

---

### 🔹 Nb Ventes par Boutique  
- Bar chart showing top-performing stores:  
  - Top store: **44K sales**  
  - Second: **31K**  
  - Others: mostly **1K–3K**  
→ Reveals **heavy concentration of sales in a few flagship stores**

---

### 🔹 Nb Produits & Catégories  
- Total products: **1,689**  
- Top categories:  
  - Computers: **606**  
  - Cameras and camcorders: **371**  
  - Cell phones: **222**  
  - Audio: **115**  
  - Music: **90**  
→ Shows **strong focus on tech and electronics**

---

### 🔹 NB Retour vs NB Vente par Produit  
- Line chart comparing **quantity sold vs quantity returned** per product  
- Most products have low return rate → healthy customer satisfaction  
- Some spikes show **higher return rates** — potential quality or fit issues

---

### 🔹 Nb Ventes par Produit  
- Treemap showing top-selling products:  
  - Adventure Works Laptop: **274**  
  - Fabrikam Laptop 14.1W: **263**  
  - Adventure Works Laptop: **256**  
→ Highlights **laptops as top performers** — key revenue drivers

---

### 🔹 CA par Catégorie Produit  
- Pie chart showing revenue by category:  
  - Computers: largest slice  
  - TV and Video  
  - Cell Phones  
  - Audio  
  - Music  
→ Confirms **Computers generate highest revenue**

---

### 🔹 CA par Marque  
- Pie chart showing brand contribution:  
  - Adventure Works  
  - Contoso  
  - Wide World Importers  
  - Proseware  
  - The Phone Company  
→ Shows **diverse brand portfolio**, with Adventure Works leading

---

### 🔹 CA par Class  
- Pie chart showing customer segment performance:  
  - Regular  
  - Deluxe  
  - Economy  
→ Reveals **Deluxe segment drives most revenue** — target for premium offerings

---

### 🔹 CA et Nb Ventes par Date  
- Scatter plot showing **revenue vs sales volume over time**  
- Peaks around **Jan–Apr 2021** → strong start to year  
→ Useful for **seasonal forecasting and inventory planning**

---

### 🔹 CA et CA - 1 (Year-over-Year Comparison)  
- Gauge showing **€242,744,288,903,500.00** (likely typo — should be ~€242B)  
- Compares current year vs previous year → shows growth trend

---

### 🔹 CA par Mois (Monthly Revenue Table)  
- Table showing monthly revenue and YoY growth:  
  - January: €21.9B (+15.10%)  
  - September: €28.6B (+8.99%)  
  - August: €28.6B (+9.40%)  
  - April: €29.8B (+7.75%)  
  - June: €31.4B (+13.22%)  
→ Confirms **strong growth in H1 2021**, especially June

---

## 📐 Methodology
- Data cleaning and preprocessing (handling missing values, standardizing country/product names)  
- Creation of calculated measures:  
  - `CA = SUM(Sales[Amount])`  
  - `Nb Ventes = COUNTROWS(Sales)`  
  - `CA - 1 = CALCULATE([CA], SAMEPERIODLASTYEAR('Date'[Date]))`  
- Time-based aggregation (monthly/yearly trends)  
- Use of:  
  - KPI cards  
  - Bar charts  
  - Pie/donut charts  
  - Scatter plots  
  - Treemaps  
  - Filters (Country, Year, Month, Class, Brand)  
- Focus on **visual consistency, readability, and blue/white corporate theme**

---

## 🛠️ Tools & Technologies
- **Power BI Desktop**  
- **Data modeling** (star schema implied)  
- **Basic–Intermediate DAX** (aggregations, time intelligence, comparisons)  
- **Data visualization principles** (color theory, spacing, hierarchy)  
- **Dashboard layout & storytelling** (flow from overview → deep dive)

---

## 📌 Key Insights
✅ **306 stores, 11K employees, 1,689 products** — large-scale retail operation  
✅ **294 stores active (96%)** — high operational efficiency  
✅ **Computers and Laptops drive most sales and revenue** — tech-focused business  
✅ **Adventure Works and Wide World Importers are top brands** — key partners  
✅ **Deluxe customer segment generates highest revenue** — target for upselling  
✅ **Strong growth in Jan–Jun 2021**, especially June (+13.22% YoY)  
✅ **Top stores generate 10x more sales than average** — focus on scaling best performers  
✅ **Low return rates overall** — good product-market fit and customer satisfaction

---

## 📁 Repository Structure

├── Sales_Dashboard_PB13.pbix
├── Dataset/
│ └── contoso_sales_data.csv
├── Screenshots/
│ └── sales_dashboard_pb13.png
└── README.md


---

## 🚀 Project Purpose
This project was built as a **portfolio Power BI project** to:  
- Practice **retail and e-commerce analytics**  
- Improve **dashboard design and visual storytelling**  
- Apply **business-oriented insight generation**  
- Simulate **analytics reporting for global retail chains**

---

## 📬 Contact
**Mustapha Tarfi**  
📍 Morocco  
🔗 LinkedIn: [https://www.linkedin.com/in/mustapha-tarfi-1106b5283/](https://www.linkedin.com/in/mustapha-tarfi-1106b5283/)  

---

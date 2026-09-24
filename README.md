# Samsung-Supply-Chain-Logistics-PowerBI
# 📱 Samsung Supply Chain & Logistics Analytics Dashboard

## 📊 Project Overview

The **Samsung Supply Chain & Logistics Analytics Dashboard** is a multi-page interactive Power BI dashboard designed to analyze end-to-end supply chain performance, inventory health, supplier efficiency, logistics delays, and customer sales metrics.

The project transforms raw supply chain and logistics data into actionable business intelligence covering gross revenue, net profit, defect rates, supplier lead times, carrier delays, shipment status, and channel sales.

The dashboard features built-in navigation buttons across six dedicated analytical views to explore operational performance seamlessly:
* **Home Page**
* **Overview**
* **Inventory & Production**
* **Supplier**
* **Shipment**
* **Customer**

---

## 🎯 Project Objectives

The main objectives of this project are:

- Track total revenue, profit margin, and perfect order fulfilment rate.
- Monitor inventory stock levels, safety stock thresholds, and reorder points.
- Evaluate product defect rates and identify high-defect hardware models.
- Analyze supplier performance based on lead time, unit cost, quality score, and order volume.
- Identify top logistics carriers contributing to delivery delays and root cause delay reasons.
- Compare revenue and profit performance across digital, retail, and direct customer sales channels.
- Build a responsive, multi-page Power BI dashboard with page-to-page navigation.

---

## 🛠️ Tools & Technologies

- Microsoft Power BI
- Power Query
- DAX (Data Analysis Expressions)
- Data Modeling & Relationships
- Supply Chain & Logistics Analytics

---

## 📁 Dataset & Modules

The dataset covers multi-dimensional supply chain operations from manufacturing to final delivery:

- **Financials**: Gross Revenue ($186.86M), Total Revenue ($176.95M), Net Profit ($48.56M).
- **Inventory & Production**: 160K Inventory Value, 89K Safety Stock, 24K Defective Units across products (e.g., Galaxy S24 Ultra, Galaxy Buds2 Pro, Galaxy Watch6 Classic).
- **Suppliers**: Supplier metrics for major tech vendors (BOE Technology, Samsung Electronics, Sony Semiconductor, Taiwan Semiconductor, SK Hynix, etc.) across various countries.
- **Shipment & Logistics**: 8K Total Shipments, 3M Shipment Quantity, 573 Total Delays handled by carriers like Maersk, DHL Express, DB Schenker, FedEx, and UPS.
- **Customer & Sales Channels**: Sales performance across platforms (Amazon.com, Flipkart, Best Buy, MediaMarkt Saturn, Samsung Direct) and channels (Online, Retailer, Direct).

---

## 🧹 Data Preparation

Data cleaning and structural transformations were executed in Power Query prior to visual report creation:

1. Imported raw CSV/Excel datasets into Power BI Desktop.
2. Verified column data types for financial values, lead times, shipment counts, and defect ratios.
3. Cleaned and normalized vendor/supplier name strings.
4. Created custom conditional columns to categorize delay status (Delivered, In Transit, Delayed, Processing).
5. Handled missing data points in lead times and defect metrics.
6. Generated a dedicated Date Table for time-intelligence functions.
7. Connected tables via clean star-schema relationships.

---

## 🗂️ Data Model

A dedicated Date Table was created to support time-based analysis.

The main relationship model connects Fact and Dimension tables:

Date Table → Orders & Shipments Fact
Product Dimension → Inventory & Defect Fact
Supplier Dimension → Sourcing & Lead Time Fact
Carrier Dimension → Delivery & Delay Fact

---

## 📌 Key KPIs

| KPI | Value |
|---|---:|
| **Gross Revenue** | $186.86M |
| **Total Revenue** | $176.95M |
| **Net Profit** | $48.56M |
| **Profit Margin** | 27.44% |
| **Perfect Order Rate** | 75% |
| **Total Shipments** | 8K |
| **Delivered %** | 75.29% |
| **Avg Quality Score** | 96.63 |
| **Avg Lead Time** | 11.53 Days |
| **Days of Inventory** | 12.99 Days |

---

## 📊 Dashboard Visualizations & Views

### 1. HOME VIEW
Features an executive landing page with navigation shortcuts to deep-dive reports (Overview, Inventory & Production, Supplier, Shipment, Customer).

### 2. OVERVIEW DASHBOARD
- High-level KPI cards for financial and operational metrics.
- Executive summary modules for Supplier, Manufacturer, Shipment, and Customer status.
- Top delayed carriers and top revenue-generating platforms.

### 3. INVENTORY & PRODUCTION DASHBOARD
- Monthly trend analysis of defective units and inventory valuation.
- Product-wise defect breakdown highlighting models with high defect rates (Galaxy S24 Ultra, Buds2 Pro).
- Dynamic stock comparison chart visualizing Current Stock, Safety Stock, and Reorder Points.

### 4. SUPPLIER DASHBOARD
- Supplier lead time performance by vendor and country (China, Japan, South Korea, Taiwan, India, Vietnam).
- Vendor comparison by order quantity, total unit cost, and average quality score.

### 5. SHIPMENT & LOGISTICS DASHBOARD
- Carrier delay comparison (Total Delay vs Total Delivered Shipments).
- Shipment status distribution donut chart (Delivered, In Transit, Delayed, Processing).
- Breakdown of root-cause delay factors (Carrier Capacity, Port Congestion, Customs Clearance, Weather).
- Shipment cost trends across months.

### 6. CUSTOMER & SALES DASHBOARD
- Revenue, profit, and revenue growth trend analysis.
- Channel sales performance (Online, Retailer, Direct) and category discount distributions.
- Platform performance breakdown (Amazon, Flipkart, Best Buy, MediaMarkt, Direct).

---

## 🎛️ Interactive Features

- **Page Navigation Buttons**: Header tabs allow seamless swapping between supply chain modules.
- **Reset & Home Actions**: Header quick icons to clear filters or return to the landing page.
- **Dynamic Slicers**: Multi-select options for product models, carrier names, and sales channels.

---

## 💡 Key Business Insights

### Operational Revenue & Margin
Gross revenue reached **$186.86M** with a healthy **27.44% profit margin**, driven largely by Online and Retailer sales channels.

### Inventory & Defect Management
Galaxy S24 Ultra and Galaxy Buds2 Pro reported the highest absolute defective units, indicating a need for tighter quality control during assembly.

### Logistics & Carrier Delays
**Maersk Line** and **DHL Express** recorded the highest number of delayed shipments. Carrier capacity limits and documentation issues were identified as primary delay drivers.

### Supplier Performance
Suppliers from Taiwan, South Korea, Japan, and China achieved top quality scores (97-98/100) while maintaining lead times of ~12 days.

---

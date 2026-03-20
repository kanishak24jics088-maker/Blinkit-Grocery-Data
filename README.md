# 🛒 Blinkit Grocery Sales Analysis (Power BI)

## 📌 Project Overview

This project presents an end-to-end **sales performance analysis** of Blinkit (India’s last-minute grocery delivery app) using **Power BI**. The dashboard provides insights into sales trends, product performance, outlet characteristics, and customer preferences.

The goal is to enable **data-driven decision-making** by identifying key drivers of revenue, optimizing inventory, and improving outlet performance.

---

## 🚀 Key Features

* 📊 Interactive Power BI dashboard with dynamic filters
* 📈 Sales trend analysis over time
* 🏪 Outlet-level performance breakdown (size, location, type)
* 🥗 Product category insights (item type, fat content)
* ⭐ Customer rating analysis
* 📦 KPI tracking:

  * Total Sales
  * Average Sales
  * Number of Items
  * Average Rating

---

## 📂 Data Sources

* Primary dataset: Blinkit grocery sales dataset (CSV/Excel)
* Data includes:

  * Item details (type, fat content)
  * Outlet information (size, location tier, type)
  * Sales and rating metrics

> ⚠️ Note: Dataset may be synthetic or sourced from publicly available datasets for learning purposes.

---

## 🛠️ Prerequisites

### Software Required

* [Power BI Desktop](https://powerbi.microsoft.com/desktop/)
* Git (optional, for cloning repo)

---

## ⚙️ Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/blinkit-sales-analysis.git
cd blinkit-sales-analysis
```

### 2. Open Power BI File

* Launch **Power BI Desktop**
* Open:

```bash
Blinkit_Sales_Dashboard.pbix
```

### 3. Load Data

* If prompted, update the data source path:

  * Go to **Transform Data → Data Source Settings**
  * Replace file path with your local dataset location

---

## ▶️ How to View the Report

### Option 1: Power BI Desktop

* Open `.pbix` file
* Interact with slicers:

  * Outlet Location Type
  * Outlet Size
  * Item Type

### Option 2: Power BI Service (if deployed)

* Upload `.pbix` to Power BI Service
* Access via workspace dashboard
* Share via link (if enabled)

---


## 🧠 Data Model & Metrics

### 📊 Key Measures

* **Total Sales**

  ```DAX
  Total Sales = SUM(Sales[Sales_Amount])
  ```

* **Average Sales**

  ```DAX
  Avg Sales = AVERAGE(Sales[Sales_Amount])
  ```

* **Number of Items**

  ```DAX
  No of Items = COUNT(Sales[Item_ID])
  ```

* **Average Rating**

  ```DAX
  Avg Rating = AVERAGE(Sales[Rating])
  ```

---

### 📐 Data Relationships

* Fact Table: `Sales`
* Dimension Tables:

  * Items
  * Outlets

Relationships:

* Items → Sales (1:M)
* Outlets → Sales (1:M)

---

## 📊 Visualization Highlights

### Dashboard Preview

![Dashboard Screenshot](assets/dashboard_screenshot.png)

### Key Visuals

* 📈 **Outlet Establishment Trend** (Year-wise sales)
* 🍩 **Fat Content Distribution** (Donut chart)
* 📊 **Item Type Performance** (Bar chart)
* 🏪 **Outlet Size Contribution**
* 📍 **Outlet Location Tier Analysis**
* 📋 **Outlet Type Summary Table**

---

## 📝 Usage Notes

* Use slicers to filter data dynamically
* Hover over visuals for detailed tooltips
* Combine filters for deeper insights

---

## ⚠️ Limitations & Assumptions

* Dataset may not reflect real Blinkit data
* Missing values handled via default aggregation
* Ratings assumed to be uniformly distributed
* Time-series analysis limited to available years

---

## 🔄 Data Refresh & Reproducibility

### Refresh Data

* Open Power BI Desktop
* Click **Refresh**
* Ensure dataset path is correct

### Reproduce Results

1. Use the same dataset file
2. Maintain consistent schema
3. Refresh all visuals after loading data

---

## ☁️ Deployment & Automation

### Power BI Service Deployment

1. Publish report from Power BI Desktop
2. Upload to workspace
3. Configure dataset credentials






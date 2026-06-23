# Corporate Financial Performance Analytics Dashboard 📈

An end-to-end Business Intelligence solution developed in Power BI to analyze global financial transactions, optimize profit margins, and deliver actionable strategic insights for corporate decision-makers.

📌 Table of Contents
* [Project Overview](#-project-overview)
* [Tools & Skills Used](#%EF%B8%8F-tools--skills-used)
* [Dataset Structure](#%F0%9F%93%8A-dataset-structure)
* [Project Screenshots & Architecture](#-project-screenshots--architecture)
* [Phase 1 — Data Import & Cleaning with Power Query](#phase-1--data-import--cleaning-with-power-query)
* [Phase 2 — Data Modeling & Workspace View](#phase-2--data-modeling--workspace-view)
* [Phase 3 — Explicit DAX Measures Engine](#phase-3--explicit-dax-measures-engine)
* [Key Business Insights](#-key-business-insights)
* [Author](#-author)

---

## 🚀 Project Overview
This project demonstrates the development of an enterprise-grade financial analytics asset. Starting with raw financial transaction records, I built a fully interactive dashboard in Power BI that allows executives to:
* Monitor **Total Sales, Gross Revenue, and Bottom-line Net Profits** instantly.
* Evaluate the health of the business via a dynamic **Profit Margin (%)** tracking engine.
* Break down performance across global territories, market segments, and product lines.
* Filter all report visuals seamlessly using interactive slicers.

---

## 🛠️ Tools & Skills Used
* **Power BI Desktop:** Core engine for reporting, data engineering, and visualization layouts.
* **Power Query Editor:** Advanced ETL process, structural anomalies cleanup, and data type management.
* **Data Modeling:** Tabular data schema workspace structuring for optimized report filtering performance.
* **DAX (Data Analysis Expressions):** Custom explicit semantic modeling to calculate business metrics.
* **UI/UX Report Design:** Pixel-perfect grid layout, structured whitespace, and card alignments for rapid executive scannability.

---

## 📊 Dataset Structure
* **Source:** Corporate Financial Transaction Logs
* **Core Granularity:** Line-item transaction records mapping international business operations.
* **Key Fields Managed:** Segment, Country, Product, Discount Band, Units Sold, Manufacturing Price, Sale Price, Gross Sales, Discounts, Sales, COGS (Cost of Goods Sold), Profit, Date, Month Number, Month Name, Year.

---

## 📸 Project Screenshots & Architecture

### 1. Interactive Executive Dashboard Visuals
*The core visual layout optimized for high scannability, structural spacing, and professional color composition.*
![Dashboard Visuals](./1_Dashboard_Visuals.png)

### 2. Backend Table View & DAX Engine
*The isolated report backend where structural table formats are verified and performance measures are computed.*
![Data and DAX View](./2_Data_Calculations.png)

### 3. Structural Data Model View
*The operational workspace displaying backend table schema structures and entity architectures inside Power BI.*
![Model Schema](./3_Model_Schema.png)

---

## Phase 1 — Data Import & Cleaning with Power Query
1. Loaded raw transaction data files into the **Power BI Power Query Engine**.
2. Inspected structural integrity and synchronized data types across all functional blocks (Dates, Integers, Decimals).
3. Evaluated relational schemas and removed system-level operational noise columns.
4. Capitalized text categories, standardized numerical precisions, and ran data profiling checks before pushing to data tables.

## Phase 2 — Data Modeling & Workspace View
* Structured the single-table operational workspace schema inside the Model View workspace.
* Configured column aggregation properties and verified implicit date dimensions mapping.
* Optimized field formatting parameters to guarantee that any visual slicer interaction instantly updates global visuals without lagging.

## Phase 3 — Explicit DAX Measures Engine
Rather than relying on default implicit aggregations, I engineered explicit DAX logic layers from scratch to secure analytical control:

```dax
// Core Sales Aggregate Logic
Total Sales = SUM('financials'[Sales])

// Core Profit Volume Engine
Total Profit = SUM('financials'[Profit])

// Pixel-Perfect Multi-Tiered Profit Margin Evaluation Ratio
Profit Margin (%) = DIVIDE([Total Profit], [Total Sales], 0)

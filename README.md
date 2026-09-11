# Sales & Profit Analysis Dashboard

An advanced, data-driven Excel workbook featuring interactive dashboards, pivot tables, and automated reporting systems built to track comprehensive business metrics, customer demographics, and transactional profit margins.

## 📊 Project Overview

This repository houses a comprehensive retail analytics and business intelligence tool. Driven by an underlying structured data model, the repository processes raw transactional history to deliver real-time metrics on performance, volumetric inventory movement, and customer purchasing behaviour.

### Core Architecture Breakdown
* **Data Foundation (`xl/worksheets/`)**: Implements dedicated operational layers (`sheet1`, `sheet2`, `sheet3`) storing granular records including Customer IDs, Product SKU specifics, regional flags, and precise timestamp arrays.
* **Analytical Engines (`xl/pivotTables/`)**: Utilizes 10 independent, pre-cached Pivot Cache Definitions coupled with multi-dimensional analytical structures to handle instant cross-tabulations dynamically.
* **Visualization Assets (`xl/charts/`)**: Houses 8 purpose-built analytical visualization models mapped to color themes for C-suite readouts, monitoring operational efficiency, and monitoring geographic market performance.
* **Automation Backend (`xl/vbaProject.bin`)**: Employs compiled VBA binary macros executing backend procedures, refresh routines, operational logic, and report-export loops.

---

## 🔑 Tracked Metrics & Data Model

The analytical model relies on a tightly integrated relational data schema tracking these critical parameters:

* **Temporal Filters**: `Year` | `Quarter` | `Month` | `Month No`
* **Customer Dimensions**: `Customer ID` | `Customer Name`
* **Product Inventory**: `Product ID` | `Product Name` | `Item Category`
* **Transactional Economics**: `Quantity Sold` | `Unit Price` | `Cost Amount` | `Sales Amount` | `Profit`

---

## ⚡ Features & Capabilities

* **Implicit & Explicit Measures**: Embedded calculation scripts optimizing aggregated calculations (e.g., `SUM of Sales Amount`, `DISTINCTCOUNT of Customers`, `SUM of Profit Margin`).
* **Slicer Integration**: Multi-layered interactive UI slicer caches allowing cross-filtering across complex product arrays and periods concurrently.
* **High-Performance Memory Layout**: Built on top of an internal `InMemory` transactional database mode optimized for speed and eliminating query-latency drop-offs on large datasets.

---

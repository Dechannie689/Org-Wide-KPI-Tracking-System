# Org-Wide-KPI-Tracking-System

![](https://github.com/Dechannie689/Org-Wide-KPI-Tracking-System/blob/main/KPI_DASHBOARD.png)

An automated KPI analysis system that consolidates employee, finance, ERP system and other manual tracking files into a weighted performance scorecard, giving managers and employee a real-time view of individual and team results against targets.

---

## 📌 Overview

Organizations with distributed teams often lack a unified, consistent method to track employee KPI performance across departments. Manually compiling results from multiple Excel files and ERP exports each month was time-consuming and error-prone, making it difficult to identify underperformers or reward top contributors in time.

This project built an automated ingestion and transformation pipeline that pulls Employee Data, Finance Data and ERP System (daily) into a Microsoft Fabric Lakehouse. Notebooks process and join these sources to calculate weighted KPI scores per employee per month, which are then surfaced in a Power BI dashboard with role and month filters.

The January 2026 snapshot shows a Manager-level Total Result YTD giving C level immediate clarity on where performance is strong and where it needs attention.

---

## 🏗️ Architecture

![](https://github.com/Dechannie689/Org-Wide-KPI-Tracking-System/blob/main/KPI_WORKFLOW.png)

---

## 🛠️ Tech Stack

- **Microsoft Fabric Pipeline / Dataflow** — automates ingestion of Excel and ERP files into the Lakehouse on defined schedules
- **Databricks Notebooks** — handles data transformation, KPI weight application, and fact table generation
- **Microsoft Fabric Lakehouse / OneLake** — unified Delta storage layer for raw, transformed, and master KPI data
- **Azure AD** — identity and access management across the platform
- **Azure Key Vault** — secure credential and secret management
- **Microsoft Purview** — data discovery and governance
- **Azure Monitor** — platform monitoring and cost management
- **Power BI** — interactive KPI scorecard with position and month slicers, gauge charts for each KPI, and color-coded performance bands (Fail / Average / Good / Excellent)

---

## 📊 Dashboard & Key Metrics

The dashboard is used by HR managers and department heads to evaluate monthly KPI performance at the individual and role level. Each KPI card shows the fiscal year target, actual YTD value, result percentage, and KPI weight — making it easy to identify which metrics are dragging down an employee's overall score and to track month-over-month improvement.

[View the full dashboard PDF](https://github.com/Dechannie689/Org-Wide-KPI-Tracking-System/blob/main/KPI_DASHBOARD.pdf)

---

## 📬 Contact

Built by [Thuy Trang](https://www.linkedin.com/in/trangthuynguyen6899/) · trangthuynguyen6899@gmail.com


# Org-Wide-KPI-Tracking-System

![](https://github.com/Dechannie689/Marketing-Analysis/blob/main/MARKETING%20DASHBOARD.png)

End-to-end multi-channel marketing analytics pipeline built on Microsoft Fabric, unifying Instagram, Pinterest, YouTube, LinkedIn and Website data into a single Power BI reporting, covering audience demographics, traffic sources, and lead quality across 5 platforms.

---

## 📌 Overview

Marketing teams tracking performance across multiple social channels and a website with fragmented, manually-exported CSV files that are slow to consolidate. Understanding where high-quality leads come from, which platform drives the most engaged traffic, and how audience profiles differ by channel requires stitching together data that rarely lives in the same place.

This project automates the full pipeline: raw data from Instagram, Pinterest, YouTube, LinkedIn, and website sessions is ingested via Microsoft Fabric Pipelines and Dataflows, stored in a Bronze/Silver/Gold Lakehouse on OneLake, cleansed and validated through PySpark Notebooks, and modelled into a Semantic Model that powers a multi-page Power BI dashboard — refreshed automatically and filterable by date range and brand.

The result is a unified marketing intelligence platform covering the period Nov 2025–Mar 2026, tracking 7,574 site sessions, 6,456 Instagram followers, 286,667 Pinterest views, and 239 qualified leads — with full visibility into audience demographics, geographic reach, and content performance across all channels.

---

## 🏗️ Architecture

![](https://github.com/Dechannie689/Marketing-Analysis/blob/main/Marketing%20Analysis.png)

---

## 🛠️ Tech Stack

- **Microsoft Fabric (OneLake + Lakehouse)** — unified Bronze/Silver/Gold storage with no data movement between services; all layers live in one logical lake
- **Fabric Pipelines & Dataflows** — low-code ingestion of CSV platform exports and SharePoint form submissions
- **PySpark Notebooks** — data quality scoring (accuracy %, completeness), text normalisation, and transformation logic
- **Power BI Semantic Model** — centralised metric definitions with row-level security and both import and DirectQuery modes
- **Power BI Desktop** — 6-page interactive dashboard (Website, Leads, Instagram, Pinterest, YouTube, LinkedIn)
- **Microsoft Purview** — data governance and lineage tracking across the pipeline
- **Azure Key Vault** — secure credential and secret management
- **Azure Monitor** — pipeline health monitoring and alerting

---

## 📊 Dashboard & Key Metrics

The Power BI dashboard serves managers and employees who need a consolidated view of cross-channel performance. Each of the 6 pages is dedicated to one channel, with a shared date slicer (Nov 2025–Mar 2026) and brand filter. Stakeholders can track how audience demographics, geographic reach, and engagement evolve month over month — and compare lead quality against the traffic sources driving site visits.

[View the full dashboard PDF](https://github.com/Dechannie689/Marketing-Analysis/blob/main/WEBSITE_LEADS_REPORT.pdf)

---

## 📬 Contact

Built by [Thuy Trang](https://www.linkedin.com/in/trangthuynguyen6899/) · trangthuynguyen6899@gmail.com


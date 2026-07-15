# 🐾 UK Farm Rescue Operations: End-to-End Data Analytics Portfolio

> To optimize resource allocation and improve animal welfare outcomes, this project cleans and analyzes emergency farm rescue data across the United Kingdom. By resolving data inconsistencies in Google Sheets and conducting deep-dive relational SQL querying in Beekeeper Studio, I built an operational framework to pinpoint high-risk rescue profiles, cost anomalies, and geographic demand hubs.

---

## 📌 Business Case & Objectives
Emergency livestock rescue services across the UK operate under tight budgets and unpredictable demand. Traditional rescue management lacks central analysis, leading to high-cost outliers and lower animal survival rates due to suboptimal emergency routing and resource preparation.

This project aims to:
* **Standardize and clean raw operational records** to build a single, reliable version of truth.
* **Identify critical high-risk animal segments** and isolate systemic veterinary pain points.
* **Uncover cost deviations across regions** to guide targeted budget allocation and strategic depot placement.

---

## ⚙️ Methodology & Analytical Framework
To turn raw data into structured business intelligence, the project was executed in two distinct, sequential phases:

1.  **Data Cleaning & Standardization (Google Sheets):**
    * *Categorical Merging:* Grouped inconsistent animal classes by merging rare and `"unknown"` classifications into a standardized `"Other"` category.
    * *Boolean Normalization:* Converted chaotic boolean fields (`True`, `False`, `1`, `0`, and capitalization anomalies) into strict database-compliant formats for `vet_healthy` and `veg_vaccinated` (veterinary vaccination).
    * *Numerical Sanitization:* Aligned the data types for `animal_count`, `animals_survived`, and `estimated_cost` to proper numeric formats by stripping trailing spaces and adjusting float precision.
2.  **Relational SQL Analysis (Beekeeper Studio):**
    * *Performance Aggregations:* Evaluated unit-level costs and survival metrics across species to isolate low-performance segments.
    * *Window Functions for Outlier Detection:* Built partitioning queries to calculate regional cost baselines and identify rescue deployments with high cost deviations.
    * *Root Cause Categorization:* Aggregated the financial impact of underlying incident causes to determine which systemic drivers generate the highest average emergency response expenses.

---

## 🛠️ Tech Stack & Tools
* **Data Preparation:** Google Sheets (data auditing, text parsing, categorical mapping, and data sanitization)
* **Database Management:** Beekeeper Studio (Community Edition)
* **Language:** SQL (SQLite/PostgreSQL compatible dialect)

---

## 📂 Project Structure
```text
├── data/                  # Contains raw and final cleaned versions of the dataset
├── sql_queries/           # Structured SQL scripts covering species performance, cost outliers, and regional deviation
├── reports/               # Executive Word (.docx) document highlighting key business insights
└── README.md              # Project documentation and portfolio overview


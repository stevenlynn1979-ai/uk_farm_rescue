# TravelTide: Causal Inference & Customer Retention Optimization

> To tackle TravelTide's declining customer retention, this project bypasses costly blanket discounts by using rigorous causal inference modeling in Python. By mapping customer friction points, I designed a personalized perk allocation strategy that targets incentives to the right users, maximizing loyalty and incremental retention lift.

---

## 📌 Business Case & Objectives
TravelTide, an online travel platform, was experiencing a critical drop in customer retention. Traditional marketing strategies relied on blanket promotional discounts—a highly expensive approach that often subsidized bookings for users who would have booked anyway (selection bias). 

This project aims to:
*   **Identify the true causal impact** of five key perks on long-term user loyalty.
*   **Build an optimization framework** to route the right perk to the right user segment.
*   **Maximize retention lift** while preserving promotional margins.

---

## ⚙️ Methodology & Causal Framework
Rather than looking at simple correlations, this analysis uses causal concepts to isolate the incremental effect of TravelTide’s incentive programs:

1.  **Friction Point Mapping:** Audited extensive, high-velocity session and user journey datasets in Python to locate where users dropped off in the booking funnel.
2.  **Targeted Segments vs. Blanket Discounts:** Discovered that blanket discounts yielded low incremental lift. Instead, users were segmented by booking habits (e.g., flight-to-hotel ratios, travel frequency).
3.  **Perk Optimization Routing:** Evaluated and mapped five core perks to specific behavioral profiles:
    *   *Free Checked Bags* (High flight-only flyers)
    *   *Free Hotel Meals* (Hotel-heavy travelers)
    *   *Cancellation Fee Waivers* (Frequent business travelers)
    *   *Flight-Hotel Bundles* (Leisure/family travelers)
    *   *Flexible Credit Rollovers* (High-frequency, fluctuating schedule travelers)

---

## 🛠️ Tech Stack & Tools
*   **Language:** Python
*   **Data Manipulation:** Pandas, NumPy (handling session-level aggregations and cleaning)
*   **Data Visualization:** Matplotlib, Seaborn (exploratory data analysis)
*   **Database Querying:** SQL (extracting historical session and transactional data)

---

## 📂 Project Structure
```text
├── data/                  # Sample behavioral cohort data (anonymized)
├── notebooks/             # Python notebooks covering EDA, segmentation, & causal modeling
├── reports/               # Executive presentation deck with final recommendations
└── README.md              # Project documentation

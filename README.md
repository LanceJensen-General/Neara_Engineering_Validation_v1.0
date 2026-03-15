<p align="center">
  <img src="images/neara-banner.png" width="100%" alt="Neara Engineering Banner"/>
</p>

# Engineering Validation Package: Value-Based Pilot

This repository provides the engineering framework, raw data, and validated results for the **1,000-pole pilot cohort**. It demonstrates the financial and operational superiority of physics-based risk modeling over traditional age-based heuristics.

## 📂 Repository Structure

| Directory | Description |
| :--- | :--- |
| `Strategy_and_Approach.md` | Strategic overview of Physics-Based vs. Age-Based management. |
| `Implementation_Guide.md` | Scaling workflow featuring the SQL and Excel Engineering Cookbooks. |
| `/data` | Raw GIS (GeoJSON) and Asset (CSV) inputs used for the Digital Twin. |
| `/docs` | Methodology whitepapers and **Neara Pole Analysis.pptx** (Executive Summary). |
| `/results` | Validated structural reports and **Analysis-Results.xlsx** (ROI Model). |
| `/images` | Branding assets, **neara-banner.png**, and **neara-icon.png**. |

---

## 🛠 Methodology: "Physics-Based" Asset Management
This pilot transitioned the maintenance strategy for a **1,000-pole cohort** from chronological heuristics to a **High-Fidelity Digital Twin** assessment.

### 1. Decision Logic & Optimization
While the analysis covered the full cohort, the repository highlights the delta between two distinct strategies:
* **Neara Optimized Strategy:** Interventions prioritized by physics-verified risk and cascading failure potential.
* **Age-Based Heuristic:** Interventions prioritized strictly by the 28 oldest assets in the cohort.

The analysis is driven by the logic defined in:
* **`data/Cost of Mitigation.csv`**: Unit costs for interventions based on material and environment.
* **`data/Intervention Effect.csv`**: Statistical probability reduction post-mitigation.

### 2. Cascading Failure Analysis
We utilized the Digital Twin to identify "Single Points of Failure" where pole collapse causes multi-span failure.
* **Logic:** See `data/Task 2_ Consequence modifier.csv` for the multipliers applied to assets with overlapping span risks.

---

## 📊 Summary of Pilot Results (N=1000)
Detailed calculations are available in **`/results/Analysis-Results.xlsx`**.

| Metric | Neara Optimized (28 Poles) | Age-Based Heuristic (Oldest 28) |
| :--- | :--- | :--- |
| **Total Cost Avoidance** | **$336,458.10** | $213,024.57 |
| **Net Mitigation Cost** | **$152,000.00** | $194,000.00 |
| **Net Enterprise Value** | **$184,458.10** | $19,024.57 |

### 🚀 Enterprise Efficiency Delta
By scaling these results to the 100,000-pole fleet, the Neara-optimized strategy is projected to create **$16,543,353 in additional net value** compared to the current age-based replacement program.
---

## 🚀 Scaling & Implementation
To assist with the enterprise-wide transition, this repository includes two specific integration guides located in `02_Implementation_Guide.md`:
* **The Neara Engineering SQL Cookbook:** For Database Architects and GIS Analysts.
* **The Neara Engineering Excel Cookbook:** For Financial Analysts and Asset Managers.

---

## 📧 Support & Documentation
For technical inquiries regarding physics-engine parameters or data normalization logic, please consult the `01_Strategy_and_Approach.md` document or the **Executive Presentation** in `/docs`.

---
<p align="center">
  <img src="images/neara-icon.png" width="100" alt="Neara Logo"/>
</p>
*© 2026 Neara. Internal Validation Use Only.*
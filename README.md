<p align="center">
<img src="images/neara-banner.png" width="100%" alt="Neara Engineering Banner"/>
</p>

# Engineering Validation Package: Value-Based Pilot

This repository provides the engineering framework, datasets, and validated results for the **1,000-pole pilot cohort**. It demonstrates the financial and operational superiority of physics-based risk modeling over traditional age-based heuristics.

## 📂 Repository Structure & Primary References

For a comprehensive understanding of the project, please refer to the following guides:

| Reference | Description |
| --- | --- |
| **[Strategy & Approach](Strategy_and_Approach.md)** | Strategic overview of Physics-Based vs. Age-Based management. |
| **[Implementation Guide](Implementation_Guide.md)** | Step-by-step technical workflow for reproducing the physics-to-finance model. |
| `/data` | Raw GIS and Asset inputs used for the Digital Twin. |
| `/docs` | Methodology whitepapers and Executive Summary. |
| `/results` | Validated structural reports and ROI Models. |

---

## 🏗 Methodology: "Physics-Based" Asset Management

This pilot transitioned the maintenance strategy for a **1,000-pole cohort** from chronological heuristics to a **High-Fidelity Digital Twin** assessment. The process followed a three-stage integration of financial and physical datasets.

### 1. Decision Logic & Optimization

While the analysis covered the full cohort, the repository highlights the delta between two distinct strategies:

* **Neara Optimized Strategy:** Prioritizes assets based on the highest net enterprise value created.
* **Age-Based Heuristic:** Prioritizes the oldest assets regardless of their physical risk or consequence.

### 2. Financial Parameter Mapping

The process begins by establishing a financial baseline. Enterprise asset datasets are integrated to map standard mitigation costs against theoretical cost avoidance. This stage defines the "Gross ROI" by evaluating the probability and financial consequence of failure before physical environmental factors are considered.

### 3. Physics Modeling & GIS Integration

The Digital Twin creates a dynamic 3D topology of the network. By simulating physical relationships between assets—such as identifies where span failure would result in cascading damage to lower-voltage lines—we quantify "Physics-Based" risk modifiers. This model is then synchronized with the GIS system of record to ensure every physical risk is accurately attributed to a specific asset identifier.

### 4. Physics-to-Finance Consolidation

The final stage merges the physical risk modifiers back into the financial framework. By applying high-fidelity structural consequences to the baseline costs, we produce a "Physics-Informed" Net Cost Avoidance. This allows for a final asset list prioritized by true enterprise value, ensuring capital is deployed where it provides the maximum possible resilience.

---

## 📊 Summary of Pilot Results (N=1000)

Detailed calculations are available in **`/results/Analysis-Results.xlsx`**.

| Metric | Neara Optimized (28 Poles) | Age-Based Heuristic (Oldest 28) |
| --- | --- | --- |
| **Total Cost Avoidance** | **$336,458.10** | $213,024.57 |
| **Net Mitigation Cost** | **$152,000.00** | $194,000.00 |
| **Net Enterprise Value** | **$184,458.10** | $19,024.57 |

### 📈 Enterprise Efficiency Delta

By scaling these results to the 100,000-pole fleet, the Neara-optimized strategy is projected to create **$16,543,353 in additional net value** compared to the current age-based replacement program.

---

## 🚀 Scaling & Support

To assist with the enterprise-wide transition, please see the **[Implementation Guide](Implementation_Guide.md)** for detailed logic regarding:

* **The Physics-Finance Bridge:** For Financial Analysts and Asset Managers.
* **Spatial Key Integration:** For Database Architects and GIS Analysts.

---

<p align="center">
<img src="images/neara-icon.png" width="100" alt="Neara Logo"/>
</p>
*© 2026 Neara. Internal Validation Use Only.*
<p align="center">
  <img src="images/neara-banner.png" width="100%" alt="Neara Engineering Banner"/>
</p>

# Strategic Approach: The Physics-Based Data Bridge

## 1. Executive Overview
Traditional utility asset management often suffers from "Data Silos"—where GIS location data, asset inventory (SAP/Maximo), and engineering simulations live in separate environments. This pilot demonstrates the power of the **Neara Digital Twin** to bridge these gaps, creating a unified model where physical coordinates and financial logic interact.

By moving from an **Age-Based** proxy to a **Physics-Based** model, we have identified a path to creating over **$16.5 Million in annual enterprise value** through CAPEX optimization.

---

## 2. Bridging GIS to the Engineering Model
The foundation of the Digital Twin is the "Data Bridge"—the process of turning flat spatial files into an interactive physics environment.

### Data Ingestion & Topology
The model ingests raw spatial data from the following sources (located in `/data`):
* **`Poles.geojson` & `Spans.geojson`**: The "System of Record" for the network's geometry.
* **The Simulator Environment**: Neara ingests these features to build a 1:1 physical topology, connecting spans to poles based on spatial proximity.

### Coordinate Snapping & Manual Data Cleanup
A critical phase of this pilot involved the "Data Bridge"—aligning the physical asset metadata with the spatial nodes in the GIS layers. 

* **The Challenge:** The simulator does not automatically align disparate datasets where coordinates vary between GIS records and engineering surveys. In this pilot, the "snap to grid" process required manual intervention to resolve discrepancies.
* **The Process:** We performed a manual cleanup to "snap" asset coordinates to the model's grid. This involved matching `Task 2_ Pole IDs` to the master `Asset List.csv` using specialized proximity logic and **Height Segmentation**.
* **Height Segmentation:** This technique was used to distinguish between overlapping line runs that exist at different vertical elevations, ensuring the metadata was attached to the correct physical asset.
* **Technical Workflow:** Detailed documentation of the cleanup functions, including coordinate alignment and key matching, is found in **`02_Implementation_Guide.md`**.

---

## 3. The Physics-Based Methodology
Once the data bridge is established, the cohort is subjected to mechanical simulation.

### Structural Utilization vs. Chronological Age
While age is a common metric, it is a poor predictor of failure.
* **Neara Logic:** We simulate NESC Heavy loading (wind/ice) to identify assets exceeding 80% utilization.
* **Cascading Failure:** We calculate the "Consequence Multiplier" using the **`Task 2_ Consequence modifier.csv`**. This identifies poles that are structurally "critical"—where a single failure would cause multiple overlapping spans to collapse.

---

## 4. Financial Validation (The ROI Delta)
The pilot compared the **Neara Optimized** strategy against the **Age-Based Heuristic** (replacing the oldest 28 poles).

| Metric | Age-Based Heuristic | Neara Optimized |
| :--- | :--- | :--- |
| **Selection Logic** | Oldest 28 Assets | Physics-Based Risk |
| **Total Cost Avoidance** | $213,024.57 | **$336,458.10** |
| **Net Mitigation Cost** | $194,000.00 | **$152,000.00** |
| **Net Value Created** | $19,024.57 | **$184,458.10** |

### The Efficiency Delta
The Neara strategy yielded a **$165,433.53 Net Value Delta** over the traditional approach. By targeting the "Physics-Verified" risk, we achieved significantly higher resilience with **21% less capital expenditure**.

---

## 5. Enterprise Scalability (100x Projection)
Scaling this "Value Delta" to a 100,000-pole enterprise fleet demonstrates the transformative potential of the Digital Twin:

### **Projected Enterprise ROI Delta: $16,543,353.00**

This represents the *additional* net value created annually by shifting from "random" age-based spend to "risk-verified" physics-based spend.

---
<p align="center">
  <img src="images/neara-icon.png" width="100" alt="Neara Logo"/>
</p>
*© 2026 Neara. Internal Validation Use Only.*
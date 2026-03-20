# Executive Supply Chain Performance Dashboard - Excel

A comprehensive, interactive Supply Chain analytics solution built entirely in **Microsoft Excel**. This project transforms raw logistics data into a high-level executive tool to optimize margins and mitigate transport risks.

## Project Overview
This dashboard provides a "Single Pane of Glass" view into global supply chain operations. It tracks **$577K in Revenue** and identifies critical bottlenecks in transportation and inventory management using advanced Excel visualization techniques.

### Key Business Insights
* **Profitability vs. Risk:** Identified a **54% Profit Margin**, with the West Coast Hub outperforming others at **57.04%**.
* **Quality Failure Point:** Isolated **Road Transport** as a primary risk factor, contributing to a **76.01% relative defect rate**.
* **Inventory Optimization:** Analyzed 100+ SKUs via Scatter Plot to categorize "Zombies" (Dead Capital) and "Stockout Risks" (High Velocity).

---

## Data Dictionary & Business Logic

To ensure data integrity, the following columns and calculated fields were utilized:

| Column Name | Description | Business Logic / Formula |
| :--- | :--- | :--- |
| **Total Revenue** | Gross sales generated per SKU. | `Units Sold * Unit Price` |
| **Total Profit** | Net earnings after all costs. | `Revenue - (Manufacturing + Shipping Costs)` |
| **Profit Margin (%)** | Efficiency of each sale. | `(Total Profit / Total Revenue) * 100` |
| **Defect Rate (%)** | Quality indicator for transport. | `(Damaged Units / Total Units Shipped) * 100` |
| **Lead Time** | Speed of supply chain. | `Arrival Date - Order Date` |
| **Stock Level** | Current inventory in hand. | Raw count used for Scatter Plot (X-Axis) |

> **Note:** All financial KPIs were aggregated using **Average (AVG)** in Pivot Tables to provide accurate regional benchmarking, avoiding "Volume Bias" from larger hubs.

## Dashboard Architecture

### 1. Dynamic KPI Header
* **Total Revenue & Net Profit:** Real-time financial tracking.
* **Global Defect Rate:** A "Code Red" indicator set at **2.28%** to trigger immediate quality audits.
* **Avg. Profit Margin:** Calculated using `Average` logic to ensure fair comparison across hubs.

### 2. Operational Performance & Quality (Center)
* **Profit Margin by Regional Hub:** A clustered bar chart sorted by performance to identify high-efficiency "Best Practices."
* **Shipping Cost vs. Speed:** A dual-axis (Secondary Axis) analysis of Carrier performance (Lead Time vs. Shipping Cost).
* **Defect Analysis:** Breakdown of quality issues by **Transport Mode** and **Supplier** using conditional color formatting (Red for high-risk).

### 3. Inventory Intelligence (Bottom-Left)
* **Units Sold vs. Stock Level:** A scatter plot analysis to visualize supply-demand gaps.
    * **Top-Left:** High sales, low stock (**Urgent Restock**).
    * **Bottom-Right:** Low sales, high stock (**Liquidate/Clearance**).

---

## Strategic Recommendations
Based on the data, the following actions were proposed:
1. **Logistics Pivot:** Transition high-value Skincare volume from **Road to Rail** to reduce 76% defect rates.
2. **Operational Benchmarking:** Replicate the West Coast Hub’s logistics model across South Asia and Tech centers.
3. **Supplier Audit:** Review **Apex Manufacturing** due to high lead-time volatility (16.8 days avg).

---

## Excel Technical Stack
* **Data Modeling:** Pivot Tables and Pivot Charts for dynamic data aggregation.
* **Advanced Formulas:** Used `IFS`, `AVERAGEIF`, and custom Margin calculations `(Profit / Revenue)`.
* **Interactive UI:**
    * **Slicers:** Connected to multiple Pivot Tables for global filtering by Region and Carrier.
    * **Conditional Formatting:** Automated visual alerts for negative margins and quality thresholds.
    * **Shape UI:** Custom-built layout using Excel shapes for a modern "Software" look.

---

## How to Use
1. Download the [Excel file - dashboard](supplychain_analysis_dashboard.xlsx) file.
2. Dataset file - csv [uncleandataset](sypplychain_dataset.csv)
3. ScreenShot of dashbaord - [dashboard](supplychain_dashbboard_image.png)
4. Use the **Right Sidebar Slicers** to filter data by region or product type.
5. Observe the **Strategic Summary** on the right for automated executive conclusions.

---

##### Connect with Author: 
On [LinkedIn](https://www.linkedin.com/in/maria-aslam-458860316/)

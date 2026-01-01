📊 Revenue Leakage Detection Dashboard

Discount & Billing Variance Analysis (Excel Project)

📌 Project Overview

Revenue leakage directly impacts profitability due to excess discounts, billing mismatches, and lack of monitoring. This project identifies, analyzes, and visualizes revenue leakage drivers using an interactive Excel dashboard to support data-driven decision-making.

The solution focuses on detecting leakage, understanding root causes, and recommending corrective actions.

🎯 Objectives

Detect revenue leakage caused by discount violations and billing errors

Quantify leakage impact using meaningful KPIs

Identify high-risk categories, products, and time periods

Provide actionable recommendations to reduce revenue loss

🧩 Dataset Description

Records: 1,200+ sales transactions

Time Period: 6 months

Dimensions:

Region

Salesperson

Product

Category & Sub-Category

Key Fields

Order_ID

Order_Date

Standard_Price

Quantity

Allowed_Discount_Percent

Applied_Discount_Percent

Actual_Billed_Amount

🧠 Data Modeling & Logic Derived Metrics

Expected Revenue

Standard_Price × Quantity × (1 − Allowed_Discount%)

Revenue Difference

Expected Revenue − Actual Billed Amount

Discount Violation

Applied_Discount% > Allowed_Discount%

Leakage Flag

LEAKAGE → Revenue Difference > 0

OK → Otherwise

Leakage Reason

Excess Discount

Billing Error

No Issue

This logic enables automated identification of leakage cases at transaction level.

📈 Key Performance Indicators (KPIs)

Total Revenue Leakage (₹)

Leakage Percentage (%)

Total Orders

Leakage Orders Count

Leakage per Affected Order (₹) (normalized metric)

These KPIs capture both scale and severity of revenue loss.

📊 Dashboard Features Visual Analysis

Leakage by Category – Highlights high-impact business segments

Top Leakage-Contributing SKUs – Prioritizes products for audit

Monthly Leakage Trend – Identifies seasonal or campaign-driven spikes

Leakage Cause Distribution – Breaks down leakage by root cause

Interactivity

Slicers: Region, Salesperson, Category

Timeline: Order Date

All charts and KPIs are fully synchronized

🔍 Key Insights

~78% of revenue leakage is driven by excess discounts, not billing errors

Electronics contributes over 55% of total leakage, driven by high-value SKUs

Leakage peaks in April and June, aligning with promotional discount periods

A small group of products accounts for a disproportionate share of total loss

✅ Recommendations

Enforce discount approval limits for high-value Electronics SKUs

Conduct weekly audits on top leakage-contributing products

Implement pre-billing validation checks for discount violations

Track leakage per order to detect systemic issues early

These actions focus on prevention, not just detection.

⚠️ Assumptions & Limitations

Assumes standard pricing data is accurate

Margin impact not calculated due to lack of cost data

Analysis is directionally strong and suitable for operational decisions

Future enhancements may include margin-level analysis and automated alerts.

🛠 Tools & Techniques

Microsoft Excel

Pivot Tables & Pivot Charts

Slicers & Timelines

GETPIVOTDATA-based KPIs

Analytical storytelling & dashboard design best practices

🏁 Conclusion

This project demonstrates an end-to-end data analytics workflow:

Problem definition

Metric design

Root cause analysis

Interactive visualization


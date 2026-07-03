# Telemarketing Funnel & Channel Performance Analysis

## Project Overview
This project analyzes a banking telemarketing campaign to identify bottlenecks in the customer conversion funnel and evaluate the performance of different communication channels.

## Tools & Technologies Used
* **Data Engineering:** Python (Pandas) for standardizing categorical data and mapping binary funnel stages.
* **Data Visualization:** Power BI for interactive funnel mapping and channel filtering.
* **Dataset:** UCI Bank Marketing Dataset (Engineered for Funnel Velocity).

---

## Core Business Problem
The bank is successfully generating leads but needs to understand exactly *where* prospects are dropping off during the sales call (Awareness -> Consideration -> Conversion) and which communication channels yield the highest ROI.

## Key Insights

### 1. The "Closing" Bottleneck
* The overall campaign achieved an **11.70%** conversion rate.
* **Top of Funnel:** 45,000 total leads were contacted.
* **Middle of Funnel:** A highly successful 31,000 leads (68%) stayed engaged on the phone for over 2 minutes.
* **Bottom of Funnel (The Drop-off):** Only 5,000 of the engaged leads ultimately converted. The data proves the sales team is highly effective at opening the call, but the actual product pitch is failing to close the deal.

### 2. Channel Disparities
* **Cellular contacts** yielded the highest conversion rate at **14.92%**.
* Traditional landline telephones underperformed at **13.42%**.
* "Unknown" contact types converted at an abysmal **4.07%**, draining call center resources.

---

## Actionable Recommendations
1. **A/B Test the Closing Pitch:** Since the massive drop-off occurs after the 2-minute mark, the bank should implement A/B testing on the actual deposit offer (e.g., promotional interest rates) to improve bottom-funnel velocity.
2. **Prioritize Mobile Leads:** Marketing teams should allocate more budget toward acquiring verified cellular numbers, as they convert at a noticeably higher rate than landlines.
3. **Purge "Unknown" Data:** Leads missing contact-type metadata should be purged from the manual call list and pushed to automated email campaigns to save call center hours.

---

## Repository Structure
* `bank-full.csv` - The original uncleaned campaign dataset.
* `bank_funnel_clean` - The engineered dataset mapped for funnel tracking.
* `telecoms funnel analysis.ipynb` - The Python script used for data cleaning and funnel engineering.
* `telecoms funnel dashboard.pbix` - The final interactive Power BI dashboard.
* `Telemarketing Funnel & Channel Performance Report.pdf` - The final executive summary of findings.

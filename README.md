# 🛍 Retail Sales Analysis – Power BI Personal Project

This is my first **data analysis project**, which is also my **final assignment for the Power BI course at Datapot**: *Retail Sales Analysis*.  It was evaluated by the teachers at Datapot as the best project of this course.

The dataset, containing retail sales data from **2014**, was sourced from **Obvience.com**.  

**Link to the dataset:** [Retail Analysis sample for Power BI](https://learn.microsoft.com/en-us/power-bi/create-reports/sample-retail-analysis)

---

## 1. Project Overview

### About the Company
- A retail company operating two store chains: **Fashion Direct** and **Lindseys**.
- Store branches are primarily located in the **Southeastern United States**.
- Product categories include **Fashion**, **Grocery**, and **Home Goods**.

### Report Objectives
- Provide an **overview** of the company’s sales performance in 2014.
- Offer **detailed insights** into the sales performance of each chain for District Managers.
- Identify **key challenges** and propose **data-driven recommendations** to improve future sales.

### Key Questions Answered
1. How was the company’s overall sales performance in 2014?  
2. How did the two store chains (Fashion Direct and Lindseys) perform under District Managers’ supervision?  
3. What challenges negatively impacted sales performance?  
4. What recommendations can help improve sales in the future?  

### Power BI Tools & Techniques Used
- **DAX** (YoY growth, COGS calculations, etc.)
- **Top N** filtering
- **Tooltips**
- **Dynamic Dimension**
- **Conditional Formatting**

---

## 2. Key Findings

**1/ Fashion Direct dominates revenue despite having fewer stores.**
Fashion Direct generated **$32.01M (70.84% of total revenue)** across only 37 stores, while Lindseys produced **$13.17M** across 67 stores. Fashion Direct's sales per sq ft ($13.25 avg) also outpaces Lindseys ($12.81 avg), confirming a clear efficiency gap between the two chains.

**2/ Total sales nearly doubled YoY, but unit volume declined.**
Overall sales grew **95.33% YoY** to $45.18M with gross margin improving slightly to **42.29% (+1.45%)**. However, total units sold dropped from 4.46M to 4M **(-9.99%)**, suggesting growth was driven by price increases rather than volume - a potential risk if pricing power weakens.

**3/ Sales dip sharply in May and July.**
The monthly trend shows revenue falling to **$5.4M in May** and **$5.6M in July**, sandwiched between stronger months. These mid-year dips are consistent and appear unmanaged. There is no visible promotional response in either period.

**4/ Revenue is heavily concentrated in 3 categories.**
Men's ($8.91M), Shoes ($7.22M), and Juniors ($6.04M) together account for **about $22M to nearly 49% of total sales**. Meanwhile, Women's (-33.30% sales growth), Hosiery (-15.25%), and Intimate (-10.79%) are all declining, signaling a shrinking customer base in key segments.

**5/ Cost growth is outpacing category performance in several segments.**
Home's cost grew **107.66%** while sales grew only 4.79%. Accessories cost grew **100.46%** on 8.34% sales growth. These mismatches point to margin pressure that is not visible at the top-line level.

**6/ Regional demand varies significantly across territories.**
Ohio (OH) and Pennsylvania (PA) lead in both units and sales volume, while states like Delaware (DE) and Tennessee (TN) sit at the bottom. The category mix also shifts by territory - a uniform stocking strategy across all regions is likely leaving revenue on the table.

---

## 3. Recommendations

> **Applying the Pareto method to define main problems:** Two problems account for the majority of the business's underperformance are:
> **(1) Lindseys' structural inefficiency** dragging down overall margins and 
> **(2) accelerating decline in Women's, Hosiery, and Intimate categories** shrinking the customer base.
> Fixing these two delivers the highest return before optimizing everything else.


### 🔴 Priority 1: Lindseys is underperforming at scale

**The Problem:**
Lindseys operates 67 stores (64% of the total network) but generates only $13.17M - just 29.16% of company revenue. Its gross margin growth is already negative (-0.24% YoY). At the district level, Brad Sutton's 14 stores are actively losing margin (-0.41%). Fashion Direct, with 37 stores, produces $32.01M at a 41.83% gross margin. The gap isn't marginal - it's structural.

**Actions & Timeline:**

| Action | Timeline | Details |
|---|---|---|
| Store-level P&L audit across all 67 Lindseys locations | Short-term (Q1–Q2 2015) | Identify bottom 15–20% of stores by revenue/sq ft and gross margin |
| Close or consolidate underperforming stores | Short-term (Q3–Q4 2015) | Start with Brad Sutton's district; target ~10–12 store closures |
| Redirect freed capital to Fashion Direct expansion | Mid-term (2016–2017) | Open 8–10 new Fashion Direct locations in OH, PA, NC (top-performing territories) |
| Rebrand or reposition remaining Lindseys stores | Long-term (2017–2018) | Test a format refresh in top 20 Lindseys stores to close the efficiency gap |

**Estimated Impact:**
- Closing 10–12 low-performing Lindseys stores could reduce COGS by an estimated **$1.5M–$2M** while preserving most of the revenue (low-volume stores contribute minimally).
- Redirecting investment to 8–10 new Fashion Direct stores (avg $865K revenue/store) could add **$7M–$8.5M in incremental revenue** by end of 2017.
- Target: raise Fashion Direct's share of total revenue from **70.84% → 80%+** by 2017.
- Target: improve company-wide gross margin from **42.29% → 44–45%** by removing the margin drag from the weakest Lindseys locations.


### 🔴 Priority 2: Women's, Hosiery & Intimate are underperforming

**The Problem:**
Women's (010) posted **-33.30% sales growth** - the steepest decline in the portfolio - on $4.47M in sales. Hosiery (070) dropped **-15.25%** and Intimate (060) fell **-10.79%**. Together, these three categories represent roughly **$7.3M in current revenue** but are on a trajectory that could wipe out a significant portion of that within 1–2 years if unaddressed. Given that Fashion Direct's top category mix skews toward Home, Men's, and Kids, there is likely a merchandising or positioning mismatch for female-oriented segments.

**Actions & Timeline:**

| Action | Timeline | Details |
|---|---|---|
| Root cause analysis: pricing, placement, or product mix? | Short-term (Q1 2015) | Pull SKU-level sell-through data for Women's, Hosiery, Intimate across top 10 stores |
| Run targeted promotions to test price sensitivity | Short-term (Q2–Q3 2015) | Bundle deals, end-of-aisle placement, seasonal campaigns for Women's and Hosiery |
| Refresh product assortment based on findings | Mid-term (2015–2016) | Replace low-sell-through SKUs; pilot new styles in 10–15 test stores before full rollout |
| Build a category recovery KPI dashboard | Mid-term (2016) | Track sell-through rate, units/store, and margin per SKU monthly |
| Evaluate full category investment or exit decision | Long-term (2016–2017) | If Women's recovery stalls below -10% YoY after intervention, consider reducing SKU range and reallocating shelf space to Kids and Juniors |

**Estimated Impact:**
- Stabilizing Women's decline from -33.30% to flat (0% growth) by end of 2015 would recover an estimated **$1.5M–$2M** in revenue at the current category size.
- If Hosiery and Intimate are stabilized at -5% or better by mid-2016, combined revenue preservation across the three categories is approximately **$800K–$1.2M**.
- Longer term: if Women's returns to modest growth of +5–8% by 2017, it could contribute an additional **$200K–$350K** in incremental revenue annually.
- Secondary benefit: recovering female-oriented categories strengthens Fashion Direct's appeal to a broader shopper demographic, supporting store traffic across all categories.
---

## 4. Limitations & Areas for Improvement

- **Dataset limitations:**
  - Restricted dataset (only until August 2014).
  - Certain key metrics not fully connected logically.
  - Outdated data; need to work with more recent datasets for practice.
  
- **Report design improvements:**
  - Limit the color scheme to **2–3 main colors**.
  - Reduce the number of charts per page to avoid visual clutter.

---

## 5. Lessons & Takeaways

- Working with this dataset taught me how to move beyond describing numbers - the real skill is connecting data patterns to business decisions that someone can actually act on.
- I deepened my technical understanding of DAX, dynamic dimensions, and conditional formatting, learning how to build dashboards that are genuinely useful rather than just visually clean.
- Most importantly, this project shifted my thinking from reporting what happened to asking why it happened and what should be done next, which is the core of what business analysis is about.

---

## 📸 Dashboard Preview

<img width="1282" height="743" alt="Screenshot 2025-08-13 181015" src="https://github.com/user-attachments/assets/d0d183a9-48a9-4d29-a471-803692d6adb4" />

<img width="1282" height="751" alt="Screenshot 2025-08-13 181037" src="https://github.com/user-attachments/assets/f08ed510-15f2-4ac6-a62c-1fe78c9f6e2d" />

<img width="1278" height="748" alt="Screenshot 2025-08-13 181102" src="https://github.com/user-attachments/assets/8744d7ba-8677-4b96-8269-c308c2bf90ac" />

<img width="1276" height="741" alt="Screenshot 2025-08-13 181122" src="https://github.com/user-attachments/assets/7517e70d-2cf7-4daf-8e5d-c549754189e7" />

<img width="1283" height="747" alt="Screenshot 2025-08-13 181140" src="https://github.com/user-attachments/assets/8e4f512b-b705-45d2-9003-3155eef2e2af" />

## 📸 Data Model

<img width="1919" height="813" alt="Screenshot 2025-02-26 125317" src="https://github.com/user-attachments/assets/5be1c2bf-d34a-4d68-ab65-af8185759f66" />




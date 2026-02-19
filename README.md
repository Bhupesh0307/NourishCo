# 🥤 NourishCo — D2C Growth Funnel & CAC Analysis

> **Self-initiated analytics project** | Tools: Python · Excel · PowerBI · DAX  
> **Domain:** Food & Beverage D2C | **Period:** Jan 2024 – Dec 2024

---

## 📌 Project Overview

NourishCo is a simulated **Direct-to-Consumer (D2C) health snacks & beverages brand**. This project replicates a real-world growth analytics workflow — from raw campaign data ingestion to funnel analysis, channel benchmarking, and actionable optimization recommendations.

The goal was to answer three core growth questions:
1. **Where is the acquisition funnel leaking?** (Funnel drop-off analysis)
2. **Which channels deliver the best CAC and ROAS?** (Channel efficiency)
3. **What optimizations would reduce CAC by ~15%?** (Budget reallocation strategy)

---

## 📊 Key Results (FY 2024)

| Metric | Value |
|---|---|
| Total Revenue | ₹1.82 Cr |
| Total Ad Spend | ₹48.6 L |
| Blended ROAS | **3.74×** |
| Blended CAC | **₹167** |
| Overall CTR | 4.36% |
| Overall CVR | 6.56% |
| Total Conversions | 29,093 |
| Total Impressions | 1.02 Cr |

---

## 🔍 Funnel Analysis — Drop-off Points

```
Impressions   10,164,341  ██████████████████████████████  100%
Clicks           443,313  █▏                                4.4%   ▼ 95.6% drop ← CRITICAL
PDP Views        264,002  ▊                                 2.6%   ▼ 40.4% drop
Add to Cart       85,102  ▎                                 0.84%  ▼ 67.8% drop ← HIGH
Checkouts         47,685  ▏                                 0.47%  ▼ 44.0% drop
Conversions       29,093  ▏                                 0.29%  ▼ 39.0% drop
```

### Top 3 Leakage Points & Recommendations

**1. Impressions → Clicks (95.6% drop)**  
Ad creatives are not compelling enough. Google Search and YouTube ads have CTRs below 2%.  
→ *A/B test ad copy, use problem-led hooks, refresh creatives every 3–4 weeks*

**2. PDP Views → Add to Cart (67.8% drop)**  
Users visit product pages but don't convert — weak social proof, poor CTAs, or pricing friction.  
→ *Add verified reviews, before/after imagery, bundle offers, urgency signals*

**3. Add to Cart → Checkout (44% drop)**  
Significant cart abandonment. Common causes: shipping cost surprise, forced login, payment friction.  
→ *Free shipping threshold, guest checkout, retargeting cart abandoners via WhatsApp/Email*

---

## 📡 Channel Performance

| Channel | Avg ROAS | Avg CAC | Avg CTR | Verdict |
|---|---|---|---|---|
| ✅ Email / WhatsApp | **19.89×** | ₹30 | 12.63% | Best — underinvested |
| ✅ Google Display | 5.94× | ₹98 | 0.64% | Efficient, scale up |
| 🟡 YouTube Ads | 3.78× | ₹170 | 1.53% | Average — optimize creatives |
| 🟡 Meta Ads | 2.82× | ₹229 | 3.00% | High volume, low efficiency |
| 🔴 Influencer | 2.55× | ₹278 | 4.06% | Poor ROAS — review contracts |
| 🔴 Google Search | 1.58× | ₹486 | 4.77% | Underperforming — reduce spend |

---

## 💡 Optimization Strategy — Reduce CAC by ~15%

**Problem:** ₹21.87L (45% of budget) is spent on Google Search + Influencer, generating only 2.1× ROAS combined.

**Proposed Reallocation:**

| Action | Budget Impact | Expected CAC Impact |
|---|---|---|
| Cut Google Search broad match spend by 30% | −₹6.6L | −₹18 CAC |
| Reduce Influencer spend, keep only high-ROI creators | −₹4L | −₹12 CAC |
| Invest in Email list growth & automation | +₹4L | −₹8 CAC (compounding) |
| Scale Google Display (proven 5.94× ROAS) | +₹2L | Neutral |

**Projected outcome:** Blended CAC ₹167 → **~₹142** (−15%) at same total budget

---

## 🗂 Project Structure

```
NourishCo_D2C_PowerBI_Dataset.xlsx
│
├── 📋 Campaign Data          → 864 rows | 6 channels × 12 months | 19 metrics
├── 📊 Monthly Summary        → 12 rows | blended KPIs + Revenue vs Spend chart
├── 📡 Channel Summary        → 6 rows | ranked by ROAS | color-scaled formatting
├── 🔻 Funnel Analysis        → Stage-by-stage drop-off | funnel bar chart
├── 📅 Quarterly Summary      → Q1–Q4 comparison
├── ⚡ PowerBI DAX Measures   → 15 copy-paste DAX formulas
└── 🗺 PowerBI Visual Guide   → 10 recommended visuals with field mapping
```

---

## ⚡ PowerBI Dashboard Setup (Quick Start)

1. Open PowerBI Desktop → **Get Data → Excel** → select `NourishCo_D2C_PowerBI_Dataset.xlsx`
2. Load sheets: `Campaign Data`, `Monthly Summary`, `Channel Summary`, `Funnel Analysis`
3. Go to **Data View** → open `PowerBI DAX Measures` sheet → copy DAX formulas into **New Measure**
4. Build visuals per the `PowerBI Visual Guide` sheet — suggested 5-page layout:

| Page | Key Visuals |
|---|---|
| Overview | 6 KPI cards · Revenue vs Spend bar · Spend donut |
| Funnel | Funnel visual · Drop-off table · Stage bar chart |
| Channels | CAC vs ROAS scatter · Channel ranking table · CTR bar |
| Trends | CAC trend · ROAS trend · CVR & CTR lines |
| Optimization | What-if parameter sliders · Budget reallocation impact |

---

## 🛠 Tech Stack

| Tool | Usage |
|---|---|
| **Python** (pandas, numpy, openpyxl) | Data simulation, aggregation, Excel generation |
| **Excel** | Structured dataset, conditional formatting, embedded charts |
| **PowerBI** | Interactive dashboard (DAX measures + visual guide included) |
| **DAX** | 15 custom measures: ROAS, CAC, CVR, MoM Growth, Retention Rate |

---

## 📁 Files

| File | Description |
|---|---|
| `NourishCo_D2C_PowerBI_Dataset.xlsx` | Main dataset — 7 sheets, fully formatted |
| `NourishCo_Growth_Dashboard.html` | Standalone interactive dashboard (no install needed) |
| `generate_data.py` | Python script — full data generation & analysis pipeline |
| `README.md` | This file |

---

## 🖥 Dashboard Preview

| Overview | Funnel Analysis |
|---|---|
| ![](assets/overview.png) | ![](assets/funnel.png) |

| Channel Performance | Optimization |
|---|---|
| ![](assets/channels.png) | ![](assets/optimization.png) |

---

## 👤 Author

**Bhupesh Jha** — Growth & Product Analyst  
📧 bjha0307.work@gmail.com · [LinkedIn](https://www.linkedin.com/in/bhupesh-jha-09aa5323a/) · [GitHub](https://github.com/Bhupesh0307) · [Portfolio](https://bhupesh-portfolio-mu.vercel.app/)

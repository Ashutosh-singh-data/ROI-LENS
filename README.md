<div align="center">

# ROI Lens
### Advanced Marketing Attribution & Budget Refinement

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green)
![NumPy](https://img.shields.io/badge/NumPy-Scientific%20Computing-orange)
![Markov Chain](https://img.shields.io/badge/Attribution-Markov%20Chain-red)
![Status](https://img.shields.io/badge/Project-Completed-success)

</div>

---

## 📌 Project Overview

ROI Lens is a marketing attribution and budget optimization system that replaces traditional Last-Click Attribution with a Markov Chain based multi-touch attribution model.

The project analyzes complete customer journeys, calculates the true contribution of each marketing channel, and recommends an optimized budget allocation strategy based on channel effectiveness.

---

## 🎯 Problem Statement

Traditional Last-Click Attribution assigns 100% credit to the final touchpoint before conversion.

Example:

```text
YouTube → Instagram → Google Search → Marketplace → Purchase
```

Last-Click gives all credit to **Marketplace**, ignoring the contribution of the previous channels.

This leads to:

- Underfunding top-funnel channels
- Over-investment in closing channels
- Misleading ROI calculations
- Poor budget allocation decisions

---

## 🚀 Solution

ROI Lens implements a 3-stage analytics pipeline:

### Stage 1 — Data Integrity
- Detect and remove bot traffic
- Validate customer journey data
- Prepare clean datasets

### Stage 2 — Markov Chain Attribution
- Build transition probability matrices
- Calculate channel Removal Effects
- Assign true contribution credit

### Stage 3 — Budget Optimization
- Calculate channel CPA
- Measure ROI
- Reallocate budget based on performance

---

## 📊 Dataset

| File | Description |
|--------|-------------|
| touchpoints.csv | Customer journey interactions |
| user_profiles.csv | Consumer demographics |
| campaign_spend.csv | Campaign budgets and costs |

Total Records: **566,510+**

---

## ⚙️ Project Pipeline

1. Data Overview
2. Bot Detection
3. Journey Reconstruction
4. Transition Matrix Creation
5. Removal Effect Calculation
6. Attribution Scoring
7. CPA Calculation
8. ROI Analysis
9. Budget Reallocation
10. Visualization

---

## 🔑 Key Findings

### Bot Traffic
- 3,155 fake users detected
- Represented 3.2% of total traffic

### YouTube Overfunded
- ₹26.60 Cr spent
- Near-zero attribution impact

### Instagram Underfunded
- Highest efficiency channel
- Only ₹61 Lakh budget allocated

### Influencer Blogs
- Significantly undervalued by Last-Click Attribution
- Received 40%+ attribution in Markov model

### Marketplace Over-Credited
- Last-Click assigned 40–50% credit
- True contribution approximately 13%

---

## 💰 Budget Reallocation Summary

| Channel | Old Budget | New Budget |
|----------|-----------|-----------|
| YouTube | ₹26.60 Cr | ₹2.66 Cr |
| Instagram | ₹19.41 Cr | ₹10.54 Cr |
| Google Search | ₹20.30 Cr | ₹26.81 Cr |
| Marketplace | ₹24.06 Cr | ₹29.32 Cr |
| Influencer Blog | ₹11.49 Cr | ₹30.68 Cr |

---

## 🧠 Attribution Methodology

### Removal Effect Formula

```python
Removal Effect =
(Baseline Conversion Rate - Conversion Rate Without Channel)
/
Baseline Conversion Rate
```

Channels causing the largest drop in conversion probability receive the highest attribution credit.

---

## 🛠️ Tech Stack

### Languages
- Python

### Libraries
- Pandas
- NumPy
- Matplotlib
- Seaborn
- DuckDB

### Concepts
- Markov Chains
- Multi-Touch Attribution
- Budget Optimization
- Customer Journey Analytics

---

## 📂 Project Structure

```text
ROI_Lens/
│
├── Markov Chain Model Simulator.md
├── ROI_Lens.ipynb
├── campaign_spend.csv
├── touchpoints.csv
├── user_profiles.csv
│
├── outputs/
│   ├── attribution_heatmap.png
│   ├── last_click_heatmap.png
│   ├── cpa_heatmap.png
│   ├── budget_comparison.png
│   └── markov_chain_transition_matrix_B01.png
│   
├── Presentation/
│   └── ROI_LENS_(Presentation).pdf
│
└── README.md
```

---

## 👨‍💻 Author

**Ashutosh Singh**  
B.Tech Production & Industrial Engineering  
Motilal Nehru National Institute of Technology Allahabad (MNNIT)  
Batch 2025–2029

---

⭐ If you found this project interesting, consider giving it a star.

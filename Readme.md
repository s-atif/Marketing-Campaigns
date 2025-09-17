# 📊 A/B Testing on Marketing Campaigns

Marketing teams constantly run **campaigns** to improve sales, but not all campaigns perform equally. To make data-driven decisions, we apply **A/B testing** to evaluate which campaigns significantly impact sales across outlets.

📓 **Notebook:** [AB_testing.ipynb](https://github.com/s-atif/Marketing-Campaigns/blob/main/AB_testing.ipynb)

---

## 🧩 Problem Description

We aim to analyze the effectiveness of **three marketing campaigns** on sales data collected from **137 outlets** across different **market sizes** (Small, Medium, Large).  

The dataset includes:  
- **OutletID**  
- **MarketSize**  
- **Age of Outlets**  
- **Campaigns (1, 2, 3)**  
- **Week (1–4)**  
- **SalesInThousands**

Using **EDA** and **A/B testing (t-tests)**, we evaluate if differences in sales performance between campaigns are statistically significant.

---

## 💡 Why A/B Testing?

Businesses need to know **which campaign works best** to allocate resources efficiently.  
A/B testing provides:  
- ✅ Evidence-based decision-making  
- 📈 Improved ROI on marketing spend  
- 🛒 Understanding of campaign effectiveness across outlet demographics  
- 🎯 Better targeting of promotions  

---

## 🔍 Approach

1. **Data inspection & cleaning**  
   - No missing values (548 rows × 6 columns)  
   - Unique outlets: 137  

2. **Exploratory Data Analysis (EDA)**  
   - Sales distribution across campaigns  
   - Campaign performance by **market size**  
   - Age of outlets distribution  

3. **Statistical Testing (t-tests)**  
   - Compare mean sales between campaigns  
   - Validate statistical significance using **p-values (< 0.05)**  

---

## 📐 Results of A/B Testing

### Campaign Means

| Campaign | Mean Sales (k$) |
|----------|------------------|
| **1**    | 58.10            |
| **2**    | 47.33            |
| **3**    | 55.36            |

---

### 🔬 Hypothesis Testing

- **Campaign 1 vs Campaign 2**  
  - *t = 6.43, p ≈ 4.3e-10*  
  - **Significant difference** → Campaign 1 outperforms Campaign 2  

- **Campaign 1 vs Campaign 3**  
  - *t = 1.55, p ≈ 0.12*  
  - **No significant difference** → Both perform similarly  

- **Campaign 2 vs Campaign 3**  
  - *t = -4.88, p ≈ 1.57e-06*  
  - **Significant difference** → Campaign 3 outperforms Campaign 2  

---

## ✅ Conclusions & Insights

- **Best performing campaign:** Campaign 1 (highest average sales).  
- **Weakest campaign:** Campaign 2 (significantly lower performance).  
- **Campaign 3:** Close behind Campaign 1, significantly above Campaign 2.  

**Recommended Actions:**  
- Prioritize **Campaign 1** and **Campaign 3** for future marketing spend.  
- Re-evaluate or redesign **Campaign 2**.  
- Consider variations of Campaign 1 to further optimize.  

---

## 📦 Requirements

```bash
pip install pandas matplotlib seaborn scipy


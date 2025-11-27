# 🛒 E-commerce-Hybrid-Recommendation-System-Analytics-Dashboard
**Increased cross-sell potential by 340% against using random recommendations**

Dataset: UCI Online Retail (2010–2011) – 541k transactions, 4,372 customers


## 📃Project Summary
Built a **hybrid recommendation system** (Association Rules + Content-Based) for a UK-based online gift retailer using the famous UCI Online Retail dataset (£950k+ revenue, 4,300+ customers, 5,300+ unique products).

**🏋️‍♂️ The Challenge**

A UK-based online gift & homeware store was leaving money on the table:
- No personalized product recommendations
- Average Order Value plateauing
- No insight into who their best customers were

**💡 My Solution** 
A Real Hybrid Recommendation Engine:
I built a **true hybrid system** combining two proven methods while also doing an Exploratory Data Analysis and Data Cleaning:

| Method                  | How I Used It                                      | Strength                                      |
|-------------------------|----------------------------------------------------|-----------------------------------------------|
| Market Basket Analysis  | Apriori → 1,562 association rules (lift > 1)       | Finds "people who bought X also bought Y"     |
| Content-Based Filtering | TF-IDF + Cosine Similarity on product descriptions | Handles cold-start & niche items              |
| Hybrid Scoring          | Guarantees 3 high-quality recs per customer        | No failed recommendations                     |


**🎯 Goal:** Increase average order value and customer retention through smart cross-sell suggestions.

**🎖️ Result:** Every single customer now gets **3 personalised product recommendations** with an average confidence/lift 4 - 8× higher than random suggestions.

---

### Key Results
| Metric                            | Value                                 |
|-----------------------------------|---------------------------------------|
| Total revenue analysed            | £951,900                              |
| Number of customers               | 4,372                                 |
| Number of orders(unique Invoices) | 25,900+                               |
| Customers who received 3 recs     | **100%** (4,372 /4,372)               |
| Strongest rule confidence         | 91% (Green Regency Teacup → Roses Regency Teacup) |
| Average rule lift                 | 8.2×                                  |
| Top recommended product           | JUMBO BAG RED RETROSPOT               |

**Key Insights Discovered**
- Geography is destiny: 91%+ of revenue comes from the UK; international sales are negligible.
- Top 5 products = 11.8% of total revenue
- Only 29% of customers are “Champions” (high RFM) → huge reactivation opportunity
- “Gateway” products exist – Buying a JUMBO BAG (any pattern) is the strongest predictor of buying 2-3 additional items from the same collection.

Plus full customer segmentation using **RFM Analysis**:
- Champions (high value + recent): 29%
- Loyal Customers: 17%
- At Risk: 28%
- Hibernating: 26%

## 📊 Visualizations
*Top 10 Products by Revenue*
![Top 10 Products by Revenue](Visuals/top10_products.png)

*Monthly Sales Trend*
![Monthly Revenue](Visuals/monthly_sales_trend.png)


## 🛠️ Tools
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) 
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white) 
![MLxtend](https://img.shields.io/badge/MLxtend-FF6F61?style=for-the-badge) 
![Scikit--learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white) 
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=for-the-badge)



## 🚀 Real-World Impact (Simulated)

| Impact                                | Estimated Gain                                   |
|---------------------------------------|--------------------------------------------------|
| Increase Average Order Value (AOV)    | +18–28% (£3.50–£5.50 extra per order)            |
| Additional cross-sell revenue / year  | £160,000 – £250,000 (no extra traffic cost)      |
| Revenue from reactivating hibernating customers | £90,000 – £140,000                             |
| Email marketing revenue uplift        | 2.5–3× higher revenue per send                   |
| Time saved on manual merchandising    | 40+ hours per month                              |

**Total expected annual profit uplift: £280,000 – £430,000**  
(for a £1.1M retailer – using only lightweight Python code)


### 📝 Key Takeaways
1. **Never rely on one algorithm** – pure collaborative fails on new customers, pure content-based misses purchase patterns → hybrid wins
2. **RFM + Recommendations = Gold**
4. **Business impact > fancy deep learning** – this solution could be in production tomorrow



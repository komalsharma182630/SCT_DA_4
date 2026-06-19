# 📊 Marketing Campaign EDA — Business Insights Report

> Exploratory Data Analysis on a marketing campaign dataset to analyze customer behavior, visualize the marketing funnel, calculate ROI per channel, and recommend budget allocation.

---

## 📌 Objective

Instead of building a Machine Learning model, this project focuses on the **"Why"** — cleaning the data, visualizing the funnel, and writing a business insights report that recommends **which marketing channels should receive more budget based on ROI**.

---

## 📁 Dataset

| Property | Details |
|---|---|
| File | `marketing_campaign.csv` |
| Total Customers | 2,240 |
| Total Features | 29 |
| Source | Marketing Campaign Dataset |

**Data Includes:**
- Customer demographics (Age, Education, Marital Status)
- Income information
- Product spending (Wines, Fruits, Meat, Fish, Sweets, Gold)
- Purchase channels (Web, Catalog, Store)
- Campaign responses

---

## 🧹 Data Cleaning

| Step | Action |
|---|---|
| Missing Values | Filled 24 missing `Income` values using **median imputation** |
| Duplicates | Identified and removed duplicate records |
| Irrelevant Columns | Dropped `ID`, `Z_CostContact`, `Z_Revenue` |
| Feature Engineering | Created `Age`, `Age_Group`, `Total_Spending`, `Total_Purchases` |

---

## 📈 EDA Visualizations

| # | Chart | Purpose |
|---|---|---|
| 1 | Customer Age Distribution | Understand age spread of customers |
| 2 | Income Distribution | Identify income range of customer base |
| 3 | Product Category Spending | Find top revenue-generating products |
| 4 | Income vs Spending Scatter | Correlate income with spending behavior |
| 5 | Campaign Response Pie Chart | Measure overall campaign success rate |
| 6 | Age Group vs Response | Find most responsive age segment |
| 7 | Education vs Spending | Analyze spending by education level |
| 8 | Purchases by Channel | Compare Web, Catalog, Store volume |
| 9 | Marketing Funnel Chart | Visitors → Purchases → Conversions |
| 10 | ROI Score Bar Chart | Compare channel efficiency by ROI |
| 11 | Correlation Heatmap | Find relationships between all variables |
| 12 | Customer Segmentation | Low / Medium / High Value segments |

---

## 🔍 Business Questions Answered

| Question | Insight |
|---|---|
| Which customers spend the most? | Customers aged **60+** show the highest average total spending |
| Which products generate maximum revenue? | **Wine** products lead, followed by **Meat** products |
| Which age group responds best? | Customers aged **18–30** have the highest campaign response rate |
| Does income impact spending? | **Yes** — positive correlation between income and spending |
| Which purchase channel is most effective? | **Store** purchases are highest in volume |
| Which customers should be targeted? | **High-income customers aged 18–30** for maximum ROI |

---

## 💰 ROI Analysis — Channel Comparison

ROI Score calculated as:
```
ROI Score = Average Spend × Conversion Rate (%)
```

| Rank | Channel | ROI Score | Budget Recommendation |
|---|---|---|---|
| 🥇 1st | Catalog | Highest | 50% |
| 🥈 2nd | Store | Medium | 30% |
| 🥉 3rd | Web | Growing | 20% |

---

## 📋 Recommendations

1. **Allocate 50% of budget to Catalog channel** — it has the highest ROI Score
2. **Maintain 30% budget for Store channel** — highest purchase volume among all channels
3. **Invest 20% in Web/Digital channel** — best reach for the high-response 18–30 age group
4. **Increase promotions for Wine & Meat products** — they generate the highest revenue
5. **Launch loyalty programs** for High-Value customer segment to improve retention ROI

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Python | Core programming language |
| Pandas | Data loading, cleaning, manipulation |
| NumPy | Numerical operations |
| Matplotlib | Charts and visualizations |
| Seaborn | Statistical visualizations |
| Google Colab | Development environment |

---



## ✅ Conclusion

The analysis revealed that **Catalog** channel delivers the best ROI, while **Wine and Meat** products are the top revenue drivers. High-income customers aged **18–30** are the most responsive segment. By focusing budget on the Catalog channel and targeting this demographic, businesses can significantly improve campaign effectiveness and revenue outcomes.

# 💰 Global Finance & Sales Performance Dashboard — Tableau

An interactive Tableau dashboard covering global finance and sales performance for **2024–2025**. It tracks revenue, profit, margin, budget attainment and customer satisfaction across regions, sales channels and product categories, so finance and sales leaders can see where the business is ahead of or behind its targets.

---

## 🎯 Project Objective

Give finance and sales teams a single view to answer questions like:

- How much revenue and profit are we generating, and at what margin?
- Are we meeting our budget targets, overall and by region?
- Which regions, sales channels and product categories drive the most revenue?
- How does customer satisfaction (CSAT) vary by product category?
- Do higher discounts reduce profit margin?

---

## 🗂️ Dashboard Components

The workbook contains one dashboard built from **12 worksheets**.

| Worksheet | Type | What it shows |
|-----------|------|---------------|
| **KPI – Revenue** | KPI card | Total revenue |
| **KPI – Profit** | KPI card | Total profit (Revenue − COGS) |
| **KPI – Margin** | KPI card | Profit margin % |
| **KPI – Budget Attainment** | KPI card | Revenue as a share of budget target |
| **KPI – CSAT** | KPI card | Average customer satisfaction score |
| **Revenue Trend** | Line chart | Revenue vs. budget target over time |
| **Revenue by Region** | Bar chart | Revenue for each region |
| **Revenue by Channel** | Bar chart | Revenue for each sales channel |
| **Category by Channel** | Matrix | Product category × sales channel view |
| **CSAT by Category** | Bar chart | Average CSAT for each product category |
| **Discount Impact** | Scatter plot | Average discount % vs. profit margin % |
| **Regional Scorecard** | Table | Key measures compared side by side for each region |

---

## 🎛️ Interactivity

- **Filters** on the dashboard: Region, Year and Product Category
- **Cross-filtering** so every chart and KPI card responds to the filters

---

## 🧮 Calculated Fields

| Field | Definition |
|-------|------------|
| **Profit** | `Revenue_USD − COGS_USD` |
| **Profit Margin %** | `SUM(Profit) / SUM(Revenue_USD)` |
| **Budget Variance** | `Revenue_USD − Budget_Target` |
| **Budget Attainment %** | `SUM(Revenue_USD) / SUM(Budget_Target)` |
| **Year** | `YEAR([Date])` |
| **Month Name** | `DATENAME('month', [Date])` |

**Data fields used:** Date, Region, Product Category, Sales Channel, Revenue_USD, COGS_USD, Budget_Target, CSAT, Discount_Percent.

---

## 🛠️ Tools & Techniques

- **Tableau** — worksheets, dashboard design and filters
- **Calculated fields** — profit, margin, budget variance and budget attainment
- **Visualization types** — KPI cards, line, bar, scatter plot, matrix and scorecard table

---

## 📁 Repository Structure

```
├── FINANCIAL_DASHBOARD.twb   # Tableau workbook
└── README.md
```

---

## 🚀 How to Use

1. Download or clone this repository
2. Open `FINANCIAL_DASHBOARD.twb` in **Tableau Desktop** or **Tableau Public**
3. If Tableau asks for the data source, point it to the CSV file the workbook was built on
4. Use the filters to explore the dashboard

---

## 💡 Key Insights

- **Headline numbers:** About **$318M** in revenue and **$169M** in profit, a **53.23%** profit margin, **100%** budget attainment and an average CSAT of **4.2**.
- **Regions:** North America leads with **$87.00M**, followed by EMEA ($81.33M), APAC ($76.58M) and LATAM ($73.05M).
- **Budget attainment:** EMEA is the only region above target (**100.48%**). APAC, LATAM and North America are all just under it, at about 99.9%.
- **Revenue vs. margin:** North America has the highest revenue but the lowest margin (**52.49%**), while LATAM has the lowest revenue but the highest margin (**53.75%**).
- **Sales channels:** Partner (**$109.15M**) and Online ($108.85M) are almost level, and both are ahead of Direct ($99.97M).
- **Category by channel:** Enterprise Software sold through Partners is the strongest combination at **$33.05M**, and Consulting sold Direct is the weakest at **$20.42M**.
- **Customer satisfaction:** CSAT is very even across categories, from 4.22 (Cloud Services) to 4.25 (Hardware).
- **Discounts:** Average discounts sit around 7.3–7.6% and margins stay close to 53% in every category, so the discount level shows no strong effect on margin.
- **Revenue vs. budget:** Monthly revenue follows the budget target closely from April 2024 to December 2025, with somewhat larger swings in 2025.

---

## 👤 Author

**Hammad**

- LinkedIn: [linkedin.com/in/hammad-ali-baig](https://www.linkedin.com/in/hammad-ali-baig)
- GitHub: [github.com/HammadAliBaig-Analytics](https://github.com/HammadAliBaig-Analytics)

Feedback and suggestions are welcome!

# BlinkIT Grocery Sales Analysis

An end-to-end data analytics project exploring BlinkIT grocery sales data, with data cleaning, exploratory analysis, an interactive executive dashboard, and a final internship report.

## Project overview

This project analyzes grocery sales performance across product categories and outlet characteristics. It focuses on answering practical business questions such as which categories contribute most to sales, how outlet types compare, and which outlets and products lead or lag.

## Key findings

| Metric | Result |
|---|---:|
| Total sales | 1,201,681.49 |
| Average sales per record | 140.99 |
| Unique products | 1,559 |
| Outlets represented | 10 |
| Average item rating | 3.97 / 5 |
| Records analyzed | 8,523 |

- **Fruits and Vegetables** and **Snack Foods** are the two largest sales categories, together contributing about **29.4%** of total sales.
- **Supermarket Type1** accounts for approximately **65.5%** of recorded sales.
- **Tier 3** locations contribute about **39.3%** of sales.
- **OUT035** is the top-performing individual outlet by total sales in this dataset.

> Sales values are presented as recorded in the source dataset. The dataset does not establish a currency, costs, or profit, so sales should not be interpreted as profit.

## Repository structure

```
BlinkIT-Grocery-Sales-Analysis/
├── Dashboard/
│   └── index.html
├── Dataset/
│   └── BlinkIT_Grocery_Data.xlsx
├── Output/
│   └── Cleaned_BlinkIT_Data.csv
├── Reports/
│   └── BlinkIT_Final_Report.pdf
└── README.md
```

## Dashboard

The interactive dashboard includes KPI cards and visualizations for category sales, outlet type, outlet location tier, outlet rankings, top products, and correlations with sales.

**[Open the interactive dashboard](https://yaksh2926.github.io/BlinkIT-Grocery-Sales-Analysis/)**

GitHub Pages must be enabled for the repository (Settings → Pages → Deploy from a branch → `main` → `/ (root)`) and the dashboard must be placed at the repository root as `index.html` or under the configured publishing directory.

## Tools and technologies

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Plotly (interactive dashboard)
- Microsoft Excel

## Data preparation

- Standardized inconsistent labels in `Item Fat Content` (for example, `LF`, `low fat`, and `reg`).
- Imputed missing `Item Weight` values using the median for the same item identifier, followed by the overall median where needed.
- Preserved potential outliers rather than deleting observations automatically.

## Important limitations

- The dataset contains no explicit transaction date, cost, margin, profit, or customer identifier fields.
- Correlations with available numeric fields are very weak and should not be treated as causal evidence.
- Product and outlet comparisons describe this dataset only; they do not establish reasons for performance differences.

## Author

**Yaksh Jindal**  
GitHub: [Yaksh2926](https://github.com/Yaksh2926)

---

This project was completed as part of a Data Analyst internship assignment for Sapphire IQ.

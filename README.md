📊 Online Retail II — Exploratory Data Analysis

Overview
This project is a complete Exploratory Data Analysis (EDA) of the **Online Retail II** dataset — real invoice-level transaction data (2009–2010) from a UK-based online retailer. It was completed as part of a Data Analysis & Business Understanding** internship task, with the goal of understanding customer behavior, top-selling products, and revenue drivers before building a product recommendation system.

Objective
Acting as a data analyst, explore the dataset to identify patterns and data quality issues, and produce insights that help the business understand:
- Who its customers are
- Which products sell the most
- Which countries generate the most revenue

Dataset Source: [UCI Machine Learning Repository — Online Retail II](https://archive.ics.uci.edu/ml/datasets/Online+Retail+II)
Size: 525,461 rows × 8 columns
Period: December 2009 – December 2010
Fields:Invoice, StockCode, Description, Quantity, InvoiceDate, Price, Customer ID, Country

What's Inside
- `Online_Retail.ipynb` — full EDA notebook (runs top to bottom without errors)
- `Online_Retail_EDA_Report.pptx` — presentation summarizing findings
- Visualizations: monthly revenue trend, correlation heatmap, outlier box plots

Key Steps Performed
1. Loaded dataset and inspected shape, columns, and data types
2. Identified missing values (20.5% missing `Customer ID`, 0.56% missing `Description`) and duplicate rows (6,865)
3. Analyzed top 10 best-selling products by quantity and by revenue
4. Analyzed sales performance by country
5. Plotted monthly revenue trend
6. Built a correlation heatmap of numerical features
7. Detected outliers in `Quantity` and `Price` using box plots
8. Derived 6 business insights

Key Findings
- 🇬🇧 The UK contributes ~88% of total revenue — high geographic concentration
- 📦 Top sellers by volume ≠ top sellers by revenue (e.g., cheap cake cases vs. the £163K Regency Cakestand)
- ⚠️ ~20.5% of transactions have no linked Customer ID — a constraint for customer-level modeling
- 🚚 "Postage" and "Dotcom Postage" appear in top revenue items — these are fees, not products
- 📈 Revenue is seasonal, trending upward toward the holiday season
- 🧹 6,865 duplicate rows and outliers in Quantity/Price need cleaning before modeling

Tech Stack
- Python
- pandas, NumPy
- Matplotlib, Seaborn
- Jupyter Notebook

How to Run
```bash
pip install pandas numpy matplotlib seaborn openpyxl
jupyter notebook Online_Retail.ipynb
```

Author
Hassan Farooq AI/Ml Engineer

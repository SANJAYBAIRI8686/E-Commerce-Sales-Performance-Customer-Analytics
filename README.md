# E-Commerce Sales Performance & Customer Analytics

<div align="center">
  

A comprehensive data analysis project demonstrating end-to-end analytics skills for business intelligence
</div>
<br>

Table of Contents

Project Overview<br>
Business Context<br>
Features<br>
Demo Screenshots<br>
Dataset Information<br>
Installation<br>
Usage<br>
Project Structure<br>
Analysis Breakdown<br>
Key Results<br>
Technical Skills Demonstrated<br>
Future Enhancements<br>
Contributing<br>
License<br>
Contact<br>


## 🎯 Project Overview
This project presents a comprehensive end-to-end data analysis of an online retail business, covering 397,884 transactions across 13 months. It demonstrates proficiency in:

✅ SQL Query Writing - Complex aggregations, joins, and window functions<br>
✅ Python Data Analysis - Pandas, NumPy, advanced data manipulation<br>
✅ Statistical Analysis - ANOVA, correlation analysis, hypothesis testing<br>
✅ Customer Segmentation - RFM Analysis for targeted marketing<br>
✅ Cohort Analysis - Customer retention and lifecycle metrics<br>
✅ Data Visualization - Professional charts using Matplotlib & Seaborn<br>
✅ Business Intelligence - Actionable insights and strategic recommendations<br>

## 💡 Why This Project Stands Out

Real-World Dataset: UCI Online Retail data with actual business complexity<br>
Production-Ready Code: Clean, documented, reproducible analysis<br>
Business Value Focus: Every analysis ties to actionable business decisions<br>
Complete Workflow: From raw data to strategic recommendations<br>
Recruiter-Friendly: Demonstrates skills sought by top employers<br>


## 🏢 Business Context
Industry: E-Commerce Retail.<br>
Business Type: Online Gift & Home Décor Store.<br>
Geography: Primarily UK (82%), with presence in 38 countries.<br>
Analysis Period: December 2010 - December 2011.<br>
Business Objectives Addressed.<br>

📈 Revenue Optimization - Identify growth opportunities and optimize pricing<br>
👥 Customer Retention - Reduce churn and increase lifetime value<br>
🌍 Market Expansion - Evaluate international growth potential<br>
📦 Product Strategy - Optimize inventory and product portfolio<br>
⏰ Operational Efficiency - Improve resource allocation and scheduling<br>


## ⚡ Features
Core Analytics Capabilities

📊 Exploratory Data Analysis (EDA)

Comprehensive data profiling and quality assessment<br>
Statistical summaries and distribution analysis<br>
Missing value and outlier treatment<br>
![Image Alt](https://github.com/SANJAYBAIRI8686/E-Commerce-Sales-Performance-Customer-Analytics/blob/main/Visuals/1.png?raw=true)
![image alt](https://github.com/SANJAYBAIRI8686/E-Commerce-Sales-Performance-Customer-Analytics/blob/main/Visuals/3.png?raw=true)
![image alt](https://github.com/SANJAYBAIRI8686/E-Commerce-Sales-Performance-Customer-Analytics/blob/main/Visuals/2.png?raw=true)
![image alt](https://github.com/SANJAYBAIRI8686/E-Commerce-Sales-Performance-Customer-Analytics/blob/main/Visuals/4.png?raw=true)



## 💾 SQL Database Integration

SQLite in-memory database implementation<br>
Complex multi-table queries<br>
Aggregation and analytical functions<br>


## 🎯 Customer Segmentation (RFM)

Recency, Frequency, Monetary analysis<br>
5-tier customer classification<br>
Segment-specific marketing strategies<br>
![image alt](https://github.com/SANJAYBAIRI8686/E-Commerce-Sales-Performance-Customer-Analytics/blob/main/Visuals/5.png?raw=true)
![image alt](https://github.com/SANJAYBAIRI8686/E-Commerce-Sales-Performance-Customer-Analytics/blob/main/Visuals/6.png?raw=true)


## 📅 Cohort Analysis

Customer acquisition cohort tracking<br>
Retention rate calculation<br>
Lifecycle value estimation<br>
![image alt](https://github.com/SANJAYBAIRI8686/E-Commerce-Sales-Performance-Customer-Analytics/blob/main/Visuals/7.png?raw=true)


## 📈 Statistical Testing

ANOVA for group comparisons<br>
Correlation analysis<br>
Hypothesis validation<br>
![image alt](https://github.com/SANJAYBAIRI8686/E-Commerce-Sales-Performance-Customer-Analytics/blob/main/Visuals/8.png?raw=true)


## 🛍️ Product Performance Analysis

Top performers identification<br>
ABC analysis for inventory optimization<br>
Cross-sell opportunity identification<br>
![image alt](https://github.com/SANJAYBAIRI8686/E-Commerce-Sales-Performance-Customer-Analytics/blob/main/Visuals/9.png?raw=true)


## 📉 Time Series Analysis

Monthly, weekly, and hourly patterns<br>
Seasonal trend identification<br>
Forecasting indicators<br>



## Visualization Suite

📊 Revenue trend visualizations<br>
🗺️ Geographic distribution analysis<br>
⏰ Temporal pattern heatmaps<br>
👥 Customer segment distributions<br>
📦 Product performance charts<br>
🔥 Cohort retention heatmaps<br>



## 📦 Dataset Information
Source<br>

Name: Online Retail Dataset<br>
Provider: UCI Machine Learning Repository<br>

Dataset Characteristics<br>
AttributeDescriptionTypeInvoiceNoUnique transaction identifierStringStockCodeProduct codeStringDescriptionProduct nameStringQuantityNumber of items purchasedIntegerInvoiceDateTransaction timestampDatetimeUnitPricePrice per unit <br>(£)FloatCustomerIDUnique customer identifierIntegerCountryCustomer's countryString<br>
Dataset Statistics<br>

Total Records: 541,909 transactions<br>
Date Range: Dec 1, 2010 - Dec 9, 2011<br>
Unique Customers: 4,338<br>
Unique Products: 3,665<br>
Countries: 38<br>
After Cleaning: 397,884 transactions (73.4% retention)<br>




## 📂 Project Structure
<pre>

ecommerce-analytics-project/
│
├── data/
│   ├── Online Retail.xlsx          # Original dataset
│   └── customer_segments.csv       # Generated RFM segments
│
├── notebooks/
│   └── ecommerce_analysis.ipynb    # Main analysis notebook
│
├── images/
│   ├── 01_data_exploration.png
│   ├── 02_business_metrics.png
│   ├── 03_revenue_analysis.png
│   ├── 04_rfm_segmentation.png
│   ├── 05_cohort_retention.png
│   ├── 06_correlation_matrix.png
│   ├── 07_product_performance.png
│   └── 08_business_insights.png
│
├── src/
│   ├── data_cleaning.py            # Data preprocessing functions
│   ├── rfm_analysis.py             # RFM segmentation logic
│   ├── cohort_analysis.py          # Retention calculations
│   └── visualizations.py           # Plotting functions
│
├── reports/
│   ├── Executive_Summary.pdf       # High-level business report
│   └── Technical_Documentation.md  # Detailed methodology
│
├── requirements.txt                # Python dependencies
├── README.md                       # This file
├── LICENSE                         # MIT License
└── .gitignore                      # Git ignore rules

</pre>


🔍 Analysis Breakdown
1. Data Cleaning & Preprocessing (20% of effort)<br>
Challenges Addressed:<br>

❌ 24.93% missing CustomerID values → Removed<br>
❌ Negative quantities (returns) → Filtered out<br>
❌ Negative prices (adjustments) → Removed<br>
❌ Data type inconsistencies → Corrected<br>

Feature Engineering:<br>
python# Created new analytical features<br>
- TotalAmount = Quantity × UnitPrice<br>
- Year, Month, Day, Weekday, Hour<br>
- YearMonth (for time series)<br>
Result: Clean dataset of 397,884 high-quality transactions<br>

2. SQL Database Implementation (15% of effort)
Database Schema:<br>
sqlCREATE TABLE sales (<br>
    InvoiceNo TEXT,<br>
    StockCode TEXT,<br>
    Description TEXT,<br>
    Quantity INTEGER,<br>
    InvoiceDate DATETIME,<br>
    UnitPrice REAL,<br>
    CustomerID INTEGER,<br>
    Country TEXT,<br>
    TotalAmount REAL<br>
);<br>
Key Queries:<br>
Top Customers Query:<br>
sqlSELECT <br>
    CustomerID,<br>
    COUNT(DISTINCT InvoiceNo) as TotalOrders,<br>
    ROUND(SUM(TotalAmount), 2) as TotalRevenue<br>
FROM sales<br>
GROUP BY CustomerID<br>
ORDER BY TotalRevenue DESC<br>
LIMIT 10;<br>
Monthly Revenue Trends:<br>
sqlSELECT <br>
    strftime('%Y-%m', InvoiceDate) as YearMonth,<br>
    COUNT(DISTINCT CustomerID) as UniqueCustomers,<br>
    ROUND(SUM(TotalAmount), 2) as MonthlyRevenue<br>
FROM sales<br><br>
GROUP BY YearMonth<br>
ORDER BY YearMonth;<br>

3. Exploratory Data Analysis (20% of effort)
Key Metrics Calculated:

Total Revenue: £8,911,407.90<br>
Average Order Value: £480.87<br>
Customer Count: 4,338<br>
Product Catalog: 3,665 SKUs<br>

Temporal Patterns Identified:

📅 Best Month: November 2011 (holiday season)<br>
📅 Worst Month: February 2011 (post-holiday)<br>
📆 Peak Day: Thursday<br>
⏰ Peak Hours: 10:00 AM - 3:00 PM<br>

Geographic Insights:

🇬🇧 UK Dominance: 82% of revenue<br>
🌍 Top 5 Countries: UK, Germany, France, EIRE, Spain<br>
📊 Market Concentration Risk: High<br>


4. Customer Segmentation - RFM Analysis (20% of effort)
Methodology:
python# Calculate RFM Metrics
rfm = df.groupby('CustomerID').agg({
    'InvoiceDate': lambda x: (snapshot_date - x.max()).days,  # Recency
    'InvoiceNo': 'nunique',                                     # Frequency
    'TotalAmount': 'sum'                                        # Monetary
})

# Assign Scores (1-5 scale)
rfm['R_Score'] = pd.qcut(rfm['Recency'], q=5, labels=[5,4,3,2,1])
rfm['F_Score'] = pd.qcut(rfm['Frequency'].rank(method='first'), q=5, labels=[1,2,3,4,5])
rfm['M_Score'] = pd.qcut(rfm['Monetary'], q=5, labels=[1,2,3,4,5])
Segment Results:
SegmentCount%Avg RevenueCharacteristicsChampions93421.5%£6,697Recent, frequent, high-valueLoyal Customers1,00823.2%£1,397Regular buyersPotential Loyalists1,09225.2%£808Growth opportunityAt Risk75917.5%£342Declining engagementLost54512.6%£193Churned customers

5. Cohort Analysis (15% of effort)
Retention Performance:
Month 0:  100.0% (Baseline)
Month 1:   36.6% (Above industry avg of 20-30%)
Month 3:   38.4% (Excellent retention)
Month 6:   36.3% (Strong loyalty)
Month 12:  26.6% (Outstanding vs. 5-10% benchmark)
Key Finding: Retention rates significantly exceed industry benchmarks, indicating strong product-market fit and customer satisfaction.

6. Statistical Analysis (10% of effort)
Correlation Analysis:

Quantity ↔ Revenue: r = 0.923 (very strong)

Implication: Bundle offers will drive revenue growth


Orders ↔ Revenue: r = 0.554 (moderate)

Implication: Frequency matters but not dominant


Orders ↔ Quantity: r = 0.558 (moderate)

Implication: Mix of small frequent and large occasional buyers



ANOVA Test: Revenue across weekdays

Result: Inconclusive due to outliers
Alternative: Non-parametric tests recommended


🎯 Key Results
Business Impact Summary
Revenue Insights

💰 Total Revenue: £8.9M across 13 months
📈 Growth Trend: Consistent upward trajectory in 2011
🎄 Seasonal Peak: November 2011 (Q4 holiday surge)
💸 High AOV: £480.87 indicates quality positioning

Customer Intelligence

👥 Customer Base: 4,338 unique customers
🏆 Champions: 21.5% generate 70.2% of revenue (80/20 rule)
⚠️ Churn Risk: 30.1% are At-Risk or Lost
📊 Retention: 36.6% Month-1 retention (above industry avg)

Operational Efficiency

⏰ Peak Hours: 10:00-15:00 (optimize staffing)
📅 Best Day: Thursday (concentrate marketing)
🌍 Market Risk: 82% UK dependency (diversification needed)

Product Strategy

📦 Top Product: Paper Craft generated £168K
🎁 Category Focus: Home décor & gifts dominate
📊 SKU Rationalization: 500+ products underperforming


Strategic Recommendations
🚀 Priority 1: Customer Retention (High Impact, Low Cost)
Problem: 63% first-purchase attrition
Solution: Automated lifecycle email campaigns
Investment: £10,000 setup + £500/month
Expected ROI: 850% (£425K annual revenue impact)
Tactics:

Welcome email series (Days 1, 3, 7, 14, 30)
Win-back campaigns for At-Risk segment
Re-engagement for Lost customers
Post-purchase feedback loops


🌍 Priority 2: Geographic Expansion (High Impact, Medium Cost)
Problem: 82% revenue from UK (concentration risk)
Solution: Structured European market entry
Investment: £18K setup + £12.5K/month
Expected ROI: 320% (£1.2M additional revenue)
Target Markets:

Germany (strengthen presence)
France (grow existing base)
Netherlands (high potential)
Italy (new market)
Spain (secondary focus)


📦 Priority 3: Product Portfolio Optimization (Medium Impact, Low Cost)
Problem: 3,665 SKUs create complexity
Solution: Rationalize to top performers
Investment: £5,000
Expected ROI: 300% (£65K inventory freed + reduced costs)
Actions:

Discontinue 500 underperforming SKUs
Focus inventory on A-category (top 20%)
Implement product bundling strategy
Seasonal inventory planning


🎯 Priority 4: Loyalty Program Launch (Medium Impact, Medium Cost)
Solution: 4-tier loyalty program
Investment: £10K setup + £300/month
Expected ROI: £650K annual revenue impact
Tier Structure:

Bronze (all customers)
Silver (5+ purchases)
Gold (10+ purchases)
Platinum (Champions)


🛠️ Technical Skills Demonstrated
Programming & Tools

✅ Python - Advanced data manipulation and analysis
✅ SQL - Complex queries, aggregations, database design
✅ Pandas - DataFrames, groupby, merging, time series
✅ NumPy - Numerical computations and array operations
✅ Matplotlib/Seaborn - Professional data visualizations
✅ SciPy - Statistical testing and analysis
✅ Jupyter - Interactive analysis and documentation

Data Analysis Techniques

✅ Exploratory Data Analysis (EDA)
✅ Data Cleaning & Preprocessing
✅ Feature Engineering
✅ Statistical Hypothesis Testing
✅ Correlation Analysis
✅ Time Series Analysis
✅ Cohort Analysis
✅ Customer Segmentation (RFM)

Business Analytics

✅ KPI Definition & Tracking
✅ Customer Lifetime Value (CLV)
✅ Retention Rate Calculation
✅ ABC Analysis
✅ Pareto Principle Application
✅ Market Basket Analysis
✅ Revenue Forecasting Indicators

Soft Skills

✅ Business Acumen - Translating data into strategy
✅ Communication - Clear visualization and reporting
✅ Problem Solving - Identifying and addressing business issues
✅ Critical Thinking - Data-driven decision making

🚀 Installation
Prerequisites<br>
bashPython 3.8 or higher<br>
Jupyter Notebook or JupyterLab<br>
Step 1: Clone the Repository<br>
bashgit clone https://github.com/yourusername/ecommerce-analytics-project.git<br>
cd ecommerce-analytics-project<br>
Step 2: Create Virtual Environment (Recommended)<br>
bash# Windows<br>
python -m venv venv<br>
venv\Scripts\activate<br>

# macOS/Linux
python3 -m venv venv<br>
source venv/bin/activate<br>
Step 3: Install Required Packages<br>
bashpip install -r requirements.txt<br>
requirements.txt contents:<br>
pandas>=2.0.0<br>
numpy>=1.24.0<br>
matplotlib>=3.7.0<br>
seaborn>=0.12.0<br>
scipy>=1.10.0<br>
openpyxl>=3.1.0<br>
jupyter>=1.0.0<br>
Step 4: Download the Dataset<br>
Option 1: Direct Download<br>
bash# Download from UCI Repository<br>
wget https://archive.ics.uci.edu/static/public/352/online+retail.zip<br>
unzip online+retail.zip<br>
Option 2: Manual Download<br>

Visit: https://archive.ics.uci.edu/dataset/352/online+retail
Download online+retail.zip
Extract Online Retail.xlsx to project directory

Step 5: Verify Installation
bashjupyter notebook
Open 'ecommerce_analysis.ipynb' and run the first cell

💻 Usage
Running the Complete Analysis<br>

Open Jupyter Notebook<br>

bash   jupyter notebook ecommerce_analysis.ipynb<br>

Execute All Cells<br>

Click Cell → Run All
Or use keyboard shortcut: Shift + Enter for each cell


View Results

Outputs display inline
Visualizations render automatically
Results saved to customer_segments.csv



Running Specific Sections
python# Section 1: Data Loading
df = pd.read_excel('Online Retail.xlsx')

# Section 3: Data Cleaning
df_clean = clean_data(df)

# Section 6: RFM Analysis
rfm_results = perform_rfm_analysis(df_clean)

# Section 7: Cohort Analysis
cohort_matrix = create_cohort_analysis(df_clean)
Customizing the Analysis
Adjust Date Range:
python# Filter for specific period
df_filtered = df_clean[
    (df_clean['InvoiceDate'] >= '2011-01-01') &
    (df_clean['InvoiceDate'] <= '2011-06-30')
]
Change RFM Thresholds:
python# Custom segment definitions
def custom_rfm_segment(row):
    if row['RFM_Score'] >= 14:  # Stricter Champion criteria
        return 'Champions'
    # ... additional conditions
Modify Visualizations:
python# Change color scheme
sns.set_palette("viridis")
Adjust figure size
plt.rcParams['figure.figsize'] = (16, 8)



🔮 Future Enhancements
Analytics Enhancements

 Predictive Modeling

Customer churn prediction (Random Forest, XGBoost)
Revenue forecasting (ARIMA, Prophet)
Customer lifetime value prediction


 Advanced Segmentation

K-means clustering
Hierarchical clustering
Behavioral segmentation


 Market Basket Analysis

Apriori algorithm for association rules
Product recommendation engine
Cross-sell optimization



Technical Improvements

 Interactive Dashboard

Plotly/Dash web application
Real-time data updates
Drill-down capabilities


 Automated Reporting

Scheduled report generation
Email distribution
PDF/PowerPoint exports


 Database Optimization

PostgreSQL implementation
Indexing strategy
Query optimization



Data Pipeline

 ETL Pipeline

Automated data ingestion
Data quality checks
Error handling and logging


 Cloud Deployment

AWS/Azure hosting
Scalable architecture
API development




🤝 Contributing
Contributions are welcome! Here's how you can help:
Reporting Issues

🐛 Bug Reports: Open an issue describing the problem
💡 Feature Requests: Suggest improvements or new analyses
📝 Documentation: Help improve README or code comments

Submitting Changes

Fork the Repository

bash   git clone https://github.com/yourusername/ecommerce-analytics-project.git

Create a Branch

bash   git checkout -b feature/your-feature-name

Make Changes

Write clean, documented code
Follow existing code style
Add comments where necessary


Test Your Changes

Ensure all cells run without errors
Verify outputs are correct


Commit and Push

bash   git add .
   git commit -m "Add: your feature description"
   git push origin feature/your-feature-name

Open Pull Request

Describe your changes
Reference related issues
Request review



Code Standards

Use meaningful variable names
Comment complex logic
Follow PEP 8 style guide
Write docstrings for functions


📄 License
This project is licensed under the MIT License - see the LICENSE file for details.
MIT License

Copyright (c) 2024 [Your Name]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.


📊 Live Demo: View Notebook
📂 Repository: GitHub
📄 Full Report: PDF Version


🙏 Acknowledgments

UCI Machine Learning Repository - for providing the dataset
Kaggle Community - for inspiration and best practices
Open Source Community - for amazing Python libraries
Stack Overflow - for technical problem solving


📊 Project Stats
v


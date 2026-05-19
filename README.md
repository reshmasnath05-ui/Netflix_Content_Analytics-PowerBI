# 🎬 Descriptive Analysis on Netflix Content

A Power BI dashboard project that performs descriptive analytics on Netflix content using interactive visualizations and data-driven insights.

---

## 📌 Project Overview

This project analyzes Netflix’s global content library using Power BI.  
The dashboard provides insights into:

- Movies vs TV Shows distribution
- Content growth over years
- Maturity rating analysis
- Country-wise content contribution
- Duration trends
- Genre distribution

The objective is to understand Netflix’s content strategy, global expansion, and audience targeting patterns.

---

## 📊 Dashboard Preview

![Netflix Dashboard](Dashboard/netflix_dashboard.png)

---

## 🛠 Tools & Technologies Used

- Power BI
- Microsoft Excel / CSV
- Data Cleaning
- DAX Measures
- Data Visualization

---

## 📂 Dataset Information

- Source: Kaggle Netflix Dataset
- Total Records: 7970
- Total Columns: 10

### Important Columns

- Type
- Title
- Country
- Release Year
- Rating
- Duration
- Listed In (Genres)

Dataset Source:  
https://www.kaggle.com/datasets/shivamb/netflix-shows

---

## 🧹 Data Cleaning Steps

- Removed duplicate records
- Handled missing values
- Converted duration text into numeric values
- Standardized data types
- Corrected inconsistent formatting

---

## 📈 Key Insights

### Content Distribution
- Movies dominate Netflix content library
- TV Shows form a smaller but growing portion

### Top Contributing Countries
- United States
- India
- United Kingdom
- Canada
- France

### Maturity Ratings
Most content belongs to:
- TV-MA
- TV-14
- TV-PG

### Duration Insights
- Most movies range between 80–120 minutes
- Short-form content increased after 2018

---

## 📊 Power BI Visualizations Used

- Donut Chart
- Area Chart
- Funnel Chart
- Treemap
- Map Visualization
- Stacked Column Chart

---

## 📌 DAX Measures Used

```DAX
Total Titles = COUNTROWS(netflix_titles)

Total Movies =
CALCULATE(
    COUNTROWS(netflix_titles),
    netflix_titles[type] = "Movie"
)

Total TV Shows =
CALCULATE(
    COUNTROWS(netflix_titles),
    netflix_titles[type] = "TV Show"
)
```

---

## 📌 Conclusion

Netflix’s catalog is heavily dominated by movies and adult-focused content.  
The rapid growth after 2015 reflects Netflix’s aggressive global expansion and investment in original productions.

This analysis demonstrates how data visualization can help identify entertainment industry trends and audience-focused strategies.



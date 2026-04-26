# 🏏 IPL 2024 Analysis Dashboard

[![Live Demo](https://img.shields.io/badge/Live-Dashboard-brightgreen)](https://YOUR_USERNAME.github.io/ipl-powerbi-dashboard/)
[![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=power-bi&logoColor=black)](https://powerbi.microsoft.com/)
[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-222222?style=flat&logo=githubpages&logoColor=white)](https://pages.github.com/)

## 🎯 Live Interactive Dashboard

> **🔗 Click here to view the live dashboard:** 

![Dashboard Preview](./assets/IPL_Dashboard_Preview.png)

---

## 📊 Project Overview

This interactive **Power BI dashboard** provides a comprehensive analysis of the **Indian Premier League (IPL) (2008-2024) season**. It answers key business questions about team performance, player statistics, and match strategies through an intuitive, filterable interface.

### Key Features

| Feature | Description | 2024
|---------|-------------|
| 🏆 **Tournament Summary** | Winner, total runs (25,971), total wickets (883) |
| 👤 **Player Performance** | Select any batsman/bowler to view detailed stats |
| 📈 **Top Performers** | Orange Cap (V Kohli - 741 runs) & Purple Cap (JJ Bumrah - 30 wickets) |
| 🎲 **Toss Analysis** | Winning percentage by toss decision (bat vs field) |
| 🏅 **Team Rankings** | Top winning teams by runs and wickets |

Key Insights from Analysis( Year - 2024)
Insight	Finding
Toss Impact	Teams choosing to bat first won only 23% of matches
Top Scorer	V Kohli dominated with 741 runs at 149.09 strike rate
Best Bowler	JJ Bumrah took 30 wickets with 6.24 economy
Champions	Kolkata Knight Riders won 11 matches (6 by runs, 5 by wickets)

---

## 🛠️ Technical Implementation

### Tools Used
- **Power BI Desktop** - Dashboard creation & visualization
- **DAX** - Advanced measures and calculated columns
- **Power Query** - Data transformation & cleaning
- **GitHub Pages** - Hosting the live dashboard

### Data Processing Steps
1. **Extract** - Gathered IPL 2024 match and player statistics
2. **Transform** - Cleaned data using Power Query (handled missing values, created calculated columns)
3. **Load** - Built relational data model with fact and dimension tables
4. **Visualize** - Created interactive report with slicers, bookmarks, and drill-through pages
5. **Publish** - Deployed to Power BI Service and embedded via GitHub Pages

### Key DAX Measures Used
```dax
// Strike Rate Calculation
Strike Rate = DIVIDE([Total Runs], [Total Balls Faced], 0) * 100

// Economy Rate for Bowlers
Economy Rate = DIVIDE([Total Runs Conceded], [Total Overs Bowled], 0)

// Win % by Toss Decision
Win % = DIVIDE([Matches Won], [Matches Played], 0) * 100

# 🏏 IPL 2024 Analysis Dashboard

[![Live Demo](https://img.shields.io/badge/Live-Dashboard-brightgreen)](https://YOUR_USERNAME.github.io/ipl-powerbi-dashboard/)
[![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=power-bi&logoColor=black)](https://powerbi.microsoft.com/)
[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-222222?style=flat&logo=githubpages&logoColor=white)](https://pages.github.com/)

## 🎯 Live Interactive Dashboard

> **🔗 Click here to view the live dashboard:** https://app.powerbi.com/view?r=eyJrIjoiOWVhMGJkNGMtYmRiZi00MmNlLTgxZjEtYTViN2MzZGEwMGY1IiwidCI6IjdiYTdhM2JkLTc2MzYtNGY1ZC04MTFmLTYxNzExNWViMDBhMiJ9

![Dashboard Preview](./assets/IPL_Dashboard_Preview.png)
<img width="907" height="508" alt="IPL Dasboard Preview" src="https://github.com/user-attachments/assets/0eb5aa53-33ff-4d0d-af48-b03b4e760b06" />

---

## 📊 Project Overview

This interactive **Power BI dashboard** provides a comprehensive analysis of the **Indian Premier League (IPL) 2024 season**. It answers key business questions about team performance, player statistics, and match strategies through an intuitive, filterable interface.

### Key Features

| Feature | Description |
|---------|-------------|
| 🏆 **Tournament Summary** | Winner, total runs (25,971), total wickets (883) |
| 👤 **Player Performance** | Select any batsman/bowler to view detailed stats |
| 📈 **Top Performers** | Orange Cap (V Kohli - 741 runs) & Purple Cap (JJ Bumrah - 30 wickets) |
| 🎲 **Toss Analysis** | Winning percentage by toss decision (bat vs field) |
| 🏅 **Team Rankings** | Top winning teams by runs and wickets |

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

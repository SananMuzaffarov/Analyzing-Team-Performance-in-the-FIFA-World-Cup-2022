# FIFA World Cup 2022 Analytics & 2026 Projections

A comprehensive data analysis project exploring team performance metrics, playing styles, and future potential from the FIFA World Cup 2022, with projections for the 2026 World Cup.

## 📊 Project Overview

This project analyzes team performance data from the 2022 FIFA World Cup to identify key success factors, team playing styles, and predict promising teams for the 2026 World Cup. The analysis covers multiple dimensions including squad age, offensive/defensive balance, set-piece effectiveness, and goalkeeper performance.

## 📁 Project Structure
├── data/
│ ├── team_data.csv # Complete team performance statistics
│ └── team_data.sql # SQL queries for data analysis
├── visualizations/
│ ├── 2026potential-2.png # 2026 World Cup team potential analysis
│ ├── aerial.png # Set-piece and aerial effectiveness
│ ├── age1.png # Squad age vs scoring performance
│ ├── age2.png # Team age distribution analysis
│ ├── averageStats.png # Distribution of key metrics
│ ├── correlationMatrix1.png # Team playing styles clustering
│ ├── correlationMatrix2.png # Offensive vs defensive balance
│ ├── goalkeeper2.png # Goalkeeper performance analysis
│ └── topAvgStats.png # Top performers in key categories
└── README.md

## 🔍 Key Insights

### 🎯 2026 World Cup Potential
- **Most Promising Teams**: France, Spain, Ecuador, USA, Argentina
- **Young Squads with High Potential**: Ecuador (Age: 25.8), USA (Age: 25.4), Spain (Age: 26.4)
- **Youth Impact**: Young teams showed +70.3% improvement in goals per game

### ⚽ Performance Metrics
**Top Scoring Teams:**
- France (16 goals)
- Argentina (15 goals) 
- England (13 goals)
- Portugal (12 goals)

**Top Possession Teams:**
- Spain (75.8%)
- England (62.8%)
- Portugal (60.4%)
- Denmark (60.0%)

### 🧭 Playing Styles Analysis
Teams clustered into distinct playing styles:
- **Offensive Powerhouses**: Brazil, Germany, Spain
- **Balanced Approach**: England, Portugal, France
- **Defensive Specialists**: Morocco, Netherlands

### 🎪 Set-Piece Effectiveness
**Top Aerial Teams:**
- Canada (58.9% aerial win percentage)
- France (57.6%)
- Costa Rica (55.9%)

**Correlation Analysis:**
- Strong correlation between corners and goals (r = 0.727)
- Strong correlation between aerial duels and goals (r = 0.667)

### 🧑‍🤝‍🧑 Squad Age Analysis
- **Youngest Teams**: USA (25.4), Ecuador (25.8), Ghana (26.4), Spain (26.4)
- **Oldest Teams**: Belgium (30.6), Costa Rica (30.6), Iran (29.3), Croatia (29.2)
- **Tournament Average Age**: 28.1 years

## 📈 Methodology

### Data Sources
- Comprehensive team statistics from FIFA World Cup 2022
- Performance metrics across 50+ variables including possession, passing, tackling, and scoring

### Analytical Approach
1. **Descriptive Analytics**: Distribution analysis of key performance indicators
2. **Correlation Analysis**: Identifying relationships between different metrics
3. **Cluster Analysis**: Grouping teams by playing styles
4. **Predictive Modeling**: Projecting team potential for 2026 based on youth and current performance

### Key Metrics Tracked
- Offensive: Goals, shots, possession, passes completed
- Defensive: Tackles, interceptions, clearances
- Special: Set-pieces, aerial duels, goalkeeper performance
- Developmental: Squad age, player utilization, progression metrics

## 🛠️ Technical Implementation

### Data Processing
- SQL queries for data extraction and aggregation
- CSV dataset with complete team performance statistics
- Statistical analysis using correlation matrices and distribution plots

### Visualization
- Multiple chart types: bar charts, scatter plots, distribution graphs
- Comparative analysis across different performance dimensions
- Team clustering based on playing style characteristics

## 🚀 Getting Started

### Prerequisites
- SQL database for querying team_data
- Data visualization tools for PNG files
- Statistical analysis software (optional)

### Basic Analysis
```sql
-- Example: Query top scoring teams
SELECT team, goals, goals_per90, avg_age
FROM team_data 
ORDER BY goals DESC 
LIMIT 10;

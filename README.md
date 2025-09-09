# Uncovering Patterns in NCAA Basketball Team Statistics  
### An Exploratory Data Analysis (2013–2021)

![NCAA Basketball](https://upload.wikimedia.org/wikipedia/commons/thumb/3/3d/NCAA_logo.svg/320px-NCAA_logo.svg.png)

## 📌 Project Overview
This project explores performance metrics of NCAA basketball teams between **2013 and 2021** (excluding 2020 due to COVID-19’s impact on postseason play). Using the dataset from Kaggle, the analysis investigates what distinguishes **successful teams from underperformers**, highlights **statistical anomalies**, and examines **trends across seasons**.  

The focus is on correlations between team statistics (e.g., offensive/defensive efficiency, shooting percentages) and outcomes (wins and postseason results).  

## 📂 Dataset
- Source: [College Basketball Dataset – Kaggle](https://www.kaggle.com/datasets/andrewsundberg/college-basketball-dataset)  
- File: `cbb.csv`  
- Seasons covered: 2013–2021 (2020 excluded)  
- Key variables:  
  - `W` – Wins  
  - `ADJOE` – Adjusted Offensive Efficiency  
  - `ADJDE` – Adjusted Defensive Efficiency  
  - `X2P_O` – Two-point shooting percentage  
  - `X3P_O` – Three-point shooting percentage  
  - `POSTSEASON` – Tournament outcome  
  - `SEED` – NCAA tournament seed  

## 🛠️ Tools & Libraries
The analysis was conducted in **RStudio** using the following packages:  
- `tidyverse` – data wrangling & visualization  
- `gganimate`, `gifski`, `magick` – animated visualizations  
- `ggrepel` – improved text labels  
- `knitr` – reporting  
- `ggcorrplot` – correlation matrices  

## 📊 Key Insights
- **Offense drives success** → Wins strongly correlate with `ADJOE` (r ≈ 0.73).  
- **Interior efficiency matters** → Teams above **50% 2PT shooting** consistently outperform, with the share of such teams rising over time.  
- **Three-point shooting is less predictive** → Correlation with wins is weaker (r ≈ 0.42), and the share of elite 3PT teams (>38%) has declined since the 2019 line extension.  
- **Consistent winners** → Programs like Gonzaga, Duke, and UNC not only sustain regular-season dominance but also achieve deep postseason runs.  
- **Parity is improving** → The number of teams with very low win percentages (<0.39) has decreased, suggesting greater balance across Division I.  

## 📈 Visualizations
The project includes:  
- Correlation heatmaps of team statistics  
- Animated scatterplots (Wins vs. ADJOE, Wins vs. Shooting %)  
- Trend analysis of shooting efficiency over seasons  
- Distribution of winning and losing teams  
- Consistency analysis of top-performing and struggling programs  

## 🚀 Getting Started
Clone the repo and open the R project in RStudio:  

```{bash}
git clone https://github.com/yourusername/ncaa-basketball-eda.git
cd ncaa-basketball-eda
```

## Install required R packages:
```{R}
install.packages(c("tidyverse", "gganimate", "gifski", "magick", "knitr", "ggrepel", "ggcorrplot"))
```

## 🏀 Conclusion

The analysis highlights how offensive efficiency and two-point scoring are central to modern NCAA success, while elite three-point shooting plays a less consistent role than in the professional game. Over time, college basketball has seen greater parity, with fewer persistently struggling programs and more competitive balance across conferences.

🔗 Author: Jakub Zoldak
📧 Contact: [GitHub Profile Link](github.com/yak0b0)

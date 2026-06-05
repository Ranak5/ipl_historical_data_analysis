# IPL Data Analysis (2008 - 2024) 🏏

A comprehensive, end-to-end data analysis project exploring 16+ seasons of Indian Premier League (IPL) historical data. This project processes and analyzes millions of data points across two distinct granularities—match-level data and ball-by-ball delivery records—to uncover long-term trends, team performance metrics, and deep player impact statistics.

## 🚀 Project Overview
Most baseline sports analyses rely on surface-level statistics. This project dives deeper into the numbers to validate real-world cricket narratives—such as analyzing the true value of death-over bowlers versus mid-over economic anchors—by handling massive, multi-year datasets.

### Key Highlights:
*   **Scale:** Analyzed structural data spanning from the inaugural 2008 season up to the 2024 tournament.
*   **Granularity Cross-Referencing:** Successfully merged and aggregated high-level match results with granular, ball-by-ball delivery datasets.
*   **Data Integrity:** Handled historical real-world data anomalies, including shifting franchise identities (e.g., mapping Delhi Daredevils to Delhi Capitals) and inconsistent naming conventions over a 16-year timeline.

---

## 🛠️ Tech Stack & Tools
*   **Language:** Python
*   **Data Manipulation:** Pandas, NumPy
*   **Data Visualization:** Seaborn, Matplotlib
*   **Environment:** Jupyter Notebook / Git

---

## 📊 Core Analysis & Features

### 1. Data Merging & Relational Schema
*   Imported and cleaned `matches.csv` and `deliveries.csv`.
*   Aligned data granularities using advanced Pandas operations (`merge`, `groupby`, and custom transformations) to map ball-by-ball events directly to specific match outcomes and seasons.

### 2. Historical Consistency & Data Cleaning
*   Standardized team names across the entire 2008–2024 timeline to ensure accurate historical aggregations.
*   Handled structural anomalies, missing values, and edge cases like "No Result" matches due to external disruptions (e.g., rain-shortened games).

### 3. Advanced Player Impact & Domain Insights
*   **The Bowler's Paradox:** Evaluated premium death-over specialists (overs 16–20) against mid-over anchors. Proved through data aggregation that raw economy rates hide a bowler's true value, as death-over specialists face highly aggressive batting conditions that naturally inflate their metrics compared to mid-over bowlers.
*   **Trend Tracking:** Plotted distribution metrics, top run-scorers, highest wicket-takers, and team win-percentages over time.

---

## 📈 Key Visualizations & Insights

> 💡 *Note: Below are the primary takeaways derived from the Jupyter Notebook analysis.*

*   **Context Over Averages:** Contextual performance (when a run is saved or a wicket is taken) is a much stronger indicator of player impact than seasonal averages.
*   **Evolution of Scopes:** Visualized how average team totals and strike rates have aggressively scaled upward in recent seasons of the IPL.

---

## 📁 Repository Structure

```text
├── ipl_data_analysis.ipynb   # Main Jupyter Notebook with core Python code
├── data/
│   ├── matches.csv           # Match-level historical data (2008-2024)
│   └── deliveries.csv        # Ball-by-ball delivery records
└── README.md                 # Project documentation
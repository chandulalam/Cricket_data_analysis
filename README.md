# Cricket_data_analysis
# T20 World Cup 2022 - Cricket Analytics Dashboard

## Overview
This project is a **Power BI Dashboard** analyzing the T20 World Cup 2022.  
It visualizes player and match statistics, with **dynamic tooltips** showing player profiles, performance summaries, and KPIs.

The pipeline starts with **web scraping data from ESPN**, converting JSON to CSV using Python (Pandas), cleaning the data, and finally building the dashboard in Power BI.

---

## Project Workflow

### 1. Web Scraping Player & Match Data
- Data scraped from **ESPN Cricinfo** using Python.
- Scraping scripts fetch:
  - Player details (profiles, photos, descriptions)
  - Batting & bowling stats
  - Match summaries
- Data is stored as **JSON files**.

### 2. Converting JSON to CSV (Python & Pandas)
- JSON files are loaded using **Pandas**.
- Cleaned and exported to CSV files:
  - `players.csv`
  - `batting_summary.csv`
  - `bowling_summary.csv`
  - `match_summary.csv`

### 3. Data Cleaning
- Using **Pandas**:
  - Removed duplicates.
  - Filled missing values (where applicable).
  - Normalized column names.
  - Converted numeric fields (runs, averages, strike rates) to proper data types.

### 4. Power BI Data Transformation (Power Query)
- Loaded all CSVs into Power BI.
- Created additional calculated columns (Player Role, Total Points, Economy Grouping, etc.).
- Changed data types for numeric fields.
- Built relationships between tables for dynamic filtering.

### 5. Visualization & Dashboard
- Designed interactive report:
  - **Player profile cards** with images and stats (tooltip pages).
  - **Team-level comparisons** (batting & bowling performance).
  - **Match summary insights** (wins, run rates, strike rates).
  - Filters by team, player, and role.
- Final dashboard file: `t20_wc_2022.pbix`.

---

## Files in This Repository
- `t20_wc_2022.pbix` – Final Power BI dashboard.
- `players.csv` – Player profiles and details.
- `batting_summary.csv` – Batting performance stats.
- `bowling_summary.csv` – Bowling performance stats.
- `match_summary.csv` – Match-level summaries.
- `README.md` – Documentation file (this file).

---

## How to Run
1. Clone or download this repository.
2. Open `t20_wc_2022.pbix` in **Power BI Desktop**.
3. Ensure all CSVs (`players.csv`, `batting_summary.csv`, `bowling_summary.csv`, `match_summary.csv`) are in the same folder as the PBIX file.
4. Refresh the dashboard to load the latest data.

---

## Requirements
- Python 3.x (for data scraping & cleaning)
  - Libraries: `requests`, `pandas`, `json`
- Power BI Desktop (latest version)
- Internet (to load player images dynamically)

---

## Dashboard Preview
*(Insert screenshot here)*  
![Dashboard Preview](your-screenshot-link-here)

---

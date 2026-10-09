# OTT Viewer Drop-Off & Retention Analysis

An exploratory data analysis (EDA) project investigating viewer engagement, retention patterns, and drop-off behaviour in a streaming-platform business scenario.

## Project Overview

This project analyses episode-level OTT viewing data to understand watch percentage, engagement patterns, drop-off behaviour, and differences across genres, platforms, and content titles.

Hotstar is used as the business scenario for this analysis. The dataset is synthetically generated and does not represent actual Hotstar proprietary viewer data.

## Objectives

- Explore viewer watch percentage and engagement distributions.
- Compare retention and drop-off patterns across genres and platforms.
- Investigate relationships between pacing, hook strength, cognitive load, and watch percentage.
- Analyse episode-number ranges and title-level performance.
- Identify data-quality issues and communicate business insights.

## Tech Stack

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Jupyter Notebook

## Repository Structure

- `Eda.ipynb` — EDA code, calculations, and visualisations.
- `EDA_Insights.ipynb` — Key findings, interpretations, and business insights.
- `ott_viewer_dropoff_retention_us_v1.0.xlsx` — Dataset file, if permitted to redistribute.
- `README.md` — Project documentation.

## Key Findings

- Average watch percentage: 56.81%.
- Comedy has a median watch percentage of 64%, compared with 52% for Drama.
- Pacing score and hook strength have moderate positive correlations with watch percentage.
- Cognitive load has a strong negative correlation with watch percentage.
- The observed drop-off rate is 14.48%.
- The drop-off label matches a threshold of 0.60 on the drop-off probability column in this dataset.

## Data Disclaimer

The OTT Viewer Drop-Off & Retention Risk Dataset contains approximately 33,200 episode-level records. Viewer behaviour variables are synthetically generated to support realistic OTT analytics.

**This is not actual Hotstar proprietary data.** All findings describe patterns within the synthetic dataset and must not be interpreted as actual Hotstar viewer behaviour.

## Limitations

- The analysis is observational and does not establish causation.
- Episode numbers are repeated across different shows, and all records have `season_number = 1`.
- An extreme episode-duration value of 1,225 minutes was identified.
- The drop-off label has a deterministic relationship with drop-off probability, which limits how independently these variables can be interpreted.

## How to Run

1. Clone or download the repository.
2. Install the required packages:

   `pip install pandas numpy matplotlib seaborn openpyxl jupyter`

3. Launch Jupyter Notebook:

   `jupyter notebook`

4. Open `Eda.ipynb` and execute the cells in order.

## Future Scope

- Verify dataset-generation rules and investigate potential data leakage.
- Explore additional engagement patterns using reliable time-stamped viewing data.
- Extend the project with predictive modelling after reviewing machine learning concepts.
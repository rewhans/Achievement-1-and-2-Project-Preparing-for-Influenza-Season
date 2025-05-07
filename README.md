# Achievement-1-and-2-Project-Preparing-for-Influenza-Season

## 🦠 Preparing for Influenza Season

*A Data-Driven Staffing Strategy for U.S. Healthcare Agencies*

### 🔍 Project Overview

Seasonal influenza presents recurring challenges for U.S. healthcare systems. This project leverages national health and population data to help a medical staffing agency proactively allocate limited personnel—nurses, physician assistants, and doctors—across all 50 states. The goal: ensure vulnerable populations receive care without overstaffing or underutilizing resources.

This analysis was completed as part of CareerFoundry's Data Analytics Immersion program (Achievements 1 & 2).

### 🎯 Objectives

* Identify *when* and *where* influenza peaks occur across the U.S.
* Prioritize states based on vulnerable population concentrations.
* Design a staffing plan that minimizes both overstaffing and understaffing.
* Provide actionable insights using spatial and temporal visualizations.

### 🧩 Key Questions

1. Does influenza follow a seasonal pattern nationwide?
2. Which states have the highest counts of vulnerable populations?
3. What correlations exist between flu incidence, deaths, vaccination rates, and population demographics?
4. How can the agency optimize staff distribution using these insights?

### 📊 Data Sources

| Dataset                          | Description                               | Source      |
| -------------------------------- | ----------------------------------------- | ----------- |
| Influenza Deaths by Geography    | Mortality data related to flu             | CDC         |
| Population by State, Age, Gender | Demographic data for risk categorization  | U.S. Census |
| Flu Shot Rates in Children       | Immunization rates among vulnerable youth | CDC         |
| Influenza Test Results           | Lab-confirmed flu cases by state          | CDC FluView |

> Note: Data preprocessing involved cleaning missing values, standardizing state names, merging on consistent state codes, and addressing format inconsistencies across time series data.

### 🧪 Methodology

* **Data Cleaning & Transformation**: Merged CDC and Census data into a unified dataset, normalized population metrics per state, and identified outliers.
* **Exploratory Analysis**:

  * Assessed flu seasonality via temporal line charts.
  * Compared vulnerable population counts with historical flu deaths.
* **Statistical Testing**:

  * Correlation analysis between flu deaths and elderly populations.
  * Hypothesis testing to determine if flu deaths differ significantly in high-vulnerability vs. low-vulnerability states.
* **Visualization**: Created dynamic dashboards in Tableau, including:

  * Temporal flu death trends by state
  * Vulnerable population heatmaps
  * Forecasts for peak flu months
  * Staffing ratio models

### 📌 Key Insights

* Influenza exhibits **strong seasonal behavior**, typically peaking between **December and February**, though start/end months vary by state.
* States with **higher vulnerable populations** (e.g., Florida, West Virginia, Mississippi) correlate with **higher flu death rates**.
* Vaccine uptake in children varies widely, influencing vulnerability levels.
* Recommended a **state-tiering system**: High, Medium, Low need—based on vulnerable population density and historical flu outcomes.

### 🧠 Recommendations

* Prioritize staff deployment to **high-need states during flu peak months**.
* Use historical flu patterns and population makeup to anticipate demand spikes.
* Improve data collection on adult vaccination rates and staff availability to further refine the model.
* Establish a **forecasting tool** for annual flu seasons to automate planning in future years.

### 📈 Tools & Technologies

* **Data Cleaning & Analysis**: Python (Pandas, NumPy), Excel
* **Statistical Testing**: SciPy
* **Visualization**: Tableau
* **Version Control**: Git/GitHub

### 🗺️ Project Structure

```
📁 Achievement-1-and-2-Project-Preparing-for-Influenza-Season/
├── Reports/
│   ├── Ryan_Wick_Data Immersion_Flu Season_Ach-01.10_Task_Interim Report.pdf
│   ├── Ryan_Wick_Data Immersion_Flu Season_Ach-02.10_Task_Final.pdf
│   ├── Ryan_Wick_Data Immersion_Flu Season_Ach-02.11_Project Reflection.docx
├── Project-brief/
│   ├── Ryan_Wick_Data Immersion_Flu Season_Ach-01.00_02.00_Project Brief.pdf
├── Data/
│   ├── raw/
│   │   ├── Ryan_Wick_Data Immersion_Flu Season_Ach-01.05_Task-Census_Raw.xlsx
│   │   ├── Ryan_Wick_Data Immersion_Flu Season_Ach-01.05_Task-Death_Raw.xlsx
│   │   ├── Ryan_Wick_Data Immersion_Flu Season_Ach-02.00_CDC_Fluview_Counts of flu lab test results by state (survey) -Lab Tests Data Set.xlsx
│   │   ├── Ryan_Wick_Data Immersion_Flu Season_Ach-02.00_CDC_Fluview_Counts of flu lab test results by state (survey)-Influenza Visits Data Set.xlsx
│   ├── cleaned/
│   │   ├── Ryan_Wick_Data Immersion_Flu Season_Ach-01.05_Task-Census_Cleaned.xlsx
│   │   ├── Ryan_Wick_Data Immersion_Flu Season_Ach-01.05_Task-Death_Cleaned.xlsx
│   │   ├── Ryan_Wick_Data Immersion_Flu Season_Ach-01.06_Task-Census_Updated_Profile.xlsx
│   │   ├── Ryan_Wick_Data Immersion_Flu Season_Ach-01.06_Task-Death_Updated_Profile.xlsx
│   │   ├── Ryan_Wick_Data Immersion_Flu Season_Ach-02.00_Integrated Data.xlsx
├── README.md
```

### 📂 Next Steps

* Integrate real-time flu tracking APIs for live updates.
* Incorporate healthcare provider availability per region to match supply/demand more accurately.
* Collaborate with state health departments to pilot deployment strategies.

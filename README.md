# Formula 1 Race Data Analysis (1950–2017)

## Project Summary

This project performs comprehensive data cleaning, preparation, and exploratory data analysis (EDA) on the Formula 1 Race Dataset covering seasons from 1950 to 2017.

The analysis combines multiple Formula 1 datasets, including races, drivers, constructors, circuits, lap times, pit stops, qualifying sessions, standings, and race results. The project focuses on improving data quality, handling missing values, standardizing formats, and extracting meaningful insights about championships, race performance, driver achievements, and race operations.

The objective is to transform raw Formula 1 historical data into a structured and analysis-ready dataset while uncovering trends and patterns from more than six decades of racing history.

---

# Features

* Automated dataset download from Kaggle
* Multi-table Formula 1 dataset integration
* Data cleaning and preprocessing across all datasets
* Missing value detection and treatment
* Duplicate record identification and removal
* Data type validation and correction
* Time format standardization
* String normalization and whitespace cleanup
* Championship analysis
* Driver performance analysis
* Constructor performance analysis
* Podium finish analysis
* Pit stop analysis
* Race distribution analysis by season
* Lap time analysis across circuits
* Statistical summaries and visualizations

---

# Tech Stack

## Programming Language

* Python

## Libraries

* Pandas
* NumPy
* Matplotlib
* Seaborn
* KaggleHub
* OS (file handling)

## Development Environment

* Google Colab
* Jupyter Notebook

## Data Analysis Techniques

* Data Cleaning
* Data Preprocessing
* Exploratory Data Analysis (EDA)
* Aggregation and Grouping
* Statistical Analysis
* Data Visualization

---

# Dataset Information

## Source

Formula 1 Race Dataset (1950–2017)

Downloaded directly from Kaggle using:

```python
path = kagglehub.dataset_download("cjgdev/formula-1-race-data-19502017")
```

## Included Datasets

| Dataset                  | Description                        |
| ------------------------ | ---------------------------------- |
| circuits.csv             | Circuit information                |
| races.csv                | Race details                       |
| drivers.csv              | Driver information                 |
| constructors.csv         | Constructor information            |
| results.csv              | Race results                       |
| qualifying.csv           | Qualifying session results         |
| lapTimes.csv             | Driver lap times                   |
| pitStops.csv             | Pit stop records                   |
| driverStandings.csv      | Driver championship standings      |
| constructorStandings.csv | Constructor championship standings |
| constructorResults.csv   | Constructor race results           |
| seasons.csv              | Season information                 |
| status.csv               | Race status descriptions           |

## Data Characteristics

* Historical Formula 1 data from 1950–2017
* Multiple relational datasets
* Driver, constructor, race, and circuit information
* Championship standings and race outcomes
* Lap timing and pit stop records
* Qualifying and season-level statistics

---

# Methodology / Workflow

## 1. Data Collection

* Download Formula 1 dataset from Kaggle.
* Load all CSV files into Pandas DataFrames.

## 2. Data Inspection

* Review dataset structure and dimensions.
* Examine column information and data types.
* Generate statistical summaries.

## 3. Data Cleaning

Performed cleaning across all datasets:

### Circuits

* Removed highly sparse columns.
* Checked null values and duplicates.
* Standardized text fields.

### Constructor Results

* Removed columns with excessive missing values.
* Verified data consistency.

### Constructor Standings

* Checked missing values and duplicates.
* Validated standings data.

### Constructors

* Cleaned categorical fields.
* Standardized text values.

### Drivers

* Inspected and cleaned driver information.
* Validated date and string fields.

### Lap Times

* Standardized time formats.
* Verified lap timing consistency.

### Pit Stops

* Normalized time values.
* Cleaned race operation records.

### Qualifying

* Handled missing timing information.
* Standardized qualifying formats.

### Results

* Treated missing position values.
* Filled missing race positions using position order where applicable.

### Seasons & Status

* Cleaned metadata tables.
* Validated reference information.

## 4. Exploratory Data Analysis

The project answers several analytical questions:

### Race Distribution

* Distribution of races across seasons.

### Constructor Championships

* Constructors with the highest number of championship wins.

### Driver Performance

* Distribution of driver race positions.

### Pit Stop Analysis

* Average number of pit stops per race.

### Podium Analysis

* Drivers with the highest number of podium finishes.

### Lap Time Analysis

* Variation in lap times across circuits.

## 5. Visualization

* Histograms
* Bar Charts
* Count Plots
* Distribution Plots
* Comparative Performance Charts

---

# Key Insights

* Formula 1 race activity varies significantly across seasons.
* Certain constructors dominate championship standings over long periods.
* Podium finishes are concentrated among a relatively small group of elite drivers.
* Pit stop behavior differs between races and seasons.
* Circuit characteristics influence lap-time performance.
* Data cleaning is essential due to inconsistencies and missing values across multiple historical datasets.

---

# Recommendations

* Build predictive models for race outcomes and championship standings.
* Analyze constructor dominance across different eras.
* Explore driver performance trends throughout careers.
* Investigate pit stop strategies and their impact on race results.
* Develop interactive dashboards for Formula 1 analytics.
* Integrate newer Formula 1 seasons to extend historical comparisons.

---

# Installation

## Clone the Repository

```bash
git clone https://github.com/Divyam-Deep/F1-Race-EDA.git
cd F1-Race-EDA
```

## Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn kagglehub
```

---

# Usage

## Run the Notebook

```bash
jupyter notebook F1_race_EDA_Practice.ipynb
```

Or open the notebook directly in Google Colab.

## Execute the Workflow

1. Download the dataset automatically from Kaggle.
2. Load all Formula 1 tables.
3. Run data cleaning cells.
4. Execute exploratory analysis.
5. Generate visualizations and insights.

---

# Project Structure

```text
F1-Race-EDA/
│
├── F1_race_EDA_Practice.ipynb
├── README.md
├── requirements.txt
│
├── data/
│   ├── circuits.csv
│   ├── races.csv
│   ├── drivers.csv
│   ├── constructors.csv
│   ├── results.csv
│   ├── qualifying.csv
│   ├── lapTimes.csv
│   ├── pitStops.csv
│   ├── driverStandings.csv
│   ├── constructorStandings.csv
│   ├── constructorResults.csv
│   ├── seasons.csv
│   └── status.csv
│
└── visualizations/
    ├── championship_analysis.png
    ├── podium_finishes.png
    ├── race_distribution.png
    ├── pitstop_analysis.png
    └── lap_time_analysis.png
```

---

# Future Improvements

* Driver performance prediction models
* Championship forecasting
* Race strategy analysis
* Circuit difficulty comparison
* Interactive dashboards using Streamlit or Plotly
* Advanced statistical modeling
* Integration of modern Formula 1 seasons and telemetry data
* Automated reporting and analytics pipelines

---

# Author

**Divyam Deep**

Data Analyst | Python Developer | Exploratory Data Analysis Enthusiast

This project demonstrates large-scale data cleaning, preprocessing, and exploratory analysis techniques using historical Formula 1 racing data to uncover insights into drivers, constructors, races, championships, and race performance trends.

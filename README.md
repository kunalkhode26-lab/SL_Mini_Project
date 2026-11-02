# Air Quality Analysis of 26 Indian Cities

A data analysis project that explores historical Air Quality Index (AQI) readings across 26 Indian cities using Python and an interactive HTML dashboard.

## 📌 Project Overview

Air pollution is a major environmental concern in India. This project analyzes historical air quality data to understand pollution levels across different cities, seasonal variations, pollutant relationships, and changes during the 2020 lockdown period.

The analysis covers daily AQI readings from **1 January 2015 to 1 July 2020**.

The project uses Python for data cleaning, exploratory data analysis, statistical analysis, and visualization. An interactive HTML dashboard presents the findings in an easy-to-understand format.

## 🎯 Objectives

- Analyze air quality across 26 Indian cities.
- Clean and preprocess the AQI dataset.
- Compare average AQI levels between cities.
- Identify yearly, monthly, and seasonal pollution patterns.
- Analyze the relationship between AQI and different pollutants.
- Compare air quality during the same period in 2019 and 2020.
- Identify the overall national AQI trend.
- Develop an interactive dashboard for visualizing results.

## 📊 Dataset Description

The project uses the `city_day.csv` dataset.

| Attribute | Description |
|---|---|
| Total records | 29,531 |
| Cities | 26 Indian cities |
| Time period | 2015–2020 |
| Target variable | AQI |
| Data type | Daily air quality readings |

### Dataset Features

- City
- Date
- AQI
- PM2.5
- PM10
- NO
- NO2
- NOx
- NH3
- CO
- SO2
- O3
- Benzene
- Toluene
- Xylene
- AQI_Bucket

Additional features such as Year, Month, and Season are derived from the Date column.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Data analysis and processing |
| Pandas | Data cleaning and manipulation |
| NumPy | Numerical calculations and trend fitting |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Requests | HTTP requests for population-data collection |
| BeautifulSoup | Web-related data processing |
| Google Colab | Notebook development |
| HTML | Dashboard structure |
| CSS | Dashboard styling |
| JavaScript | Interactive dashboard functionality |

## ⚙️ Methodology

### 1. Data Collection and Inspection
- Load the `city_day.csv` dataset.
- Inspect the dataset structure, columns, and data types.
- Analyze missing values and basic statistics.

### 2. Data Cleaning
- Sort records by city and date.
- Handle missing pollutant and AQI values using city-wise interpolation.
- Limit interpolation to gaps of up to seven consecutive values.
- Fill remaining missing values using city-wise medians.
- Remove rows where AQI remains missing.
- Recalculate AQI categories.

### 3. Feature Engineering
Create additional features from the Date column:

- Year
- Month
- Season

### 4. Exploratory Data Analysis
- City-wise AQI comparison
- Yearly and monthly AQI trends
- AQI category distribution
- Seasonal AQI analysis
- Pollutant correlation analysis
- Lockdown-period comparison

### 5. National AQI Trend
Calculate the daily national average AQI and fit a straight-line trend using NumPy's `polyfit()` function.

### 6. Interactive Dashboard
Develop an HTML dashboard using HTML, CSS, and JavaScript to display the analysis results interactively.

## 📈 Key Findings

| Analysis | Result |
|---|---|
| Highest average AQI | Ahmedabad – 426.7 |
| Lowest average AQI | Aizawl – 34.8 |
| Highest seasonal AQI | Winter – 214.4 |
| Lowest seasonal AQI | Monsoon – 121.3 |
| Strongest pollutant correlation | CO – 0.63 |
| Second strongest pollutant correlation | PM2.5 – 0.62 |
| Cities with lower AQI in 2020 | 19 out of 20 |
| Largest reported lockdown-period decrease | Ahmedabad – 76.3% |
| National AQI trend | Decrease of 13.3 points per year |

*Note: Correlation does not establish causation. The lockdown comparison does not prove that lockdown was the only reason for the AQI changes.*

## 📊 Interactive Dashboard

The project includes a browser-based dashboard titled:

**"How polluted is the air in India's cities?"**

Dashboard features:

- Overview of major AQI indicators
- City-wise AQI profiles
- City comparison tool
- Year explorer
- City rankings
- Yearly AQI trends
- Monthly AQI heatmap
- AQI category distribution
- Seasonal analysis
- Pollutant relationship charts
- Lockdown-period comparison
- National AQI trend
- Data quality overview

## 🚀 How to Run the Project

### Prerequisites

Install Python and the required libraries.

```bash
pip install pandas numpy matplotlib seaborn requests beautifulsoup4
```

### Step 1: Clone the Repository

```bash
git clone https://github.com/kunalkhode26-lab/air-quality-analysis.git
```

### Step 2: Navigate to the Project Directory

```bash
cd air-quality-analysis
```

### Step 3: Open the Notebook

Open the `Mini_Project_SL.ipynb` notebook in Google Colab or Jupyter Notebook.

### Step 4: Upload the Dataset

Upload the `city_day.csv` dataset when prompted.

### Step 5: Run the Notebook

Execute all notebook cells to perform data cleaning, analysis, and visualization.

### Step 6: Open the Dashboard

Open `index.html` in a web browser to explore the interactive dashboard.

## 📁 Project Structure

```text
Air-Quality-Analysis/
│
├── city_day.csv
│
├── Mini_Project_SL.ipynb
│
├── index.html
│
├── README.md
│
└── Air_Quality_Analysis_Report.pdf
```

## ⚠️ Limitations

- The dataset covers only 26 cities and a limited historical period.
- Data availability varies between cities.
- Missing-value handling may affect averages and correlations.
- The lockdown comparison cannot isolate the effect of lockdown from other factors.
- The national AQI trend is not a forecasting model.
- Population-adjusted AQI analysis is not included.

## 🔮 Future Scope

- Include more recent air quality data.
- Add more Indian cities.
- Integrate weather data such as temperature, rainfall, and wind speed.
- Improve missing-value handling techniques.
- Develop and evaluate an AQI forecasting model.
- Include population-adjusted air quality analysis.
- Publish the dashboard online.
- Add downloadable city-wise summary reports.

## 👥 Project Team

| Name | Roll Number | Batch |
|---|---|---|
| Arnav Dhait | 40 | B3 |
| Yogesh Hadge | 35 | B3 |
| Kunal Khode | 50 | B3 |
| Soumya Samarth | 52 | B4 |

**Academic Year:** 2026–2027

## 📚 References

- Dataset: `city_day.csv`
- Project Notebook: `Mini_Project_SL.ipynb`
- Interactive Dashboard: `index.html`
- Python documentation
- Pandas documentation
- NumPy documentation
- Matplotlib documentation
- Seaborn documentation

---

⭐ If you find this project useful, consider giving it a star on GitHub.


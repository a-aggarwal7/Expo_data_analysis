# Exploratory Data Analysis (EDA) on Tech Layoffs (2020–2023)

This project focuses on performing **data cleaning** and **exploratory data analysis (EDA)** using **MySQL** on a dataset of global tech layoffs from 2020 to 2023.  
The goal was to uncover trends, detect anomalies, and summarize insights to better understand layoff patterns across industries, company stages, and countries.

## Key Tasks

* **Data Cleaning**: Standardized column names, handled missing values, and removed duplicates to prepare the dataset for analysis.  
* **Trend & Pattern Analysis**: Conducted SQL-based exploratory queries to reveal major trends and relationships in the data.  
* **Outlier Detection**: Identified anomalies such as companies with unusually high layoff percentages or funding discrepancies.  
* **Insight Generation**: Summarized the findings into actionable insights highlighting the key factors driving layoffs.

## Tech Stack

* SQL (MySQL)
* MySQL Workbench / Command Line

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/a-aggarwal7/Expo_data_analysis.git
   cd Expo_data_analysis
   ```
   
2. Import the dataset into your MySQL database:

   ```bash
   LOAD DATA INFILE 'path_to/layoffs.csv'
   INTO TABLE layoffs
   FIELDS TERMINATED BY ','
   IGNORE 1 LINES;
   ```
   
3. Run the SQL scripts:
   ```bash
   SOURCE data/Data_cleaning.sql;
   SOURCE EDA_sql/EDA.sql;
   ```


4. View the results in the results/summary.txt file for key observations and insights.


## Results

* The analysis revealed several key insights:

* Most affected companies were startups with a total layoff percentage of 1, indicating complete shutdowns.

* Firms like BritishVolt (EV sector) and Quibi raised large funding amounts before failing.

* Amazon, Google, Meta, and Twitter had some of the largest total layoffs.

* Industries most impacted included consumer, retail, transportation, and finance.

* The United States had the highest layoffs, followed by India, Netherlands, Sweden, and Brazil.

* 2023 recorded the highest layoffs despite including only the first three months of the year.

* Post-IPO and acquired companies experienced higher layoff rates than early-stage startups.

* These findings provide a clearer picture of the post-pandemic tech employment landscape and help explain how economic shifts and over-expansion led to widespread layoffs.



# ✈️SkyWest Airlines | Flight Operations & On-Time Performance Analysis (2025)

## 📌Project Overview

This project analyzes SkyWest Airlines' flight operations and on-time performance in 2025 using data from the U.S. Bureau of Transportation Statistics (BTS).

The main goal is to understand SkyWest's flight volume, delay patterns, airport and route performance, and the major causes of flight delays. The project also compares SkyWest with two regional airlines, Envoy Air and Republic Airways.

**Tools:** R, Tableau  
**Data Source:** Bureau of Transportation Statistics (BTS)  
**Period:** January - December 2025  
**Dataset:** 839,821 SkyWest flight records

---

## 🎯Project Objectives

The analysis focuses on the following questions:

- How does SkyWest's flight volume change throughout the year?
- When are flights more likely to be delayed?
- Which airports and routes have higher delay rates?
- What are the main causes of flight delays?
- How does SkyWest perform compared with other regional airlines?

---

## 🗂️Data Collection & Preparation

The dataset comes from the BTS Airline On-Time Performance Data, covering January through December 2025.

R was used to prepare the data for analysis:

- Combined 12 monthly CSV files using `read.csv()` and `rbind()`.
- Standardized date formats and numerical fields.
- Checked missing values, flight status, and duplicate records.
- Created additional fields for flight routes and on-time performance.
- Prepared 839,821 SkyWest flight records with 41 fields.

---

## 📊Key Performance Indicators

The 2025 SkyWest dataset provides the following overview:

| Metric | Value |
|---|---|
| Total Flights | 839,821 |
| On-Time Performance | 80.41% |
| Average Departure Delay | 12.67 min |
| Average Arrival Delay | 9.15 min |
| Cancellation Rate | 1.41% |

Flight volume peaked in July with 75,877 flights, while February had the lowest volume with 59,806 flights.

Major operating airports included Denver (DEN), Chicago O'Hare (ORD), and Seattle (SEA).

---

## 🔍Key Findings

### 1. Monthly Delay Trends

Flight delay rates changed throughout the year, with noticeable increases during summer and December.

- December recorded the highest delay rates, with approximately 27% of arrivals and 25% of departures delayed.
- September had the lowest rates, at around 15% for arrivals and 13% for departures.
- June and July also showed relatively high delay rates.
- Arrival delay rates remained higher than departure delay rates throughout the year.

These results show that flight delays vary by season, with summer and December standing out as periods with higher delay rates.

### 2. Delay Heatmap - Day of Week & Time

The heatmap shows how departure delay rates change depending on the day of the week and scheduled departure time.

- Delay rates generally increased from morning to evening.
- Sunday between 7-8 PM had the highest departure delay rate at 29.8%.
- Wednesday and Thursday between 6-7 AM had the lowest rates at 7.9%.

Evening flights, especially on Sundays, had higher delay rates compared with early morning flights.

### 3. Airport Performance

Airport performance was compared using flight volume and departure and arrival delay rates.

- Chicago O'Hare (ORD) had relatively high departure (~28%) and arrival (~30%) delay rates.
- Denver (DEN) handled more flights but had lower delay rates than ORD.
- Salt Lake City (SLC) maintained relatively low delay rates despite handling a large number of flights.

The results show that airports with higher flight volumes do not always have higher delay rates.

### 4. Route Performance

The route-level analysis compares departure and arrival delay rates across selected routes.

- ORD-MKE had the highest departure (31.7%) and arrival (32.9%) delay rates among the displayed routes.
- DEN-COS and COS-DEN also showed relatively high delay rates.
- Routes between SFO and LAX had comparatively lower delay rates.

Looking at individual routes helps identify differences that may not be visible when analyzing overall airline performance.

### 5. Delay Causes Analysis

The analysis examines total delay minutes, delay distribution, and average delay duration across different causes.

- Carrier-related delays accounted for approximately 6.82 million delay minutes in 2025, the largest total among the delay categories.
- In December, carrier-related delays represented 44.2% of classified delay minutes.
- Carrier-related delays also had the highest average delay duration in December at 47.9 minutes.

Carrier-related delays stood out as the largest contributor to total delay minutes and had the longest average duration in December.

### 6. Competitor Comparison

SkyWest was compared with Envoy Air and Republic Airways based on similar average flight distances.

- SkyWest had the lowest cancellation rate at approximately 1.4%.
- Its average departure delay was 17.2 minutes in the comparison, higher than both competitors.
- Carrier-related delays accounted for 47.6% of SkyWest's classified delay minutes, compared with 23.3% for Republic Airways and 20.4% for Envoy Air.

Although SkyWest had fewer cancellations, its average departure delay duration was longer than the other two regional airlines.

---

## 📈 Dashboard Preview

### Monthly Delay Trends
![Monthly Delay Trends](images/Monthly%20Delay%20Trends.png)

### Delay Heatmap
![Delay Heatmap](images/Delay%20Heatmap.png)

### Delay Causes Analysis
![Delay Causes Analysis](images/Delay%20Causes%20Analysis.png)

For the complete analysis, including airport performance,
route comparisons, and competitor benchmarking,
see the [Full Project Presentation](presentation/SkyWest_Analysis_2025.pdf).

---

## 📁 Project Files

| File | Description |
|---|---|
| [Full Project Presentation](presentation/SkyWest_Analysis_2025.pdf) | Complete analysis report covering flight operations, delay patterns, and competitor comparison |
| [SkyWest Cleaned Dataset](data/skywest_sample.csv) | Cleaned 2025 SkyWest flight records used for analysis |
| [All Airlines Cleaned Dataset](data/all_airlines_cleaned.csv) | Cleaned airline dataset used for comparison across carriers |
| [Dashboard Screenshots](images/) | Tableau visualizations used in the project |

**Note:** Sample datasets are provided due to file size limits. The analysis was conducted using the complete 2025 datasets from BTS.

---

## 👤My Focus

This was a team project. My main focus was analyzing flight delay patterns and operational performance using Tableau.

I worked on the monthly delay trends, delay heatmap, airport performance, route performance, and delay causes analysis.

Through these analyses, I explored how flight delays change across different months, departure times, airports, and routes, as well as which delay categories contribute the most delay minutes.

Other parts of the project, including data preparation, the KPI overview, and competitor comparison, were completed by my teammates.

---

## 📚Data Source

U.S. Department of Transportation - Bureau of Transportation Statistics (BTS)

Airline On-Time Performance Data, 2025

https://www.transtats.bts.gov/

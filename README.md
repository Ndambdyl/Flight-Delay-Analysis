# ✈️ Flight Delays Analysis Project

## 1. Project Overview
This project explores U.S. flight delay data to identify factors that influence delays and cancellations.  
It demonstrates an **end-to-end data workflow**: data collection, cleaning, analysis (SQL & Python), visualization (Power BI), and final reporting.

**Business Question:**  
- What factors most influence flight delays in the U.S.?  
- Which airlines and airports are most affected?  
- Are there seasonal trends in delays?  

---

## 2. Project Workflow
1. **Data Collection**  
   - Source: Bureau of Transportation Statistics (BTS) On-Time Performance Dataset
   - Years: Filtered to 2023, 2024, 2025
   - Variables: Airline, Origin/Destination Airport, Flight Date, Departure Delay, Arrival Delay, Cancellation Reasons
   - file: `Airline_Delay_Cause.xlsl`
   - Stored in `data`

2. **Data Cleaning & Preparation**  
   - Handle missing values  
   - Convert date/time formats
   		- Converted 'Year' and 'Month' columns to a single 'Date' column to ease filtering dates.
   - Create calculated columns (e.g., `Is_Delayed`, `Delay_Category`)  

3. **Exploratory Data Analysis (EDA)**  
   - Flights delayed vs on-time  
   - Delays by airline, airport, season  
   - Trends across months  

4. **Data Modeling**  
   - Star schema: fact (flights) + dimensions (airlines, airports, dates)

5. **Analysis**  
   - SQL queries for aggregation & ranking  
   - Python (pandas, matplotlib) for deeper insights  

6. **Visualization**  
   - Power BI dashboard with KPIs, maps, trends, and filters  

7. **Final Report**  
   - Insights & recommendations for airlines/airports  

---

## 3. Repository Structure

flight-delays-analysis/
│── data/        → raw + cleaned CSVs
│── notebooks/   → Python notebooks for EDA + analysis
│── sql/         → SQL queries
│── dashboard/   → Power BI file (.pbix)
│── report/      → Final PDF or Markdown report
│── README.md    → Main project page (portfolio showcase)

---

## 4. Tools & Technologies
- **Python** (pandas, matplotlib, seaborn)  
- **SQL** (joins, aggregates, window functions)  
- **Power BI** (dashboard & visuals)  
- **GitHub** (version control, portfolio showcase)  

---

## 5. Example Insights (to be filled later)
- Airline X has the highest delay rate (avg XX mins).  
- Delays peak in summer months due to weather + high traffic.  
- Hub airports show significantly higher delay rates.  

---

## 6. Next Steps
- Add machine learning predictions (optional)  
- Expand analysis to international flights 

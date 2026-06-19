

# Comparative Dollar-Cost Averaging (DCA) Analysis: Major Index ETFs

## 📌 Project Overview
This project evaluates the long-term performance of a **Dollar-Cost Averaging (DCA)** strategy across five of the most popular index-tracking ETFs: **SPY, VOO, IVV, QQQ, and VTI**. 

By simulating a disciplined investment of **$1 per day over a 10-year period**, this analysis highlights the impact of ETF choice on final portfolio wealth.

---

## 🛠️ Tech Stack & Skills
* **Data Sourcing:** Historical financial data extraction (Investing.com).
* **Data Cleaning & Preprocessing:** Handling missing time-series data, alignment of non-synchronous trading calendars.
* **Data Visualization:** Tableau (interactive dashboarding, trend analysis).

---

## 📁 Dataset & Data Cleaning Challenge
The raw data spans 10 years of daily historical closing prices. 

### The Challenge: Asynchronous Trading Dates
Because different funds occasionally recorded prices on days others didn't (due to localized data anomalies, settlement differences, or exchange holidays), the dates did not perfectly align across all five CSVs. Leaving this unaddressed would have skewed the DCA simulation results.

### The Solution
Using Excel, the data was thoroughly cleaned and standardized by:
1. Outer-joining the datasets on the `Date` column to identify gaps.
2. Imputing or dropping mismatched dates where trading didn't actually occur across the broader market, ensuring a perfectly synchronized 10-year timeline for an unbiased comparison.

---

## 🧮 Investment Simulation Methodology
To simulate a real-world $1/day DCA strategy, Excel functions were used to calculate the return for each trading day:

1. **Fractional Share Calculation:** Each day, the $1 investment buys a fractional unit of the ETF based on that day's closing price 
2. **Cumulative Portfolio Balance:** The total shares accumulated and are tracked and re-valued daily.
3. **Output:** The spreadsheet generated a clean, unified time-series dataset tracking the growth of the principal versus the total portfolio value for all 5 assets over the 10-year span.

---

## 📊 Visualizations & Insights
The finalized dataset was imported into **Tableau** to create an interactive line chart tracking the growth of the five portfolios over time.

### Key Takeaways from the Analysis:
* **QQQ Outperformance:** Due to the massive tech bull run over the last decade, QQQ significantly outperformed the S&P 500 and Total Market funds, despite experiencing higher volatility.
* **The S&P 500 Clones:** SPY, VOO, and IVV performed almost identically, visually demonstrating that expense ratio differences of a few basis points have minimal visual separation even over 10 years, though VOO and IVV slightly edge out SPY.




<img width="2495" height="1280" alt="Screenshot 2026-06-19 at 1 30 40 PM" src="https://github.com/user-attachments/assets/d17b4389-d38f-411c-88ec-32ca72246079" />
<a href="https://public.tableau.com/views/Top5ETFInvestments112014-12312024/Sheet2?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link" target="_blank">Link To Tableau Dashboard</a>


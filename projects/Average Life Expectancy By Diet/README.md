# Dietary Patterns and Longevity: A Comparative Life Expectancy Analysis

## 📌 Project Overview
This project investigates the correlation between various popular dietary frameworks and projected life expectancy. By aggregating data across multiple public health and media sources, the analysis contrasts nine distinct diets: **Mediterranean, Vegan, Flexitarian, Vegetarian, Atkins, Keto, Paleo, Raw Food, and Carnivore**. 

The goal of this project is to provide a normalized, data-driven comparison of how whole-food-focused, plant-forward, and restrictive high-protein/low-carb diets stack up against one another regarding long-term longevity metrics.

---

## 🛠️ Tech Stack & Skills
* **Data Sourcing:** Multi-source web extraction of health and longevity data.
* **Data Normalization:** Data aggregation, cross-source conflict resolution, and statistical averaging using spreadsheet modeling.
* **Data Visualization:** Design and implementation of structured data visualizations (Bar Charts) to clearly communicate comparative metrics.

---

## 📁 Data Sourcing & Aggregation Challenge
The dataset was compiled from three distinct publishing and health-reporting platforms: **Healthline.com, Health.com, and The Guardian**. 

### The Challenge: Discrepant Reporting Metrics
Each source reported slightly different life expectancy estimates, baseline populations, or observational metrics for the same dietary patterns. Using a single source would introduce bias, while leaving the data unaligned would create an inconsistent narrative.

### The Solution: Cross-Source Normalization
To establish a reliable baseline for each diet, a data aggregation pipeline was built in a spreadsheet:
1. **Extraction:** Collected all historical and observational life expectancy data points across all three sources for the 9 distinct diets.
2. **Standardization:** Aligned the disparate metrics into a singular comparative matrix.
3. **Statistical Averaging:** Calculated the arithmetic mean of the life expectancy estimates across the sources to smooth out individual publisher variances, yielding a singular, balanced average for each dietary framework.

---

## 📊 Visualizations & Insights
The aggregated data was compiled into a comprehensive **bar chart** to visually contrast the average projected life expectancies of the nine diets side-by-side.

### Key Frameworks Analyzed:
* **Plant-Forward & Balanced:** Mediterranean, Vegan, Flexitarian, Vegetarian.
* **Low-Carb & High-Protein/Fat:** Atkins, Keto, Paleo, Carnivore.
* **Alternative/Restrictive:** Raw Food.

### Key Takeaways from the Analysis:
* **The Plant-Forward Advantage:** (*Diets emphasizing high fiber, plant fats, and whole grains—like the Mediterranean and Flexitarian diets—consistently averaged the highest life expectancies across the aggregated data.*)
* **High-Restriction/Low-Carb Variances:** (*Extreme low-carbohydrate or highly restrictive protocols showed more significant variance across sources, ultimately averaging lower projected longevity metrics compared to more balanced, sustainable dietary patterns.*)
<img width="965" height="1159" alt="Screenshot 2026-06-20 at 3 55 10 PM" src="https://github.com/user-attachments/assets/ac189263-2b32-4740-af96-5cc67778c07f" />

<a href="https://public.tableau.com/views/AverageLifeExpectancyByDiet/Sheet3?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link" target="_blank">Link To Tableau Dashboard</a>

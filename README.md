## Addis Ababa Road Traffic Flow Analysis (2024) – README v2.0🚦 
## Explanatory Data Science Project

Synthetic traffic dataset and statistical analysis for the Megenagna → Ayat, Addis Ababa.

**Project Overview**

This project analyzes daily traffic flow along one of Addis Ababa’s major arterial roads connecting **Megenagna Square to Ayat Square (8.1 km).**

**Objective:**

To explain what **drives daily traffic variation** using statistical modeling, while incorporating **realistic variability** to reflect stochastic behavior seen in urban traffic.

This dataset allows for:
- Interpretable regression analysis
- Scenario exploration (holidays, school closures, rain)
- Future ML-based prediction modeling

⚠️ Disclaimer
Some values in this dataset are **synthetic or estimated** for demonstration purposes. While traffic patterns are designed to be realistic, **not all numbers correspond to actual observed traffic.**

This project emphasizes **explanatory modeling** rather than exact real-world measurements.

📄 **Version**
**v2.0 – 2026-02-11**

- Added stochastic traffic variation to improve realism
- Emphasized explanatory modeling using OLS regression
- Clarified disclaimer for synthetic data
- Highlighted future ML modeling potential

Previous versions (v1.0) focused on deterministic simulation and are accessible via Git history.

**Urban Context**
- **City population:** ~12 million
- **Estimated road usage:** ~35% of residents
- **Traffic ranking:** 3rd busiest of the city’s five main gateways
- **Intersections:** Two major connecting roads

Road serves: High-income residential areas, newly developed condominiums, construction zones, intercity buses, and freight vehicles

**Vehicle Composition**
|Vehicle Type|	Description|
|------------|--------------|
|🚗 Automobile|	Dominant share (high car ownership areas)|
|🚌 Minibus	|Local public transport (5× city buses)|
|👩‍💼 Public Servant Bus|	50 total (work hours only)|
|🚌 Public Bus	|60 city + 20 intercity|
|🚚 Pickup Truck	|Construction & delivery|
|🏍️ Motorcycle	|Local commuters|
📊 Dataset Description

Daily observations for 365 days of 2024, including:

|Traffic Counts|Event Indicators (Binary 0/1)|
|--------------|-----------------------------|
|Automobile|PublicHoliday|
|Minibus|MarketDay|
|PublicServantBus|ReligiousEvent|
|PublicBus|Semester_break|
|PickupTruck|Long_Closure|
|Motorcycle||
|Total_Traffic||

**Weather**
- Heavy rain events (randomly distributed during rainy season)

**Temporal Patterns & Stochastic Enhancements**

- **Weekly Trends:** Monday → busiest; Thursday & Friday → lighter traffic
- **School Calendar:** Semester break (March 1–5), Long closure (June 22 – Sept 13)
- **Special Events:** January 19 → low traffic, April 16–19 → peak period, September 9–11 & 27–28 → extreme variation, monthly spiritual days (2nd & 30th)
- **Seasonality:** Smooth yearly variation
- **Random Variation:** Daily traffic fluctuates ±3–5% around baseline

**Analytical Objective**

Main question:
        
        Which factors significantly influence daily traffic volume on this corridor?

This project emphasizes interpretation rather than prediction, using OLS regression while incorporating realistic variability to ensure robust and meaningful coefficients.

**Methodology**

Regression model:

Total_Traffic ~
Day_of_Week +
PublicHoliday +
ReligiousEvent +
Semester_break +
Long_Closure +
HeavyRain

**Enhancements Over Purely Deterministic Data**
- Random daily fluctuations around baseline traffic
- Event effects vary slightly day-to-day (±10%)
- Smooth seasonal trends
- Optional interaction terms (e.g., Monday × PublicHoliday)
- Small lag effect (traffic influenced by previous day’s level)

These adjustments ensure that the regression captures true effect sizes while reflecting realistic urban traffic variation.

**Model Outputs**
The regression provides:
- Coefficient estimates (impact size in vehicles)
- Statistical significance (p-values)
- Model explanatory power (R²)
- Residual diagnostics

**Example Insights**
- Mondays increase traffic by ~2,000 vehicles on average
- Public holidays reduce traffic by 15–25% depending on day-of-week
- Heavy rain decreases traffic by 5–10%
- Long school closures reduce daily demand significantly
- Coefficients are interpretable, capturing both expected trends and realistic daily variability.

📁 Sample Dataset Preview (Preview retained from previous README) 

⚠️ Full dataset includes all 365 days of 2024.  Download CSV: Simulated_Traffic_2024.csv

**Why This Project Matters**
Demonstrates:
- Translation of urban domain knowledge into structured data
- Feature engineering with stochastic realism
- Statistical modeling for interpretation
- Quantification of traffic drivers
- Foundation for future predictive ML modeling

**Tools Used**: | Python | pandas | statsmodels | scikit-learn | Matplotlib |

**Future Evolution**

Planned next steps:
- Time-series forecasting using lag features
- ML-based traffic prediction (Random Forest, XGBoost, LSTM)
- Nonlinear interaction analysis
- Congestion saturation modeling

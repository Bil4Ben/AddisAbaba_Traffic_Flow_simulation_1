# AddisAbaba_Traffic_Flow_simulation_1
**Synthetic traffic dataset and analysis for a city road from Megenagna Square to Ayat Square,** Addis Ababa
City Road Traffic Flow Analysis (2024)

##  Overview

This repository contains a synthetic dataset representing traffic flow along a major city road in Addis Ababa, Ethiopia, connecting Megenagna Square to Ayat Square. The dataset is created for demonstration, regression modeling, and scenario analysis of traffic patterns.

**Note:** The problem formulation and dataset were generated with ChatGPT assistance, based on a mix of real facts provided by the author and estimates/assumptions to create a realistic daily traffic dataset.

## Road Details

- **Route:** Megenagna Square → Ayat Square

- **Length:** 8.1 km

- **Branches:** Extends toward newly developed condominiums and surrounding villages

- **Intersections:** Two major city roads along the route

## City Context

- *Population:* 12 million

- *Road usage:* ~35% of city residents

- *Traffic:* Commuters, public transport, intercity buses, trucks, and construction vehicles

- *Ranking:* Third busiest of the city's five main gatways

## Vehicle Types & Counts (Along this road)**


| Vehicle Type               | Count / Description                         |
|----------------------------|--------------------------------------------|
| 🚗 Automobile              | 300,000 (high-income villages along the road) |
| 🚌 Minibus                  | 5 × city buses (local public transport)    |
| 👩‍💼 Public Servant Bus     | 50 total (10 per route, work hours only)   |
| 🚌 Public Bus               | 60 city buses + 20 intercity buses         |
| 🚚 Pickup Truck             | Minor share (construction & delivery vehicles) |
| 🏍️ Motorcycle              | Minor share (local commuters)              |

## Temporal Patterns
- Weekly Trends:
    - Monday → busiest
    - Thursday & Friday → lighter traffic
- Semester & School Events:
  - Semester break: March 1–5 → drop in traffic
  - Long school closure: June 22 – Sept 13 → significant decrease
- Holidays & Special Days: January 19 (low), April 16–19 (peak), Sept 9–11 & 27–28 (extreme variation), Monthly spiritual days (2nd & 30th)
- Weather Effects:
    - Heavy rain events: 10 random days between June 30 – August 10
    - Reduces traffic for automobiles, minibuses, motorcycles, and pickup trucks
 
| **Date**       | **🚗 Automobile** | **🚌 Minibus** | **👩‍💼 Public Servant Bus** | **🚌 Public Bus** | **🚚 Pickup Truck** | **🏍️ Motorcycle** | **Total_Traffic** | **🎉 PublicHoliday** | **🛒 MarketDay** | **✝️ ReligiousEvent** | **🏫 Semester_break** | **🏖️ Long_Closure** |
|----------------|-----------------|----------------|----------------------------|-----------------|-------------------|-----------------|-----------------|------------------|----------------|-------------------|-----------------|----------------|
| 2024-03-01 | 10250 | 510  | 50  | 80  | 30  | 200 | 11020 | 0 | 0 | 0 | 1 | 0 |
| 2024-03-02 | 10500 | 520  | 50  | 82  | 32  | 210 | 11394 | 0 | 0 | 0 | 1 | 0 |
| 2024-03-03 | 10700 | 530  | 50  | 85  | 35  | 215 | 11515 | 0 | 0 | 0 | 1 | 0 |
| 2024-03-04 | 10400 | 525  | 50  | 80  | 33  | 205 | 11293 | 0 | 0 | 0 | 1 | 0 |
| 2024-03-05 | 10300 | 515  | 50  | 78  | 30  | 200 | 11173 | 0 | 0 | 0 | 1 | 0 |
| 2024-03-06 | 10800 | 540  | 50  | 90  | 35  | 220 | 11635 | 0 | 1 | 0 | 0 | 0 |
| 2024-03-07 | 10950 | 550  | 50  | 92  | 38  | 225 | 11805 | 0 | 0 | 0 | 0 | 0 |
| 2024-03-08 | 10750 | 535  | 50  | 88  | 35  | 215 | 11473 | 0 | 0 | 0 | 0 | 0 |
| 2024-03-09 | 10850 | 540  | 50  | 90  | 36  | 220 | 11686 | 0 | 0 | 0 | 0 | 0 |
| 2024-03-10 | 10600 | 530  | 50  | 85  | 34  | 210 | 11409 | 0 | 0 | 0 | 0 | 0 |
| 2024-03-11 | 10700 | 535  | 50  | 88  | 35  | 215 | 11473 | 0 | 0 | 0 | 0 | 0 |
| 2024-03-12 | 10850 | 540  | 50  | 90  | 36  | 220 | 11686 | 0 | 0 | 0 | 0 | 0 |
| 2024-03-13 | 11000 | 550  | 50  | 92  | 38  | 225 | 11955 | 0 | 1 | 0 | 0 | 0 |
| 2024-03-14 | 11100 | 555  | 50  | 95  | 40  | 230 | 12170 | 0 | 0 | 0 | 0 | 0 |
| 2024-03-15 | 10950 | 550  | 50  | 92  | 38  | 225 | 11805 | 0 | 0 | 0 | 0 | 0 |
| 2024-03-16 | 10800 | 540  | 50  | 90  | 36  | 220 | 11636 | 0 | 0 | 0 | 0 | 0 |
| 2024-03-17 | 10750 | 535  | 50  | 88  | 35  | 215 | 11473 | 0 | 0 | 0 | 0 | 0 |
| 2024-03-18 | 10900 | 545  | 50  | 90  | 37  | 225 | 11847 | 0 | 0 | 0 | 0 | 0 |
| 2024-03-19 | 11050 | 550  | 50  | 92  | 38  | 230 | 12110 | 0 | 1 | 0 | 0 | 0 |
| 2024-03-20 | 11100 | 555  | 50  | 95  | 40  | 235 | 12275 | 0 | 0 | 0 | 0 | 0 |

⚠️ Note: This is a sample preview. The full dataset contains all 365 days of 2024

## Full Dataset

Download the full CSV: [traffic_2024.csv]
## Dataset Objectives
- Daily traffic counts by vehicle type
- Total traffic per day (Total_Traffic)
- Indicator columns for events: PublicHoliday, MarketDay, ReligiousEvent, Semester_break, Long_Closure
- Reflects realistic variations: weekly patterns, holidays, school closures, heavy rain, seasonal traffic

## Intended Analysis
- Regression modeling (OLS, scikit-learn)
- Scenario simulation for holidays, closures, and weather
- Urban traffic planning and infrastructure optimization


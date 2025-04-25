# The Death Penalty and lethal crime: A multi-city analysis with socioeconomic insights at the State and City Levels

## PowerBI Dashboard
Link: https://app.powerbi.com/view?r=eyJrIjoiOWIyNzM4MTItOTE3ZC00MmQ0LWE0MTUtMWRjM2NhYmNlNTVkIiwidCI6IjEwMWRhNTg3LTE4NDMtNGY1Mi04YjhhLTE3YjA2OWM2NmQzMyIsImMiOjJ9



## Table of Contents
* [PowerBI Dashboard](#Tableau-dashboard)
* [Motivation](#motivation)
* [Questions](#questions)
* [Normalizing the Data](#normaling-the-data)
* [Problems and Hurdles](#problems-and-hurdles)
* [Technologies Used](#technologies-used)
* [Sources](#sources)
* [Conclusion](#conclusion)

## Motivation:
As someone passionate about both social issues and data storytelling, I wanted to explore the real-world impact of the death penalty on lethal crimes. Coming from Poland - a country without capital punishment — I’ve always been curious about how such a policy might influence crime rates, particularly those relevant to the death penalty.

Capital punishment remains one of the most controversial topics in the U.S., often discussed without a deep dive into the data behind it. This project gave me the opportunity to combine my interest in justice, public policy, and socioeconomic disparities. I focused on six major U.S. cities, analyzing murder rates, state-level unemployment, and city-level poverty and education levels, aiming to uncover meaningful patterns and offer a more nuanced view of the factors that surround lethal crime.

## Questions:
1) How do murder rates compare between cities with and without active use of the death penalty?
2) How have homicide rates changed from 2021 to 2024 across the selected cities, and which cities experienced the most    significant increases or decreases?
3) What do state-level unemployment rates suggest about crime trends?
4) How do city-level poverty and education rates correlate with lethal crime rates?

## Normalizing the Data
The primary dataset contained detailed crime records across multiple U.S. cities. I selected and normalized the relevant columns to focus the analysis specifically on lethal crimes that could be impacted by the presence or absence of the death penalty. This included narrowing down to key categories such as justifiable homicide, voluntary manslaughter, involuntary manslaughter, and potential homicide/death. These categories were chosen because they best reflect the types of crimes typically considered in capital punishment cases.

Dates were standardized across datasets to ensure consistency, especially when pairing crime data with socioeconomic indicators. I also cleaned and aggregated external datasets covering state-level unemployment, city-level poverty, and education rates to align with the same timeframes and geographic levels.

For city-to-city comparisons, I selected two cities—one in a state with an active death penalty and one without it. These cities had overlapping but varied data availability, so I aligned the analysis based on the most consistent timeframes available, which included 2019–2024, 2015–2024, and 2020–2024, depending on the dataset.

## Problems and Hurdles
Cleaning and aligning data from six different cities came with challenges, especially when standardizing inconsistent column names and city definitions. Filtering for homicide-related crimes and categorizing them into four key types—justifiable homicide, voluntary manslaughter, involuntary manslaughter, and potential homicide/death—was tricky due to varying crime descriptions. RegEx was essential for accurate classification.

Extracting dates, months, and times, assigning crimes to time-of-day categories, and merging population data added complexity. Combining all six cities into one dataset for comparative analysis was demanding, especially when managing large files. Balancing city-level crime data with state-level socioeconomic indicators also required careful alignment across different timeframes.

## Technologies Used
1) Python / Pandas / RegEx — for data exploration, cleaning, categorization, and aggregation
2) Power BI — for creating an interactive dashboard
3) PowerPoint - for visualizations of dashboard
4) Git - for version control

## Data Sources
To answer the above questions I used the following sources to collect datasets for my analysis

1) Crime Data from city-specific Open Data Portals (2015–2024)
* Minneapolis, MN - https://opendata.minneapolismn.gov/datasets/cityoflakes::crime-data/about 
* Houston, TX - https://www.houstontx.gov/police/cs/Monthly_Crime_Data_by_Street_and_Police_Beat.htm
* Chicago, IL - https://data.cityofchicago.org/Public-Safety/Crimes-2001-to-Present/ijzp-q8t2/about_data 
* Milwaukee, WI - https://data.milwaukee.gov/dataset/wibrarchive/resource/395db729-a30a-4e53-ab66-faeb5e1899c8 
* San Francisco, CA - https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-2018-to-Present/wg3w-h783/about_data
* Phoenix, AZ - https://www.phoenixopendata.com/dataset/crime-data
2) U.S. Census Bureau - Population , Poverty and Education Data by City
https://data.census.gov/
3) Death Penalty Information Center - Status of Death Penalty by State
https://deathpenaltyinfo.org/state-and-federal-info/state-by-state
4) Unemployment Rates by State
https://www.kaggle.com/datasets/justin2028/unemployment-in-america-per-us-state
5) State Crime (1976-2019)
https://corgis-edu.github.io//corgis/csv/state_crime/


## Conclusion
From 2020 to 2024, cities in states without the death penalty consistently showed higher homicide rates per capita than those with it. While bachelor’s degree attainment was high across all cities, high school graduation rates revealed a clearer pattern—cities with lower graduation rates tended to have higher homicide rates.

Unemployment data varied by state and year, making patterns less consistent, though some correlations were observed. Most cities saw a spike in homicides in 2021, followed by a decline—except for San Francisco, which peaked in 2022–2023 before dropping in 2024.

These findings suggest that factors like basic education and policy may have a stronger influence on crime rates than previously assumed, warranting further investigation.

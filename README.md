# Project Documentation

_by Luis Millet and Gian F. Villafañe_

## Project Title: Changes in Population due to Migration of Young Puerto Ricans

## Introduction:

This project aims to investigate the influence of various phenomena and events that have occurred in Puerto Rico on the migration patterns of Puerto Ricans leaving their island. By analyzing census data from Puerto Rico and the data from The World Bank on "Net migration" spanning the years 2015 to 2022, we seek to understand the demographic trends and factors driving migration.

## Hypotheses:

1. **Demographic Trend Hypothesis:** The majority of individuals migrating from Puerto Rico during the period from 2015 to 2022 are younger than 30 years old, driven by variations in job availability, wages, and quality of life. This hypothesis suggests that younger individuals, particularly those under 30, are more likely to migrate due to factors such as education opportunities, career advancement, or economic challenges.

2. **Policy Influence Hypothesis:** Changes in federal policies and governance, including the implementation of PROMESA in 2016, influenced migration patterns of Puerto Ricans. Political and policy changes, such as the establishment of the federal oversight board under PROMESA, are expected to have affected migration decisions among Puerto Ricans, either by encouraging or discouraging migration.

3. **Natural Disaster Impact Hypothesis:** Natural disasters such as Hurricane Maria in 2017 resulted in a significant temporary surge in migration from Puerto Rico. This hypothesis suggests that the impact of natural disasters on Puerto Rico led to a temporary increase in migration to the outside as individuals sought refuge and opportunities elsewhere.

## Data Sources:

1. **The World Bank:** The data from The World Bank on "Net migration" for Puerto Rico provides information on the net migration rate in Puerto Rico over a certain period. Net migration refers to the difference between the number of immigrants (people moving into Puerto Rico) and emigrants (people leaving Puerto Rico) per 1,000 population.

   - Excel: [Link](https://api.worldbank.org/v2/en/indicator/SM.POP.NETM?downloadformat=excel)

2. **United States Census Bureau:** The data from the United States Census Bureau includes demographic information from the American Community Survey (ACS) 5-Year Estimates Subject Tables for the years 2015 to 2022.
   - API: [Link](https://api.census.gov/data/{year}/acs/acs5)
   - 2015-2022: [Link](https://api.census.gov/data/2022/acs/acs5/subject)

## Data Wrangling, Cleaning & Manipulation

To clean and filter The World Bank data on "Net migration" for Puerto Rico, we specifically:

- Extracted the relevant information related to our research questions and hypotheses.
- Filtered the data to include only information concerning Puerto Rico.
- Visualized the data to identify the availability of years between 2015 and 2022.
- Renamed the columns to their respective years.
- Dropped the unnecessary data.
- Merged this cleaned dataset with the census data.

Cleaning the Puerto Rico ACS Data from 2015-2022 presented its own set of challenges. We undertook the following steps to ensure data integrity and relevance:

- Extracted relevant information pertaining to total population, population aged 0-35, and median age across the years.
- Filtered the data retrieved from the Census API and CSV files for the respective years.
- Removed any unnecessary or outlier data points.
- Visualized the extracted data to analyze trends from 2015 to 2022.
- Merged this cleaned dataset with The World Bank data for comprehensive analysis.
- Conducted a comparative analysis of all datasets to validate their relevance to the project's objectives.

## Findings & Interpretation:

### Overall Trend:

- From 2015 to 2017, there was a consistent negative net migration, indicating more people leaving Puerto Rico than moving in. This supports the hypothesis that external factors, such as economic challenges or political changes, might be influencing migration patterns.
- In our analysis of demographic trends in Puerto Rico, we observed a significant decline in the overall population from 2015 to 2022, along with notable changes in the age composition of the island. The median age increased, suggesting an aging population with fewer young people.
- The negative net migration trend continued but at a reduced rate in 2018 and 2019. This could be attributed to changes in economic conditions or other factors influencing migration decisions.
- Interestingly, in 2020 and 2021, the trend shifted to a smaller negative net migration, indicating a slight improvement compared to previous years. This could suggest changes in external factors or policies influencing migration patterns.
- In 2022, there was a notable reversal with a positive net migration, contradicting the previous trend. This could indicate significant changes in factors influencing migration, such as economic opportunities or policy changes.

### Comparison with Hypotheses:

1. **Demographic Trend Hypothesis:** [Approved] The data indicates a consistent decline in the total population for ages 0-35 in Puerto Rico from 2015 to 2022. This decline suggests a decrease in the younger population cohort over the years, supporting the hypothesis that younger individuals are migrating from Puerto Rico. The negative net migration trend aligns with the hypothesis that younger individuals may be migrating due to factors like job availability and economic challenges.

2. **Policy Influence Hypothesis:** [Inconclusive] The implementation of PROMESA in 2016 coincides with a period of significant demographic changes in Puerto Rico. While the data does not directly measure the impact of PROMESA on migration patterns, it provides insights into broader demographic trends during this period. The fluctuations in net migration over the years coincide with potential policy changes or economic conditions, supporting the idea that governance and policy decisions can influence migration patterns.

3. **Natural Disaster Impact Hypothesis:** [Inconclusive] While the data indicates a temporary surge in migration from Puerto Rico following natural disasters such as Hurricane Maria in 2017, the collected data from the World Bank's Net Migration dataset for Puerto Rico refutes this claim. While natural disasters can lead to increased migration as individuals seek refuge and opportunities elsewhere, a more in-depth analysis must be conducted to ascertain the legitimacy of this data.

### Conclusion:

The net migration data for Puerto Rico reveals a steady decline in the 8-year period, suggesting a relationship between migration patterns and various influencing factors. The data partially supports the hypotheses regarding demographic trends, policy influence, and natural disaster impacts on migration patterns in Puerto Rico, emphasizing the need for further analysis to understand the factors driving population dynamics in the region. Further research is necessary to confirm the hypotheses and gain an understanding of the multifaceted factors driving population dynamics in the region.

## References:

- U.S. Census Bureau. (n.d.). AGE AND SEX. American Community Survey, ACS 5-Year Estimates Subject Tables, Table S0101, 2015-2022. Retrieved Month Day, Year, from [Link](https://data.census.gov/table/ACSST5Y2020.S0101?moe=false)

- World Bank. (n.d.). Net migration - Puerto Rico [Data file]. Retrieved Month Day, Year, from [Link](https://data.worldbank.org/indicator/SM.POP.NETM?end=2023&locations=PR&start=2015)

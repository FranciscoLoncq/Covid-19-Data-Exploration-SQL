# Covid-19-Data-Exploration-SQL
## Overview
This project explores Covid-19 deaths and vaccination data from the source [Dataset: CovidDeaths](https://ourworldindata.org/covid-deaths) This exploratory analysis looks to obtain insights on how the pandemic affected differently each region of the world.
## Analysis
Overview of Achievements in the Project:

## 1. Initial Data Exploration:
Retrieved and compared data from the CovidDeaths table, filtering out records where the continent is not specified.

## 2. Selecting Relevant Data:
Extracted key columns (Location, Date, Total_Cases, New_Cases, Total_Deaths, Population) from the CovidDeaths table.
Ordered the data for analysis based on Location and Date.

## 3. Analyzing Likelihood of Death in country of interest (Argentina):
Calculated the death percentage in Argentina by dividing Total_Deaths by Total_Cases and multiplying by 100.
Examined the progression of this percentage over time.

## 4. Population Infection Rate in a country of interest (Argentina):
Calculated the infection rate in Argentina by dividing Total_Cases by Population and multiplying by 100.
Explored the temporal changes in the infection rate.

## 5. Which ountries have the Highest Infection Rates:
Identified countries with the highest infection rates compared to their population.
Calculated the infection rate as a percentage of the population for each country.

## 6. Countries with Highest Death Count Per Capita:
Updated the CONTINENT column, setting it to NULL where it was empty.
Examined and ranked countries with the highest death count per capita.

## 7. Breakdown by Continent and Global Numbers:
Investigated the total daily cases, total daily deaths, and daily death percentage globally and by continent.
Analyzed the overall global numbers for new cases, new deaths, and the death percentage.

## 8. Rolling Vaccination Metrics:
Combined data from the CovidDeaths and CovidVaccinations tables.
Computed the rolling count of people vaccinated over time for each location.
Using CTE and Temporary Table for Analysis:

## 9. Utilized a Common Table Expression (CTE) to calculate the rolling count of people vaccinated.
Implemented a temporary table to store and analyze the percentage of the population vaccinated over time.

## 10. Creating a View for Visualization:

Established a view named PercentPopulationVaccinated to store the data for subsequent visualizations.
The view incorporates the rolling count of people vaccinated and related information.

These SQL queries and analyses collectively provide a comprehensive exploration of COVID-19 data, covering infection rates, death rates, vaccination progress, and other key metrics across various geographical locations. The project facilitates further analysis and visualization to gain insights into the impact of the pandemic.

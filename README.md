# Global Terrorism Risk Dashboard

This Power BI dashboard analyses global terrorism incidents from 2011 to 2020, focusing on event frequency, fatalities, attack success, and country-level risk adjusted by population.

## Dashboard Preview

![Dashboard Overview](images/dashboard_overview.png)

## Project Objectives

- Analyse terrorism event distribution across countries and years.
- Compare country-level risk using events per million people.
- Explore attack types, target types, weapon types, and active organisations.
- Provide interactive drill-down from country-level risk to event locations.

## Key Features

- Choropleth map showing terrorism events per million people.
- Year slicer for temporal filtering.
- Country-level overview panel with total events, fatalities, and average deaths per event.
- Dynamic Top 5 charts for attack types, target types, organisations, and weapon types.
- Event location map that displays incident points after selecting a country.

## Data Model

The dashboard uses a star-schema style model:

- Fact table: terrorism events
- Dimension tables: country, geography, attack type, target type, weapon type, organisation, date
- Population fact table: yearly population by country

The key calculated metric is:

`Events per million people = Total Events / Population * 1,000,000`

## Tools Used

- Power BI
- DAX
- Power Query
- Python / Excel for data preparation
- Global Terrorism Database
- Population data

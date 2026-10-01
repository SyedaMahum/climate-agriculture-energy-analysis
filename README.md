# Data Analytics and Visualization --- India Climate, Agriculture & Energy

## Project Overview

This project explores relationships between **temperature, agricultural
crop production, and energy trends in India** using Tableau. The
analysis combines Berkeley Earth global land temperatures by major city
with two India-focused datasets: agriculture crop production and energy
scenarios.


## Objectives

-   Explore how temperature trends relate to crop production and yield.
-   Compare agricultural production across cities, states, crops,
    seasons, and years.
-   Examine energy consumption and electricity generation in relation to
    temperature.
-   Explore city-level CO₂ emissions, energy consumption, weather
    categories, and clean cooking technologies.
-   Present findings through Tableau visualizations and dashboards.

## Datasets

The analysis uses three datasets:

1.  **Berkeley Earth --- Global Land Temperatures by Major City**\
    Used as the base dataset.
2.  **India Agriculture Crop Production**\
    Kaggle:
    https://www.kaggle.com/datasets/pyatakov/india-agriculture-crop-production\
    The report identifies `output.csv` inside the downloaded ZIP.
3.  **Complete Energy Profile of India (1965--2019)**\
    Kaggle:
    https://www.kaggle.com/datasets/shubamsumbria/complete-energy-profile-of-india-1965-2019\
    The report identifies `output2.csv` inside the downloaded ZIP.

The agriculture and energy datasets were joined to the temperature
dataset using year and city/country fields, as applicable.

## Data Preparation

The report describes the following preprocessing steps:

-   Removed missing (`NaN`/`NULL`) values from each dataset.
-   Corrected column data types where needed.
-   Filtered the temperature dataset to **India** and the years
    **2003--2013** before joining.
-   Standardized city-name capitalization so that join keys matched
    across datasets.
-   Prepared the joined datasets in Tableau Prep and loaded them into
    Tableau Desktop for visualization.

## Dashboards and Visualizations

### 1. Temperature and Agriculture

The agriculture analysis includes these visualizations:

-   Annual yield and temperature change
-   Crop production trends by city and year
-   City crop production per area
-   Crop growth analysis by temperature
-   Annual crop production growth by city
-   State crop production per area
-   Top crop-producing state by year
-   Seasonal crop production over time (Whole Year, Rabi, Kharif, and
    Summer)
-   Production versus yield over the years
-   Temperature trends and uncertainty

The report groups the first five visualizations into one dashboard and
the next five into another.

### 2. Temperature and Energy

The energy analysis includes these visualizations:

-   Energy consumption (EJ) in relation to temperature
-   Electricity in relation to temperature
-   Total consumption in relation to temperature
-   Electricity generation per temperature compared with total
    electricity generation
-   Annual primary energy consumption and temperature uncertainty
-   City-level CO₂ emissions by weather category
-   Electricity generation by city and weather
-   Per-capita energy consumption by city and weather
-   Annual weather categories across cities
-   Clean cooking fuels and technologies by city and temperature

The report groups the first five visualizations into one dashboard and
the next five into another.

## Key Questions Explored

-   How do temperature changes and variability coincide with changes in
    crop production and yield?
-   How does crop production differ by city, state, crop, season, and
    year?
-   How do energy consumption and electricity-related measures vary
    alongside temperature?
-   How do weather categories relate to city-level emissions,
    electricity generation, and per-capita energy consumption?
-   How does the adoption of clean cooking fuels and technologies vary
    across cities and temperature conditions?

## Tools and Technologies

-   **Tableau Desktop** --- visualizations and dashboards
-   **Tableau Prep** --- data preparation and joining
-   **Kaggle** --- agriculture and energy datasets

## Repository Structure

A suggested structure for this GitHub repository is:

``` text
.
├── README.md
├── your_tableau_workbook.twb
├── data/
│   ├── output.csv
│   └── output2.csv
└── screenshots/
    └── dashboard.png
```


## Viewing the Project

A `.twb` file stores workbook definitions and usually references
external data files. To make the project easier to open:

-   Include the required data files if you are permitted to share them,
    or explain where to obtain them.
-   Alternatively, save a packaged Tableau workbook (`.twbx`) with the
    supporting files.
-   Add screenshots of the dashboards to the `screenshots/` folder.
-   If the workbook is published on Tableau Public, add its URL here.

**Tableau Public link:** *Add link if available.*

## Notes and Limitations

This project explores relationships and patterns in the selected
datasets. Observed associations do not, by themselves, establish that
temperature caused a change in crop production, energy use, or
emissions. Findings are also limited by the selected datasets, the join
fields, and the 2003--2013 India temperature filter described in the
report.


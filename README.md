# Flight Data EDA

This repository contains a data analysis and visualization project exploring flight data, including flight distances, wind speed, turbulence, departure and arrival airports, and seasonal trends.

## Overview

The project performs exploratory data analysis (EDA) on flight datasets to understand patterns in:

- Flight distances
- Wind speed variations
- Turbulence levels
- Departure and arrival airport frequency
- Seasonal trends in flight activity
- Time-of-day patterns (morning, afternoon, evening, night)
- Weekday vs. hour correlations

Visualizations include:

- Histograms of flight counts by hour
- Count plots of flights by weekday
- Boxplots of wind speed and distance by turbulence level
- Heatmaps showing total flights by weekday, hour, and time of day, split by season
- Bar plots of average wind speed per season and average distance per weekday/season
- Top 10 departure and arrival airports mapped geographically with circle size and color indicating flight counts

## Data

### Importing Data from Kaggle and Other Sources

1. **Weather Observations in Aviation Industry**  
   Source: [Kaggle Flight Data](https://www.kaggle.com/datasets/aadharshviswanath/flight-data)

2. **Global Airport Database**  
   For airport names and coordinates  
   Source: [Partow Airport Database](https://www.partow.net/miscellaneous/airportdatabase/)

> **Note:** All measurements in the datasets have been converted to the United States Customary system:
> - Wind speed in miles per hour (mph)  
> - Visibility in miles  
> - Temperature in Fahrenheit  
> - Distance in miles  

### Columns in the Dataset

| Column | Description |
|--------|-------------|
| Flight_ID | Unique flight identifier |
| Date | Date of the flight |
| Time | Scheduled departure time |
| Departure_Airport | Departure airport code |
| Arrival_Airport | Arrival airport code |
| Datetime | Combined date and time |
| Hour | Hour of the flight |
| Weekday_numeric | Numeric day of the week |
| Wind_Speed_knotstomph | Wind speed in mph |
| Visibility_km_tomile | Visibility in miles |
| Temperature_Celsius_toFahrenheit | Temperature in Fahrenheit |
| Season | Season of the flight (0=Winter, 1=Spring, 2=Summer, 3=Fall) |
| Turbulence_LeveltoNumerical | Turbulence level converted to numeric |
| Depart_Latitude / Depart_Longitude | Departure airport coordinates |
| Arrive_Latitude / Arrive_Longitude | Arrival airport coordinates |
| Distance_mile | Flight distance in miles |

## Key Insights

- Flight activity peaks in the morning and night.  
- Average wind speeds and distances per season show minor variations.  
- Top 10 airports account for the majority of flights.  
- Heatmaps reveal weekday-hour patterns and seasonal trends.  

## Usage

1. Clone the repository:
```bash
git clone https://github.com/tiakorre/EDA_Flight_Data.git
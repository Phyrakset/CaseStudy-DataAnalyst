# Analyst Grap Diver

This repository contains the analysis and visualization of a dataset related to a transportation booking system. The analysis aims to understand various factors impacting driver behavior, booking patterns, and booking cancellations.

## Table of Contents

- [Installation](#installation)
- [Overview of Dataset](#overview-of-dataset)
- [Key Statistics](#key-statistics)
- [Factors Impacting Number of Ignored Drivers](#factors-impacting-number-of-ignored-drivers)
- [Factors Leading to Booking Cancellations](#factors-leading-to-booking-cancellations)
- [Recommendations](#recommendations)
- [Contributing](#contributing)
- [License](#license)

## Installation

To run the analysis, you need to have the following packages installed:

```sh
pip install pandas
pip install matplotlib
pip install seaborn
pip install openpyxl

## Overview of Dataset

The dataset contains the following columns:

- nhour_local
- pickup_area
- dropoff_area
- booking_state
- driver_incentive_khr
- ntrip_distance_km
- trip_time_mins
- eta_mins
- ignored_drivers

## Loading the Dataset

```sh
import pandas as pd

df = pd.read_excel('Copy of casestudy_dataset_mkpbi_analyst.xlsx')
```

# Key Statistics

The dataset provides insights into various metrics related to the transportation booking system. Below are the key statistics derived from the dataset:

- **Total Bookings:** 9894
- **Average Trip Distance:** 3.61 km
- **Average Trip Time:** 12.35 mins
- **Average Driver Incentive:** 578.18 KHR
- **Average ETA:** 2.05 mins
- **Average Ignored Drivers:** 4.55

### Detailed Descriptive Statistics

| Metric                  | Count | Mean   | Std Dev  | Min   | 25%     | 50%    | 75%     | Max   |
|-------------------------|-------|--------|----------|-------|---------|--------|---------|-------|
| **hour_local**          | 9894  | 16.684 | 1.037    | 15.00 | 16.00   | 17.00  | 18.00   | 18.00 |
| **driver_incentive_khr**| 9894  | 578.184| 233.306  | 300.00| 400.00  | 510.00 | 710.00  | 2410.00|
| **trip_distance_km**    | 9894  | 3.612  | 2.088    | 1.00  | 1.96    | 3.05   | 4.78    | 9.998 |
| **trip_time_mins**      | 9894  | 12.345 | 6.790    | 3.07  | 6.98    | 10.60  | 16.17   | 36.00 |
| **eta_mins**            | 9894  | 2.049  | 1.763    | 0.00  | 0.68    | 1.53   | 2.93    | 9.37  |
| **ignored_drivers**     | 9894  | 4.546  | 0.617    | 0.00  | 4.00    | 5.00   | 5.00    | 6.00  |

### Summary

This dataset provides a comprehensive view of the booking system, including how often drivers ignore bookings, the incentives provided to drivers, and the typical trip characteristics. Such insights can be crucial for optimizing the booking process and improving overall efficiency.

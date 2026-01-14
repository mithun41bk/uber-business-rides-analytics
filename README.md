# uber-business-rides-analytics
 Data science project analyzing 2016 Uber ride logs with end‑to‑end workflow: data loading, cleaning, feature engineering (date, time, day‑night, round trips, weekdays, ride durations), exploratory data analysis, and business insights. The notebook explores ride demand by time of day and weekday, monthly miles......
Report Structure:

 Uber Rides EDA – Practice Project
This repository contains a practice data analysis project on Uber ride data using Pandas, NumPy, and Matplotlib/Seaborn. It focuses on data cleaning, feature engineering, exploratory data analysis (EDA), and visualization to build hands‑on skills, not on production‑level modeling or deployment.
​

Project Overview
Dataset: 2016 Uber ride logs with columns such as start and end datetime, category (business/personal), start and stop locations, miles, and trip purpose.
​

Goal: Practice cleaning real‑world style data, create useful time‑based features, and understand ride patterns through EDA and plots.
​

Scope: Only analysis and visualizations (no advanced machine learning models).

Objectives
Practice loading and inspecting tabular data.

Handle missing and inconsistent values (e.g., “not”, NaN in purpose, totals row, odd characters in locations).
​

Engineer time features (date, hour, part of day, month, weekday, round trip flag, trip duration).
​

Visualize key patterns in ride usage: when, where, how far, and for what purpose.
​

Technologies Used
Language: Python 3

Core Libraries:

pandas – data loading, cleaning, feature engineering, grouping.
​

numpy – basic numerical operations and support.
​

matplotlib.pyplot – base plotting.
​

seaborn – statistical visualizations (count plots, box plots, etc.).
​

Data Cleaning & Feature Engineering
Main steps performed in the notebook:
​

Removed or fixed non‑data rows like the final “Totals” row.
​

Converted START_DATE and END_DATE to proper datetime types.
​

Created new columns:

date (date part of start time).
​

time (hour of day as numeric).
​

day-night (morning/afternoon/evening/night label).
​

ROUNDTRIP (yes/no if start and stop locations are same).
​

MONTHS (month name abbreviation).
​

MINUTES (trip duration as END_DATE - START_DATE).
​

WEEKDAYS (weekday name).
​

Exploratory Data Analysis (EDA)
The notebook runs several EDA steps to understand the data:
​

Descriptive statistics

describe() for numeric columns like MILES and derived time/duration.
​

Value counts for categorical columns (CATEGORY, PURPOSE, START, STOP, WEEKDAYS, MONTHS).
​

Univariate analysis

Distribution of miles per trip.

Frequency of business vs personal trips.
​

Most common purposes (meeting, customer visit, errand/supplies, etc.).
​

Time‑based analysis

Trips by hour and day-night bucket (morning/afternoon/evening/night).
​

Trips by weekday (WEEKDAYS).
​

Trips and miles by month (MONTHS).
​

Derived insights practice

Which times of day have more rides.

Which weekdays are busier.

Typical miles and durations by purpose or category.
​

Visualizations
Example plots included in the notebook:
​

Count plots for:

CATEGORY (business vs personal).

day-night vs MILES using boxplots to see distance distribution across time of day.
​

MONTHS to see monthly ride frequency.
​

Other possible plots:

Rides by weekday.

Miles by purpose (bar plots).

Duration (MINUTES) distributions.

All plots are generated using Matplotlib and Seaborn for quick visual inspection and practice.
​

 

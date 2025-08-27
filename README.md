🚖 Uber Trips Analysis (September 2014)
Overview

This project looks at Uber pickup data for New York City in September 2014.
The goal was to understand demand patterns, visualize rider behavior, and test if pickup locations could help predict trip timing.

Tools & Libraries

Python (pandas, numpy) for data wrangling

matplotlib, seaborn, and plotly for charts and visuals

scikit-learn for the machine learning model

Dataset

The dataset includes pickup records with:

date/time – timestamp of the ride

lat, lon – pickup coordinates

base – base company code

Engineered features: day, weekday, hour

Analysis Workflow

Data Prep

Converted timestamps to datetime

Extracted day, weekday, and hour for richer analysis

Exploratory Analysis

Daily ride counts and weekday patterns

Hourly demand spikes

Pickup hotspots mapped on NYC

Modeling

Random Forest Classifier to predict the pickup hour from location

Accuracy ~35% (showing that location alone doesn’t strongly determine pickup time)

Findings

Rides spike in the evening rush hours (5–8 PM).

Fridays and Saturdays are consistently the busiest.

Central Manhattan and JFK are clear hotspots.

Basic models struggle to predict pickup hour just from location data — additional context (like weather or events) would help.

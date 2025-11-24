# Connecticut Traffic Stops Analysis

## Project Overview
Analyzed nearly 270,000 traffic stops conducted by the Connecticut State Police (Oct 2013 – Mar 2015) to explore factors influencing stop outcomes and whether searches were conducted. The project involved data cleaning, transformation, exploratory analysis, and logistic regression modeling to predict contraband found and other stop outcomes.

## Key Steps
1. **Data Cleaning & Transformation**
   - Removed irrelevant/duplicate columns and handled missing values.
   - Recoded `search_type` NAs as "No Search".
   - Dropped minor fraction of rows with missing critical values (<1.7% of total).
   - Created new variables for stop time intervals and stop month categories.
   - Log-transformed `driver_age` to reduce skew.

2. **Exploratory Data Analysis**
   - Visualized relationships between predictors and outcomes using boxplots, histograms, KDE plots, and stacked bar plots.
   - Analyzed factors like search type, contraband found, and time of stop to understand their impact on stop outcomes.

3. **Modeling**
   - Built logistic regression models to predict whether contraband was found based on driver demographics, search type, and other variables.
   - Selected optimal thresholds and evaluated model performance on a test set.

## Tools & Technologies
- R (tidyverse, ggplot2, lubridate, dplyr, patchwork, inspectdf)  
- R Markdown → HTML report  
- GitHub Pages for hosting final report  

## View Report
Full HTML report with visualizations and results is available online:  
https://evapeters2.github.io/Traffic-Stops-Model/Project1.html 

## Repository Structure
- `CT_stops.csv` — Raw dataset  
- `analysis.R` — R script for cleaning and modeling  
- `analysis.Rmd` — R Markdown file for generating the HTML report  
- `docs/` — Contains final HTML report

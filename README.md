# Week2
This project aims to analyze country-specific data and develop predictive models to estimate CO2 emissions.The dataset comprises data from 1990 to 2011, covering countries worldwide. It includes a wide variety of features such as population statistics, economic indicators, land use, energy consumption, and more.

# Dataset Summary
Years: 1990 to 2011 Countries: Global coverage

Features: Greenhouse gas emissions (CO2, CH4, N2O) Population data (total, urban, growth) Economic indicators (GDP, GNI, FDI) Agricultural and land parameters Energy usage Climate statistics (precipitation, disasters) Health indicators (medical staff counts)


# Stage 1: Data Cleaning and Preparation
Import and overview of raw data
Handling missing values
Feature renaming and formatting
Conversion to numerical types
Melting and transforming datasets
Final clean dataset exported as data_cleaned.csv

# Stage 2 : Data exploration and visualization
Explored how various socio-economic, environmental, and energy-related factors influence CO₂ emissions, and prepared the data for predictive modeling.

## Notebook Highlights
#### 1. Setup and Data Import
Imported cleaned dataset data_cleaned.csv
Loaded essential libraries: pandas, numpy, matplotlib, seaborn, statsmodels

### 2. Global Data Overview
Dataset shape: (1700, 18)
Column summaries, data types, and initial descriptive statistics


### 3. Hypothesis
CO₂ emissions are influenced by factors such as energy use, population metrics, GDP, and land use — and can be predicted using them.

### 4.Feature Engineering
Derived en_ttl (Total Energy Use)
Correlation matrix to evaluate feature relationships
Multicollinearity check using VIF (Variance Inflation Factor)

### 5. Visualizations
Line plot: Global average CO₂ emissions per capita (1991–2008)
Scatter plot: CO₂ emissions vs population
Pair plots: Visualizing dependencies across selected countries
4D plot: Relationship between urb_pop_growth_perc, co2_per_cap, en_per_cap, and pop_urb_aggl_perc

### 6.Outlier Analysis
Detected outliers (e.g., United Arab Emirates with 25–40 t/capita)
Removed extreme outliers to improve clarity of plots

## Key Insights
Strong linear relationship: co2_per_cap and en_per_cap
Nonlinear patterns: with variables like gni_per_cap, urban population growth
Country-specific clusters influence emission trends
Outliers like UAE deviate heavily from global norms
Population count showed low relevance and was dropped

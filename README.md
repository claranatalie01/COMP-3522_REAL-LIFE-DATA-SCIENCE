# Analyzing Public Transportation Fare Discrepancies in Hong Kong

## Project Title
Analyzing Public Transportation Fare Discrepancies in Hong Kong

## Group Information
- **Group Number**: A1
- **Group Members**:
  - Lie Warren Leander (3036094306)
  - Winiera Sutanto (3035964671)
  - Huang Da Fang (3036052205)
  - Clara Natalie Surjadjajadi (3036029686)

## Table of Contents
1. [Objective](#objective)
2. [Project Highlights](#project-highlights)
3. [Background](#background)
4. [Methodology](#methodology)
   - [Project Focus and Approach](#project-focus-and-approach)
   - [Conceptual Framework](#conceptual-framework)
   - [Initial Methodological Approach](#initial-methodological-approach)
   - [Methodological Evolution](#methodological-evolution)
   - [Definition of "Unreasonably Expensive"]( #definition-of-unreasonably-expensive)
5. [Bus Dataset](#bus-dataset)
   - [Data Acquisition](#data-acquisition)
   - [Data Cleaning](#data-cleaning)
   - [Exploratory Data Analysis](#exploratory-data-analysis)
   - [Model and Evaluation](#model-and-evaluation)
   - [Interpretations and Communications](#interpretations-and-communications)
6. [MTR Dataset](#mtr-dataset)
   - [Data Acquisition](#data-acquisition-1)
   - [Data Cleaning](#data-cleaning-1)
   - [Exploratory Data Analysis](#exploratory-data-analysis-1)
   - [Data Modelling and Evaluation](#data-modelling-and-evaluation)
   - [Interpretations and Communications](#interpretations-and-communications-1)
7. [Downloads](#downloads)

## Objective
The primary objective of this data science project is to analyze public transportation costs across Hong Kong districts, focusing on bus and MTR fares. The project aims to determine whether claims of "unreasonably expensive" transportation in certain areas are supported by data. Specifically, the project aims to:

1. Conduct a comprehensive analysis of bus and MTR fare structures across Hong Kong's 18 districts to identify patterns, disparities, and potential inequities.
2. Develop robust predictive models capturing factors influencing public transportation fares, including distance, geographic location, service providers, and route characteristics.
3. Establish a data-driven methodology to objectively compare transportation costs between different areas of Hong Kong, accounting for socioeconomic factors like population density and median income.
4. Identify districts with potentially "unreasonably expensive" public transportation by establishing statistical thresholds and evaluating outliers against model predictions.
5. Provide evidence-based insights to inform public discourse on transportation equity and accessibility in Hong Kong.

## Project Highlights
- **Identified Key Fare Determinants**: Advanced modeling techniques (XGBoost, Random Forest) revealed that MTR fares are primarily influenced by travel distance (R² = 0.96), while bus fares are significantly affected by specific route groups and journey distance (R² = 0.88).
- **Discovered Geographic Disparities**: Analysis identified Tuen Mun and Yuen Long as having the highest percentages of "unreasonably expensive" bus routes (21.0% and 18.5% respectively).
- **Methodological Innovation**: Improved model accuracy by transitioning from average fare per kilometer metrics to raw fare analysis, increasing explanatory power from approximately 30% to over 88% (R²).

## Background
Public transportation is crucial for Hong Kong, facilitating millions of journeys daily. Despite its efficiency, there are ongoing concerns regarding fare equity and affordability across different geographical regions.

## Methodology

### Project Focus and Approach
This research employs a comprehensive, multi-modal approach to investigate public transportation costs, focusing on bus and MTR fare structures. The central research questions include:
1. What factors significantly influence public transportation fares in Hong Kong?
2. Do certain districts bear disproportionately higher transportation costs?
3. Can objective criteria be established to identify "unreasonably expensive" transportation in specific areas?

### Conceptual Framework
The analysis incorporates multiple variables affecting fare structures, recognizing the complexity of transportation costs.

### Initial Methodological Approach
The initial focus on average fares per kilometer revealed limitations and led to a methodological pivot.

### Methodological Evolution
Transitioning to raw fare analysis allowed for a more accurate representation of fare pricing dynamics, enhancing model predictive power and insights.

### Definition of "Unreasonably Expensive"
A statistical outlier approach was established, defining unreasonable expenses as those exceeding 1.5 times the interquartile range (IQR) above the upper quartile. This method allows for a robust identification of fare anomalies.

## Bus Dataset

### Data Acquisition
The primary dataset includes bus stops, routes, and fares sourced from [DATA.GOV.HK](https://data.gov.hk/en-data/dataset/hk-td-tis_3-routes-and-fares-of-public-transport/resource/707cdb6b-e45c-4e76-aca6-b1622672dd73).

### Data Cleaning
Data cleaning involved type conversions, string manipulations, and handling of NA values.

### Exploratory Data Analysis
EDA revealed strong correlations between transportation prices and distances traveled, along with geographic disparities.

### Model and Evaluation
Multiple models (OLS Regression, Random Forest, XGBoost) were used to analyze fare structures, with key insights regarding fare determinants.

### Interpretations and Communications
Insights emphasized specific route groups and journey distances as significant factors influencing bus fares.

## MTR Dataset

### Data Acquisition
The MTR dataset was obtained from the government database, focusing on station names and fares.

### Data Cleaning
Cleaning involved retaining key columns, labeling districts, and calculating distances using geodetic methods.

### Exploratory Data Analysis
EDA confirmed correlations between MTR fares and distances, highlighting outlier stations.

### Data Modelling and Evaluation
Various regression models were tested, with XGBoost selected for its superior predictive accuracy.

### Interpretations and Communications
Distance was identified as the primary factor influencing MTR fares, with specific districts showing higher rates of "unreasonably expensive" routes.

## Downloads
- The detailed project report can be downloaded [here](https://github.com/claranatalie01/COMP-3522_REAL-LIFE-DATA-SCIENCE/blob/main/COMP3522%20Final%20Report.docx).
- The code, dataset, and a video of code explanation can be downloaded [here](https://github.com/claranatalie01/COMP-3522_REAL-LIFE-DATA-SCIENCE/blob/main/COMP%203522_VIDEO%2BCODE.zip).

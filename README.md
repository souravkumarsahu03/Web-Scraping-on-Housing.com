# 🏡 Hyper-Local Rental Arbitrage Detector (Housing Data Web Scraping)

### Project Overview

This project focuses on leveraging Web Scraping and Exploratory Data Analysis (EDA) to create a proprietary dataset of rental properties. The primary business goal is to identify and analyze supply concentration, pricing trends, and key property attributes to pinpoint high-potential neighborhoods for rental arbitrage (profiting from the difference between long-term rent and potential short-term rental revenue).

### Key Project Stages

* Data Collection: Automated extraction of 1,500+ property records.

* Data Cleaning: Normalization of key features like price, area, and configuration.

* Analysis & Visualization (EDA): Identifying market saturation, price anomalies, and demand indicators.


<img width="990" height="397" alt="image" src="https://github.com/user-attachments/assets/9754c8e1-7fc1-4e38-a8ea-6a49b822a86e" />


### 📈 Data Pipeline & Analysis Breakdown

The project follows a standard data science workflow, ensuring reliability and quality at every step:

1. Data Collection (Web Scraping)

> Target: Rental listings from a static housing portal (similar to Housing.com).

> Method: A Python script was developed to iterate through multiple search pages, handle headers and delays, and extract core features from each property card, including BHK configuration, Price, Area (SqFt), Furnishing Status, and Locality.

> Result: A raw dataset containing over 1,500 rows of current rental market information.

2. Data Cleaning & Transformation

Raw web-scraped data is often noisy and inconsistent. Key cleaning steps included:
*Price Normalization: Converting Indian financial units (e.g., "Lac" or "Cr") into a single numerical format (e.g., INR) for uniform analysis.
* Feature Extraction: Separating the numerical area value from its unit (SqFt/SqMtr) and ensuring uniform measurement units.
* Handling Missing Values: Imputing or dropping columns with high null percentages to maintain data integrity.

3. Exploratory Data Analysis (EDA) & Insights
The cleaned data was subjected to EDA to uncover market trends.
* Supply Concentration: Analyzed the Distribution of BHK Types, confirming the 3 BHK configuration as the most saturated segment, which indicates high competition.
* Price Anomalies: Used statistical methods (describe(), box plots) to identify outliers and understand the typical price distribution across key localities.
* Furnishing Segmentation: Visualized the Furnishing Status to confirm that Semi-Furnished units (approx. 70%) are the market standard, highlighting the investment gap needed to convert these to premium Fully-Furnished units for short-term rental strategies.

Result: Identified the top 5 localities showing a favorable supply/demand imbalance for immediate investment focus.

### 📊 Key Visualizations & Output

* The final analysis delivered clear, actionable visualizations:
* BHK Distribution Bar Chart: Showcasing market supply concentration.
* Price-Locality Heatmap: Illustrating average rental prices across different neighborhoods.

Furnishing Status Pie Chart: Highlighting the dominance of Semi-Furnished listings.

### 🚀 How to Run the Project

<img width="983" height="649" alt="image" src="https://github.com/user-attachments/assets/863f0372-8471-40d0-8c69-87405fe04613" />


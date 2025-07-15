# Eda-project_Muhammad_Saad_cohort5
# Real Estate Market Insights: Zameen.com EDA Project

This project explores real estate listings from [Zameen.com](https://www.zameen.com/) using data analysis and visualization techniques. The goal is to extract actionable insights — such as pricing trends, property sizes, and city-wise comparisons — to help investors and analysts make more informed decisions.

---

## Project Objective

To conduct exploratory data analysis (EDA) on Pakistan's real estate market using property listings from Zameen.com. We aim to uncover:

- Median property prices by city
- Price per square foot distribution
- Listings trends by area, type, and bedroom count
- Top cities for real estate investment
- Outlier detection and data consistency

---

##Dataset Description

The dataset includes the following fields:

- `Title`: Property title  
- `City`: City name (e.g., Lahore, Karachi)  
- `Type`: Property type (House, Plot, Flat, etc.)  
- `Area`: Area in local units (Kanal, Marla, Sq. Ft.)  
- `Price`: Price listed in PKR  
- `Purpose`: Buy / Rent  
- `Location`: Area within city  
- `Description`: Textual description  
- `Bedrooms` and `Bathrooms`: Number of rooms  

---

## Tools & Libraries

- Python  
- Pandas & NumPy  
- Matplotlib & Seaborn  
- Jupyter Notebook / Google Colab  

---

##  Analysis Sections

### 1.  Data Cleaning & Preprocessing
- Removed commas, symbols (e.g., PKR), and converted `Price` and `Area` to numerical values.
- Standardized all area values to square feet.
- Dropped listings with missing key fields like price or area.
- Created new columns such as `Price_Clean`, `Area_Sqft`, and `Price_per_Sqft`.

---

### 2.  Univariate Analysis
Analyzing single features to understand their distribution and patterns:

- **Property Prices:** Histogram with KDE showing skewed price distribution (most properties priced in the lower-mid range).
- **Property Areas:** Most properties are below 5,000 sqft — large plots are rare.
- **Top 10 Cities by Listings:** Lahore, Karachi, and Islamabad dominate listings volume.
- **Property Types:** Plots are listed more frequently than houses or flats.
- **Bedrooms & Bathrooms:** Most listings are 3-bedroom with 2–3 bathrooms, indicating mid-size family homes are common.

---

### 3.  Bivariate Analysis
Studying relationships between two variables to uncover trends:

- **Price per Sqft vs Property Type:** Flats and houses have higher price/sqft than plots.
- **Price Distribution by City:** Islamabad and Lahore have higher median prices than other cities.
- **Bedrooms vs Price:** Price increases with more bedrooms, though with wide variability.
- **Area vs Price (Scatter Plot):** Positive correlation, but some expensive listings have small area (e.g., luxury flats).
- **Correlation Heatmap:** 
  - `Area_Sqft` and `Price_Clean` are positively correlated.
  - Bedrooms and bathrooms moderately correlate with price.
  - `Price_per_Sqft` is negatively correlated with `Area_Sqft` (larger properties tend to be cheaper per sqft).

---

## Key Insights

- **Islamabad, Lahore, and Karachi** have the highest median property prices.
- **Plots** are the most frequently listed property type.
- Most listings are for **3-bedroom homes** with **2–3 bathrooms**.
- Price per square foot varies widely across cities — offering opportunities for both luxury and budget investments.
- Larger homes generally cost more, but **luxury flats** may have higher prices with smaller footprints.

---



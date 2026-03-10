# Exploratory Data Analysis on Zameen Properties (2025)

## Objective
Analyze property listings from Zameen.com to uncover market trends, pricing patterns, and location-based insights.

## The Problem
Raw property data contained duplicates, missing values, and complex string formats (e.g., "PKR\n4.75 Crore"). This made it difficult to extract reliable pricing and area insights.

## The Solution
- Imported only relevant columns: Price, Area, Bedrooms, Bathrooms, City, Purpose.
- Removed 16,431 duplicate rows, reducing dataset to 1,824 unique entries.
- Cleaned `Area` (converted "Sq. Yd." to numeric) and `Price` (parsed PKR, Crore, Lac).
- Converted Bedrooms/Bathrooms to numeric and imputed missing values (median for numeric, mode for categorical).
- Visualized:
  - **Violin plots** of price distribution by city.
  - **Scatter plots** of Price vs. Area.
  - **Correlation heatmap** of numerical features.

## The Impact
- Delivered a clean dataset with **zero missing values** and consistent numeric formats.
- Identified **median property price ~ PKR 31,000,000** and area median ~ 217 sq. yd.
- Highlighted city-level pricing trends and correlations between property size and price.
- Created a reusable framework for real estate analytics and predictive modeling.

## Deliverables
- [EDA Jupyter Notebook](https://github.com/sarahafreenmalik/EDA-Portfolio/blob/main/EDA_Portfolio.ipynb)
- Visualizations: violin

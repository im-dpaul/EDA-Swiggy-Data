# Swiggy Insights: Restaurant Data Analysis

This project conducts an exploratory data analysis (EDA) on Swiggy's sales data, focusing on restaurant ratings, cost distribution, and popular cuisines. Utilizing pandas and numpy, the analysis uncovers key insights about the dining trends across different cities, helping inform data-driven decisions for Swiggy and restaurant owners.

### About Data:

- Dataset: [Swiggy Data](https://drive.google.com/file/d/1xtUucJirZ50D7JP7GftRoMcWAECkbWfW/view?usp=sharing)
- The dataset contains information about various restaurants listed on Swiggy. The informations includes **id**, **name**, **rating**, **cost**, **cuisine** etc.

### Table of Contents:

1. [Importing Libraries](#importing-libraries)
2. [Data Exploration](#data-exploration)
3. [Data Preprocessing](#data-preprocessing)
4. [Exploratory Data Analysis](#exploratory-data-analysis)
5. [Conclusion](#conclusion)

## Importing Libraries

**Importing required libraries:**
- `pandas` for data manipulation.
- `numpy` for numerical operations.

## Data Exploration

 - Loads a Swiggy dataset containing restaurant information (ID, name, city, rating, rating count, cost, cuisine, license number, link, address).
 - Provides a data dictionary for understanding each feature.
 - Analyzes basic statistics using head(), tail(), and info() methods.

## Data Preprocessing

- Handles missing values:
  - Removes rows with any missing values.
  - Fills missing "rating" values with -999.0 (alternative: median imputation).
- Converts "cost" feature from string to numeric format by removing the rupee symbol.
- Deals with the categorical count in "rating_count" (optional: Label Encoding).

## Exploratory Data Analysis

- **Restaurant Distribution:**
   - Determines the number of cities served by Swiggy.
   - Counts the total number of restaurants and unique restaurant names.
   - Identifies the most popular food chains based on name frequency.
      
- **Customer Reviews:**
   - Analyzes the overall rating distribution of restaurants.
   - Visualizes the percentage of ratings for different rating categories.
      
- **City Performance:**
   - Discovers the city with the highest number of restaurants.
   - Explores the city with the highest average rating (considering reliable rating counts).
      
- **Cost Analysis:**
   - Examines the cost distribution of restaurants through visualizations.
   - Explores the most expensive restaurants based on cost.
      
- **Cuisine Popularity:**
   - Identifies the most common cuisine types among highly-rated restaurants (rating > 3.5).
   - Utilizes list comprehension and string manipulation to analyze cuisine data.

## Conclusion
The analysis provides a comprehensive overview of Swiggy's restaurant data, including insights into ratings, cost, and popular cuisines. This can help Swiggy and restaurant owners to make data-driven decisions.

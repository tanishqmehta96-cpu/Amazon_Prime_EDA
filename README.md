# Amazon Prime TV-Shows and Movies EDA

## Project Summary

This project performs exploratory data analysis (EDA) on the Amazon Prime Video dataset. The analysis focuses on understanding the content catalog of TV shows and movies available on the platform. It uncovers trends, insights, and patterns related to content type, genre distribution, ratings, release years, and regional availability.

## Problem Statement

This dataset helps to analyze all shows available on Amazon Prime Video, allowing us to extract valuable insights such as:

**Content Diversity:** Understanding the dominant genres and categories on Amazon Prime is crucial for strategic content planning. 

**Trends Over Time:** The entertainment landscape evolves constantly. Analyzing how Amazon Prime's content library has changed to adapt to viewer preferences and market trends is important.

**IMDb Ratings & Popularity:** IMDb ratings and popularity scores offer valuable insights into viewer engagement and satisfaction. Analyzing these metrics to identify high-performing content and potential areas for improvement is needed.

## Data Wrangling

The manipulations performed on given data are as follows:

1.  **Data Loading and Merging:** Two datasets, `titles.csv` and `credits.csv`, were loaded and merged based on the common column `id`.
2.  **Handling Missing Values:**
    -   Null values in the `description` and `imdb_id` columns were dropped.
    -   Null values in `age_certification` were replaced with the mode.
    -   Null values in `seasons`, `imdb_votes`, and `character` were replaced with 0, 0, and 'unknown', respectively.
    -   Null values in `imdb_score`, `tmdb_popularity`, and `tmdb_score` were replaced with their respective means.
3.  **Handling Duplicates:** Duplicate rows identified and removed from the dataset.

## Data Visualization

The project utilizes various visualization techniques to gain insights from the data:

- **Univariate Analysis:** Box plots, histograms, and bar plots were used to explore individual variables like `imdb_score`, `runtime`, `release_year`, and `genres`.
- **Bivariate Analysis:** Scatter plots and line plots were used to examine relationships between variables like `imdb_votes` and `imdb_score`, and trends over time.
- **Multivariate Analysis:** Pair plots and heatmaps were used to visualize relationships between multiple variables.

## Conclusion

This EDA has provided valuable insights into the Amazon Prime Video dataset, revealing patterns and trends in content, user preferences, and platform strategies. The findings can be used by content creators, platform strategists, and viewers to make informed decisions and understand the dynamics of the streaming landscape.

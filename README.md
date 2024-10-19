# Analyzing Genre Influence on IMDb Ratings for Film and TV 

## Table of Contents

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Data Cleaning and Preparation](#data-cleaning-and-preparation)
- [Analysis Methods](#analysis-methods)
- [Key Findings](#key-findings)
- [Recommendations](#recommendations)
- [References](#references)

## Project Overview

This project uses data from the IMDb datasets to explore how film genres influence IMDb ratings. The goal is to provide insights into which genres are most frequently associated with high-rated films and TV shows on IMDb. This analysis is designed for a streaming service or film studio seeking to optimize project selection by investing in genres with a higher likelihood of critical success.

**This overview provides summaries for each project stage. To view the full analysis steps, download the PDF version of imdb_analysis. To replicate the analysis yourself, download the imdb_analysisv01.Rmd project file from this repository and the datasets from the IMDB Non-Commerical linked in References.**

### Skills
- Data cleaning
- Exploratory data analysis
- Data filtering
- Trend analysis
- Data visualization

### Tools
- Python
- Jupyter Lab

## Data Sources

The data comes from IMDb's Non-Commercial Datasets, including:
- title_basics: Title information
- title_ratings: IMDb rating and number of votes
- title_principals: Information on directors, writers, and key actors
- title_akas: Alternative title information
- title_crew: Names for crew
- title_episode: Episode and season numbers
- name_basics: Key names involved with the titles

## Data Cleaning and Preparation

I performed the following tasks:
1. Loaded data and libraries
2. Duplicated data frames for cleaning
3. Resolved null values
4. Converted data types
6. Standardized column names using snake_case
7. Checked unique categorical values
8. Standardized capitalization of string values
9. Dropped unnecessary columns
10. Split professions into multiple columns
11. Split genres into multiple columns
12. Trimmed trailing whitespaces
13. Standardized string formatting
14. Mapped unique identifiers to title and principal names
16. Merged tables
17. Removed any duplicate rows
18. Handled outliers
19. Validated numerical data
20. Saved cleaned copies as CSV files
    
## Analysis Methods

EDA: 
- Overviewed data structure and statistics.
- Identified top-rated actors and directors.
- Counted titles per genre and examined distribution with histogram.
  
Genre and Rating Analysis:
- Calculated average ratings per genre.
- Examined descriptive statistics for genre counts.
- Plotted title counts and average ratings for genres.
- Plotted genre and average rating relationship.
- Examined average ratings for multiple genre combinations.
- Identified top titles per genre.
  
Trend Analysis:
- Plotted average ratings and counts for genres to examine changes over time.
- Examined genre trends for recent years.
  
Visualizations:
- Histogram
- Bar charts
- Line charts
- Box plot
- Scatter plot

## Key Findings

- History, Documentary, and Biography (all non-fiction genres) have the highest average ratings.
- Drama, Comedy, Documentary, and Action are the most popular genres based on title counts alone. Most film and TV shows fall into the Drama or Comedy category.
- Along with the non-fiction genres, Action and Adventure have seen an increase in ratings in the past few years.
- Horror movies and Thrillers currently have the worst average ratings on IMDb.
- There are fewer titles being made in History, Documentary, and Biography genres yet they tend to have high ratings. This could suggest viewers are more interested in and appreciative of non-fiction projects, and with fewer films overall, less competition in these genres to stand out.
- Short films have seen a decrease in popularity and have an average rating lower than other genres. This suggests feature films and TV shows are more profitable now.
- Most genre combinations that have high average ratings include at least one non-fiction genre.

## Recommendations

Based on this analysis, I recommend the following actions for project selection:

- Invest in Documentary, Historical, or Biographical films to increase the likelihood of critical success.
- Invest in projects with genre combinations that bring multiple popular genres together. If one of those genres is non-fiction, it may increase critical success.
- Dramas and comedies are more common genres and generally tend to rate lower than other genres. Combining a non-fiction genre like History or Biography with genres like Comedy and Drama to create Historical Fiction pieces could be a method for ensuring higher ratings and a wider audience. Invest in films that combine successful genres in unique ways.
- Invest in feature-length films and TV shows rather than short films.

## References

1. [IMDb Non-Commerical Datasets](https://developer.imdb.com/non-commercial-datasets/)

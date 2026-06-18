# Netflix Content Analytics Dashboard

## Project Overview

This project presents an interactive Power BI dashboard built using the Netflix dataset. The dashboard provides insights into Netflix's content library, including movies, TV shows, genres, ratings, countries, and release trends.

---

## Business Problem

Streaming platforms generate vast amounts of content-related data. Understanding content distribution and audience preferences is essential for strategic decision-making.

This dashboard helps analyze Netflix's catalog and identify trends across different categories.

---

## Objectives

- Analyze Movies vs TV Shows distribution
- Identify popular content ratings
- Explore genre distribution
- Analyze content by country
- Track content release trends over time
- Understand Netflix content growth

---

## Dataset Information

Dataset: Netflix Titles Dataset

Key Columns:

- Show ID
- Type
- Title
- Director
- Cast
- Country
- Date Added
- Release Year
- Rating
- Duration
- Listed In (Genre)
- Description

---

## Data Cleaning

Performed using Power Query:

- Removed null values
- Standardized country names
- Converted date formats
- Removed duplicate records
- Split genre fields
- Corrected data types

---

## Dashboard Features

### KPI Cards

- Total Titles
- Total Movies
- Total TV Shows
- Total Countries

### Visualizations

- Movies vs TV Shows
- Content by Rating
- Content by Country
- Top Genres
- Release Year Trend
- Content Added Over Time

### Filters

- Type
- Country
- Rating
- Release Year

---

## Data Modeling

Single-table analysis with calculated columns and DAX measures.

---

## DAX Measures

```DAX
Total Titles =
COUNTROWS(Netflix)

Movies Count =
CALCULATE(
COUNTROWS(Netflix),
Netflix[Type] = "Movie"
)

TV Shows Count =
CALCULATE(
COUNTROWS(Netflix),
Netflix[Type] = "TV Show"
)
```

---

## Dashboard Preview

### Main Dashboard

![Dashboard](https://github.com/soniyashaik29/Netflix-Movies-and-TV-Shows-Analysis/blob/main/Overview%20of%20netflix.png)

---

## Key Insights

- Movies represent the majority of Netflix content.
- TV Shows have shown significant growth in recent years.
- Drama and International Movies are among the most common genres.
- Content is distributed across multiple countries, with the United States contributing the largest share.
- Netflix content additions increased rapidly after 2015.

---

## Tools Used

- Power BI Desktop
- Power Query
- DAX
- CSV Dataset

---

## Future Enhancements

- Sentiment analysis on descriptions
- Recommendation insights
- Genre forecasting
- Interactive drill-through reports

---


GitHub: Your GitHub Profile

LinkedIn: Your LinkedIn Profile

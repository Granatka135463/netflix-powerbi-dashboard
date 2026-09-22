# Netflix Content Strategy Dashboard — Power BI

## Overview
An interactive Power BI dashboard analyzing 8,800+ Netflix titles to understand 
how the platform's content mix has evolved over time — comparing Movies vs. 
TV Shows, tracking genre trends, and identifying release-year patterns.

## Key Insight
TV Show share of Netflix's catalog has grown significantly since 2015, while 
Movies still dominate the overall count. International Movies and Dramas are 
the leading genres across the catalog.

## Dataset
- Source: Netflix Titles dataset (8,807 records)
- Fields: title, type, director, cast, country, date added, release year, 
  rating, duration, genres

## Data Cleaning (Power Query)
- Fixed date parsing errors caused by locale mismatch (English date format)
- Split multi-value fields: genres (`listed_in`) and duration (mixed 
  "min" for movies / "seasons" for TV shows) into separate usable columns
- Removed records with missing `type` values
- Trimmed whitespace inconsistencies causing duplicate category entries

## Dashboard Features
- KPI cards: total titles, Movies vs. TV Shows count
- 100% stacked bar chart: Movie/TV Show split by release year (trend over time)
- Line chart: title count by release year and type
- Top 10 genres by title count
- Interactive slicer to filter by content type

## Tools
Power BI Desktop, Power Query

## Files
- `netflix_titles.csv` — source dataset
- `Film_BI.pbix` — Power BI report file

## Author
Nataliia Vyshynska — [LinkedIn](https://www.linkedin.com/in/наталія-вишинська-3231b72b6/)

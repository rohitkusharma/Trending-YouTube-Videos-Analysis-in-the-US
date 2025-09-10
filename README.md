# YouTube Trending Video Analysis with Python and SQL

## Objective
This project analyzes trending YouTube video data to uncover insights into what makes a video successful. The primary goal was to use SQL queries within a Python environment to identify top channels, popular categories, and key engagement patterns.

## Dataset
The dataset is the [Trending YouTube Video Statistics](https://www.kaggle.com/datasets/datasnaek/youtube-new) from Kaggle, which includes data on trending videos in the USA.

## Tools and Libraries
- **Language:** Python, SQL
- **Libraries:** Pandas (for data handling), SQLite3 (for database management)
- **Environment:** Google Colab

## Analysis Process
1.  **Data Preparation:** Loaded `USvideos.csv` and `US_category_id.json` into pandas DataFrames. The JSON file was correctly parsed to create a clean category lookup table.
2.  **Database Creation:** An in-memory SQLite database was created, and the two DataFrames were loaded as SQL tables (`USvideos` and `UScategories`).
3.  **SQL Querying:** Ran SQL queries to answer key business questions directly from the database using pandas.

## Key Questions Answered
1.  **What are the most popular video categories?** The analysis showed that 'Entertainment' and 'Music' have the highest number of trending videos.
2.  **Which videos are the most *loved* by audiences?** By calculating a like-to-view ratio, we identified videos that generated the most positive engagement relative to their viewership.
3.  **Which channels are the most consistent performers?** By calculating the average likes per video, we identified channels that consistently produce highly engaging content.

## Conclusion
This project demonstrates a complete data analysis workflow, from handling raw data in different formats (CSV, JSON) to creating a relational database and using SQL to extract actionable insights. The findings can help content creators and platforms better understand the drivers of video popularity and audience engagement.

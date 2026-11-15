
# Movie Web Scraping and SQLite Data Pipeline

## Project Overview

This project demonstrates web scraping and data extraction using Python. It retrieves information about the top 50 highly ranked movies from an archived webpage and stores the extracted data in CSV and SQLite database formats.

Developed as part of the IBM Data Engineering learning program.

## Technologies Used

- Python
- Requests
- BeautifulSoup
- pandas
- SQLite
- HTML Parsing

## Project Workflow

**1. Data Extraction**
- Retrieve HTML content using HTTP GET requests.
- Parse HTML using BeautifulSoup.
- Extract movie rankings, titles, and release years.

**2. Data Processing**
- Organize extracted information into a pandas DataFrame.
- Limit the dataset to the top 50 movie records.

**3. Data Loading**
- Export movie information to `top_50_films.csv`.
- Store the records in the `Top_50` table within `Movies.db`.

## Dataset

The output contains 50 movie records with three fields:

| Column | Description |
|---|---|
| Average Rank | Movie ranking |
| Film | Movie title |
| Year | Release year |

## How to Run

1. Clone or download the repository.
2. Install the dependencies using `pip install -r requirements.txt`.
3. Execute `python webscraping_movies.py`.
4. Review the generated CSV and SQLite database files.

The pipeline requires access to the archived source webpage.

## Skills Demonstrated

- Web Scraping
- HTTP Requests
- HTML Parsing
- Data Extraction
- DataFrame Manipulation
- SQLite Database Integration
- Python Programming

## Future Improvements

- Add error handling for unavailable webpages.
- Validate extracted records.
- Add SQL queries for movie analysis.
- Implement automated execution and logging.

## Acknowledgment

Based on the IBM Data Engineering hands-on web scraping lab. This repository documents my implementation and learning process.

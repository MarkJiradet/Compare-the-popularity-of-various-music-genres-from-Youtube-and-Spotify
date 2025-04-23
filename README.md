# Compare the Popularity of Various Music Genres from YouTube and Spotify

## Project Overview
This project collects and analyzes music data from two of the most popular streaming platforms—Spotify and YouTube—to compare the popularity of various music genres across both services. By leveraging APIs, web scraping, and data visualization techniques, we offer insights into genre trends and listener preferences.

## Features
- **Data Collection**: Fetch data from Spotify using the Spotipy API and from YouTube via Selenium and Beautiful Soup.
- **Data Storage & Management**: Store and manage collected data in a MongoDB database for efficient querying and scalability.
- **Analysis & Visualization**: Perform in-depth comparisons of genre popularity using Python libraries such as Pandas, Seaborn, and Matplotlib.

## Technologies & Tools
- **Programming Language:** Python
- **Data Handling:** Pandas
- **Web Scraping:** Beautiful Soup, Selenium
- **APIs:** Spotipy (Spotify), YouTube Data (via scraping)
- **Database:** MongoDB
- **Visualization:** Seaborn, Matplotlib

## Repository Structure
```
Compare_the_popularity_of_various_music_genres/
├── Code
│   ├── Analyze.ipynb                  # Exploratory data analysis and visualizations
│   ├── Retrieve_data_from_MongoDB.ipynb  # Scripts to load data from MongoDB for analysis
│   ├── ScrapingYoutube.ipynb          # YouTube scraping logic with Selenium & Beautiful Soup
│   ├── Spotify_To_MongoDB.ipynb       # Ingest Spotify API data into MongoDB
│   ├── SpotifyAPI.ipynb               # Raw API calls to Spotify using Spotipy
│   ├── Youtube_To_MongoDB.ipynb       # Parse and store scraped YouTube data
│   ├── DatasetSPYT.xlsx               # Raw combined dataset for initial review
│   ├── Predict_Youtube.xlsx           # YouTube prediction results (if applicable)
│   ├── SpotifyDataset.xlsx            # Raw Spotify dataset export
│   └── YoutubeDataset.xlsx            # Raw YouTube dataset export
├── Database
│   ├── spotify_db.json                # Exported MongoDB collections for Spotify
│   └── youtube_db.json                # Exported MongoDB collections for YouTube
└── README.md                          # Project documentation
```

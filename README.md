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

## Installation & Setup
1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/Compare_the_popularity_of_various_music_genres.git
   cd Compare_the_popularity_of_various_music_genres
   ```
2. **Create a virtual environment** (optional but recommended):
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # macOS/Linux
   venv\Scripts\activate   # Windows
   ```
3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
4. **Configure environment variables:**
   - Create a `.env` file in the root directory and add your Spotify credentials:
     ```env
     SPOTIPY_CLIENT_ID=your_client_id
     SPOTIPY_CLIENT_SECRET=your_client_secret
     ```

## Usage
1. **Load data into MongoDB:**
   - Run `Spotify_To_MongoDB.ipynb` to fetch and store Spotify data.
   - Run `ScrapingYoutube.ipynb` and `Youtube_To_MongoDB.ipynb` to scrape and store YouTube data.
2. **Analyze the data:**
   - Open and run `Analyze.ipynb` to perform exploratory analysis and generate visualizations.
3. **Retrieve data for custom analysis:**
   - Use `Retrieve_data_from_MongoDB.ipynb` to pull data into a DataFrame for further processing.

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository
2. Create a feature branch (`git checkout -b feature-name`)
3. Commit your changes (`git commit -m "Add feature"`)
4. Push to the branch (`git push origin feature-name`)
5. Open a pull request

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

*Created by Jiradech "Mark" Narkham*


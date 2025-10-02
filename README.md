🎵 Spotify Streaming Popularity Analytics Dashboard

📌 Project Overview

This project presents a Power BI dashboard that analyzes the most streamed songs and artists on Spotify (2024 dataset). The goal is to uncover streaming patterns, highlight top-performing artists and tracks, and provide insights into music consumption trends.The dashboard helps explore key performance indicators (KPIs) around popularity, explicit content, platform presence, and streaming distribution, enabling deeper understanding of how artists and songs gain traction on Spotify.

⚙️ Tech Stack

💻 Power BI – For Data Modeling, Visualizations and Dashboard Design
💻 Microsoft Excel – For initial dataset exploration and cleaning
💻 DAX (Data Analysis Expressions) – For calculated measures and KPIs
💻 CSV Dataset – raw dataset format

📂 Data Source

Kaggle Dataset : https://www.kaggle.com/datasets/nelgiriyewithana/most-streamed-spotify-songs-2024
- Original Data Size: 4,600 tracks across 29 features.

Key Data Dimensions:
Core Track Details : Track, Album Name, Artist, Release Date.

Core Platform Metrics (All as object/string and need cleaning) : Spotify Streams, Spotify Playlist Count, Spotify Popularity.
YouTube Views, YouTube Likes.TikTok Posts, TikTok Views.Shazam Counts, AirPlay Spins, Pandora Streams, etc.

🛠️ Data Cleaning and Transformation 

Handling Non-Numeric Data: Convert all count and stream columns (e.g., Spotify Streams, YouTube Views) from object (string with commas) to a proper numeric data type (int64 or float64).

Example: $390,470,936 must be cleaned to 390470936.

Missing Data Strategy: Address significant null values in streaming metrics.

Imputation: For stream and count metrics, fill missing values (NaN) with 0 since an absence of a count often means 0 activity on that platform for that track/artist.

Dropping: Consider dropping the TIDAL Popularity column as it is entirely null (0 non-null values).

📌 Feature Engineering : 

Extract Year and Month from Release Date to enable time-series analysis on music trends.
Calculate composite metrics, such as Cross-Platform Engagement Score or Streams per Playlist.

🚀 Business Problem – Key Questions

- Who are the top artists by total streams on Spotify?
- Which songs have the highest number of streams?
- What is the distribution of explicit vs. clean tracks?
- Which albums/songs stand out as flagship hits for artists?
- How do song characteristics  relate to popularity?

🎯 Goal of the Dashboard

- Provide an interactive analytical view of Spotify’s most-streamed content
- Track artist-level performance and their top hits
- Identify listener trends in explicit content and song releases
- Enable music industry stakeholders (labels, producers, marketers) to make data-driven decisions
  
📊 Live Dashboard

 You can view the Spotify Streaming Popularity Analytics Dashboard :

🔗 You can explore it Live here : https://github.com/Sreeparvathy-Radhakrishnan/Spotify-Streaming-Popularity-Analytics-Dashboard/blob/main/Spotify%20Streaming%20Popularity%20Analytics%20Dashboard.pbit

📈 Dashboard Overview

✨ Home Page 
![Home Page](https://github.com/Sreeparvathy-Radhakrishnan/Spotify-Streaming-Popularity-Analytics-Dashboard/blob/main/Dashboard%20Images/Home%20Page.jpg)
✨ Overview 
![Overview](https://github.com/Sreeparvathy-Radhakrishnan/Spotify-Streaming-Popularity-Analytics-Dashboard/blob/main/Dashboard%20Images/Overview.jpg)
✨ Artists Insights
![Artists Insights](https://github.com/Sreeparvathy-Radhakrishnan/Spotify-Streaming-Popularity-Analytics-Dashboard/blob/main/Dashboard%20Images/Home%20Page.jpg)
✨Songs Insights 
![Songs Insights](https://github.com/Sreeparvathy-Radhakrishnan/Spotify-Streaming-Popularity-Analytics-Dashboard/blob/main/Dashboard%20Images/Song%20Insights.jpg)

📊 Walkthrough of Key Visuals

- Top 10 Artists by Streams – Highlights artists driving the most engagement
- Top 10 Songs by Streams – Identifies the most popular tracks globally
- Most Streamed Song (Flagship Hit) – Identifies each artist’s defining track
- Album Insights – Top albums based on cumulative streaming performance
- Slicers & Filters – Interactive options for deeper exploration (year, artist, explicit flag)

💡 Business Impact and Insights

Artist Benchmarking – quickly identify artists dominating Spotify in 2024
Content Strategy – insights into whether explicit or clean music gains more traction
Release Trends – understanding how newer vs. older tracks perform
Engagement Drivers – finding characteristics that boost streams

🎥 Demo
The Power BI dashboard visually demonstrates these insights with interactive charts and KPIs.

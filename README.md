🎵 Spotify Streaming Popularity Analytics Dashboard

📌 Project Overview

This project presents a Power BI dashboard that analyzes the most streamed songs and artists on Spotify (2024 dataset). The goal is to uncover streaming patterns, highlight top-performing artists and tracks, and provide insights into music consumption trends.The dashboard helps explore key performance indicators (KPIs) around popularity, explicit content, platform presence, and streaming distribution, enabling deeper understanding of how artists and songs gain traction on Spotify.

⚙️ Tech Stack

💻 Power BI – For Data Modeling, Visualizations and Dashboard Design <br>
💻 Microsoft Excel – For initial dataset exploration and cleaning<br>
💻 DAX (Data Analysis Expressions) – For calculated measures and KPIs<br>
💻 CSV Dataset – raw dataset format<br>

📂 Data Source

Kaggle Dataset : https://www.kaggle.com/datasets/nelgiriyewithana/most-streamed-spotify-songs-2024<br>
Original Data Size: 4,600 tracks across 29 features.

Key Data Dimensions:

- Core Track Details : Track, Album Name, Artist, Release Date.
- Core Platform Metrics (All as object/string and need cleaning) : Spotify Streams, Spotify Playlist Count, Spotify Popularity.
YouTube Views, YouTube Likes.TikTok Posts, TikTok Views.Shazam Counts, AirPlay Spins, Pandora Streams, etc.

🛠️ Data Cleaning and Transformation 

- Handling Non-Numeric Data : Convert all count and stream columns (e.g., Spotify Streams, YouTube Views) from object (string with commas) to a proper numeric data type (int64 or float64).
Example: $390,470,936 must be cleaned to 390470936.
- Missing Data Strategy : Address significant null values in streaming metrics.
- Imputation : For stream and count metrics, fill missing values (NaN) with 0 since an absence of a count often means 0 activity on that platform for that track/artist.
- Dropping : Consider dropping the TIDAL Popularity column as it is entirely null (0 non-null values).

📌 Feature Engineering : 

- Extract Year and Month from Release Date to enable time-series analysis on music trends.
- Calculate composite metrics, such as Cross-Platform Engagement Score or Streams per Playlist.

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

📈 Dashboard Overview

###  Home Page 

<br>This page serves as the user-friendly entry point and navigation hub for the entire dashboard. It provides a brief introduction to the project's goal (Cross-Platform Music Analysis) and contains clear, intuitive buttons or links to navigate to the main analytical sections: Overview, Artist Insights, and Song Insights. It ensures users can quickly orient themselves and access the data they need.<br><br>![Home Page](https://github.com/Sreeparvathy-Radhakrishnan/Spotify-Streaming-Popularity-Analytics-Dashboard/blob/main/Dashboard%20Images/Home%20Page.jpg)<br>
*****

###  Overview 

<br>This is the landing page of the dashboard, providing a high-level summary of key performance metrics, including total streams, total songs, and a monthly trend analysis. It serves as a quick snapshot of the entire dataset.<br><br>![Overview](https://github.com/Sreeparvathy-Radhakrishnan/Spotify-Streaming-Popularity-Analytics-Dashboard/blob/main/Dashboard%20Images/Overview.jpg)<br>
*****

###  Artists Insights

<br>This page focuses on artist performance. It highlights the top artists by total streams and provides a powerful cross-platform view, comparing an artist's popularity on Spotify, YouTube, and TikTok to guide marketing strategy.<br><br>![Artists Insights](https://github.com/Sreeparvathy-Radhakrishnan/Spotify-Streaming-Popularity-Analytics-Dashboard/blob/main/Dashboard%20Images/Artist%20Insights.jpg)<br>
*****

### Songs Insights 

<br>This page dives deep into individual song performance. It showcases the most streamed tracks, analyzes performance by album, and allows for a detailed comparison of a song's popularity across different platforms.<br><br>![Songs Insights](https://github.com/Sreeparvathy-Radhakrishnan/Spotify-Streaming-Popularity-Analytics-Dashboard/blob/main/Dashboard%20Images/Song%20Insights.jpg)<br>
*****

📊 Walkthrough of Key Visuals

- Top 10 Artists by Streams – Highlights artists driving the most engagement
- Top 10 Songs by Streams – Identifies the most popular tracks globally
- Most Streamed Song (Flagship Hit) – Identifies each artist’s defining track
- Album Insights – Top albums based on cumulative streaming performance
- Slicers & Filters – Interactive options for deeper exploration (year, artist, explicit flag)

💡 Business Impact and Insights

- Artist Benchmarking – quickly identify artists dominating Spotify in 2024
- Content Strategy – insights into whether explicit or clean music gains more traction
- Release Trends – understanding how newer vs. older tracks perform
- Engagement Drivers – finding characteristics that boost streams

🚀 Future Enhancements

- Integrate Additional Data Sources: Incorporate data from other platforms like TikTok Analytics and chart data from Billboard to enrich the analysis.
- Create a Predictive Model: Develop a machine learning model to predict a song's virality based on its initial streaming and social media metrics.
- Add Advanced Filtering: Implement more granular filters for genres, regions, and song moods to provide deeper, niche-specific insights.
- Automate Data Refresh: Set up a scheduled data pipeline using a tool like Power Automate or Python to automatically refresh the dashboard with the latest streaming data.
  
🎉 Conclusion

This Spotify Streaming  Popularity Analytics Dashboard successfully transforms complex, cross-platform data into a clear and intuitive visualization tool. It provides music industry professionals with the critical insights needed to make data-driven decisions on artist promotion, marketing budget allocation, and revenue optimization, proving the power of a strategic data-centric approach.

🎥 Demo

This section provides immediate access and a visual preview of the deployed dashboard.Click the button below to access the full, interactive Power BI Dashboard hosted on the web. Explore real-time trends, filter artists, and compare cross-platform performance live.<br>
🔗 View Live Dashboard : [View Interactive Dashboard Here](https://github.com/Sreeparvathy-Radhakrishnan/Spotify-Streaming-Popularity-Analytics-Dashboard/blob/main/Spotify%20Streaming%20Popularity%20Analytics%20Dashboard.pbit)


✍️ Author

Name : Sreeparvathy Radhakrishnan <br>
LinkedIn : [ LinkedIn Profile URL](https://www.linkedin.com/in/sreeparvathy-radhakrishnan-151883249/)


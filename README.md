<h1>Spotify Top 50 Charts in Spanish-Speaking Countries Analysis</h1>

<h2>Project Overview</h2>

<p>Spotify's Top 50 charts are determined based on the listening habits of Spotify users. These charts reflect the popularity of songs within a specific region or country over a set period, typically from Friday to the following Thursday. The charts are updated weekly and are influenced by the number of streams each song receives during this period. Essentially, the more streams a song gets, the higher it ranks on the chart. The "Top 50 - Ecuador" chart, for example, showcases the 50 most popular songs in Ecuador based on Spotify streaming data.</p>

<p>This project focuses on analyzing the top 50 charts of all Spanish-speaking countries (except Cuba) for the period from Friday, July 19 - Thursday, July 25, 2024. This resulted in a dataset of 900 songs (18 countries x 50 songs per country). As someone from a Spanish-speaking country (Ecuador), this topic is particularly interesting to me. The analysis aims to uncover trends and insights within the music preferences of these regions. The primary goals are to collect data from Spotify, store and manage it using SQL, perform detailed data analysis through SQL queries in Python, and visualize the findings using Tableau.</p>


<h3>Key Objectives:</h3>
<ul>
    <li><strong>Data Collection</strong>: Retrieve data from Spotify's API for the top 50 charts in Spanish-speaking countries.</li>
    <li><strong>Data Storage and Management</strong>: Structure and store the data using SQL for efficient querying and analysis.</li>
    <li><strong>Data Analysis</strong>: Utilize SQL queries within Python to extract meaningful insights from the data.</li>
    <li><strong>Data Visualization</strong>: Create comprehensive visualizations using Tableau to present the findings effectively.</li>
</ul>

<h2>Repository Structure</h2>
<pre>
.
├── .cache
├── README.md
├── SQL_queries.ipynb
├── SQL_queries_in_Python.html
├── Spotify Tableau Dashboard.png
├── Spotify_Analysis_Dashboard.twb
├── Spotify_SQL_queries_in_Python.pdf
├── artist_genre_df.csv
├── artists_data.csv
├── data_collection_and_db_creation.ipynb
├── track_data.csv
├── track_data.hyper
</pre>

<h3>Files Description</h3>
<ul>
    <li><strong>SQL_queries.ipynb</strong>: Jupyter notebook demonstrating the execution of SQL queries through Python.</li>
    <li><strong>SQL_queries_in_Python.html</strong>: HTML version of the SQL queries Jupyter notebook.</li>
    <li><strong>Spotify_SQL_queries_in_Python.pdf</strong>: PDF version of the SQL queries Jupyter notebook.</li>
    <li><strong>Spotify Tableau Dashboard.png</strong>: Image of the Tableau dashboard created for this project.</li>
    <li><strong>Spotify_Analysis_Dashboard.twb</strong>: Tableau workbook file for the Spotify data analysis dashboard.</li>
    <li><strong>artist_genre_df.csv</strong>: CSV file containing artist genre data.</li>
    <li><strong>artists_data.csv</strong>: CSV file containing artist data.</li>
    <li><strong>data_collection_and_db_creation.ipynb</strong>: Jupyter notebook for collecting data from Spotify using the Spotipy API and creating the database.</li>
    <li><strong>track_data.csv</strong>: CSV file containing track data.</li>
    <li><strong>track_data.hyper</strong>: Hyper file for Tableau visualization.</li>
</ul>

<h2>Data Collection and Database Creation</h2>
<p>The data collection process involves using the Spotipy API to retrieve data from Spotify. The collected data is stored in three main tables:</p>

<h3>Track Data (track_data.csv)</h3>
<ul>
    <li>Columns: track_id, track_name, artist_id, album_id, track_popularity, track_duration_ms, explicit</li>
</ul>

<h3>Artist Data (artists_data.csv)</h3>
<ul>
    <li>Columns: artist_id, artist_name, artist_followers, artist_popularity</li>
</ul>

<h3>Artist Genre Data (artist_genre_df.csv)</h3>
<ul>
    <li>Columns: artist_id, genre</li>
</ul>

<p>The <em>data_collection_and_db_creation.ipynb</em> notebook details the steps for data collection and database creation, ensuring that the data is properly structured for efficient querying and analysis.</p>

<h2>SQL Queries in Python</h2>
<p>The <em>SQL_queries.ipynb</em> notebook demonstrates how SQL queries can be executed within a Python environment. This approach allows for powerful data manipulation and analysis capabilities, leveraging the strengths of both SQL and Python.</p>

<h2>Data Visualization</h2>

<img src="./Spotify Tableau Dashboard.png" alt="Spotify Tableau Dashboard">

<h3>Tableau Dashboard Insights</h3>
<p>The Tableau dashboard provides a comprehensive visualization of the Spotify Top 50 charts in Spanish-speaking countries. Key insights include:</p>

<ul>
    <li><strong>Most Followed Artists</strong>: This section highlights the artists with the highest number of followers. Notable names include Billie Eilish, The Weeknd, and Bad Bunny.</li>
    <li><strong>Top 15 Genres</strong>: Visual representation of the most popular genres, with "urbano latino," "trap latino," and "reggaeton" leading the charts.</li>
    <li><strong>Artists with the Most Songs</strong>: Lists artists with the highest number of songs in the Top 50 charts, such as Feid, KAROL G, and Myke Towers.</li>
    <li><strong>Explicit Content</strong>: Pie chart showing the proportion of explicit content in the Top 50 charts. "Explicit" indicates that the song contains explicit language or content that may be considered inappropriate for some audiences.</li>
    <li><strong>Most Songs in Top 50 Charts</strong>: Highlights the songs that appear most frequently in the Top 50 charts across Spanish-speaking countries.</li>
</ul>

<p>Users can filter the top N artists, genres, and songs directly within the Tableau dashboard for more customized insights.</p>

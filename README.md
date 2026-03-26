#  Spotify Music Data Analysis

##  Project Overview

This project analyzes Spotify track data to explore relationships between audio features and song popularity, as well as trends in music production over time.

---

##  Problem Statement

Understanding what makes a song popular is complex due to multiple interacting audio features. This project aims to uncover patterns and relationships between features such as energy, loudness, acousticness, and popularity.

---

##  Dataset

* Source: Spotify Tracks Dataset (Kaggle)
* Link: https://www.kaggle.com/datasets/yamaerenay/spotify-dataset-19212020-600k-tracks?select=tracks.csv
* Records: ~586,000 songs
* Features include:

  * Popularity (0–100)
  * Energy
  * Loudness
  * Danceability
  * Acousticness
  * Release Date
  * Tempo
  * Valence

---

##  Tools & Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn

---

##  Approach

### 1. Data Cleaning

* Converted `release_date` to datetime format
* Created `duration` feature from milliseconds
* Handled missing values safely

### 2. Exploratory Data Analysis

* Selected numerical features
* Generated correlation heatmap

### 3. Feature Relationships

* Energy vs Loudness (strong positive correlation)
* Acousticness vs Popularity (negative trend)

### 4. Time-Based Analysis

* Extracted release year
* Analyzed growth of music production over time

---

##  Key Insights

*  Energy and loudness are strongly positively correlated (~0.76)
*  Acoustic songs tend to be less popular
*  Danceability and valence show moderate correlation
*  Extremely high acousticness tracks rarely achieve high popularity
*  Music production increased significantly after 1980
*  Peak song releases occurred between 2000–2020

---

##  Visualizations

### Correlation Heatmap

![Heatmap](images/heatmap.png)

### Energy vs Loudness

![Energy vs Loudness](images/energy_loudness.png)

### Acousticness vs Popularity

![Acousticness vs Popularity](images/acoustic_popularity.png)

### Songs Released Over Time

![Year Distribution](images/year_distribution.png)

---

##  Impact

* Helps understand key features influencing music characteristics
* Useful for building recommendation systems
* Provides foundation for predicting song popularity

---

##  Future Work

* Build machine learning model to predict popularity
* Perform genre-based analysis
* Create interactive dashboards (Streamlit / Power BI)

---

##  Conclusion

This project demonstrates how data analysis can uncover meaningful insights in music trends, helping both producers and analysts understand what drives modern music.

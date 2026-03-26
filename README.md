#  Spotify Music Data Analysis

##  Project Overview

This project analyzes Spotify track data to explore relationships between audio features and song popularity, along with trends in music production over time. The goal is to extract meaningful insights from a large real-world dataset and understand patterns in modern music.

---

##  Problem Statement

Understanding what makes a song popular is complex due to multiple interacting audio features. This project aims to uncover patterns and relationships between features such as energy, loudness, acousticness, and popularity using exploratory data analysis.

---

##  Dataset

* Source: Spotify Tracks Dataset (Kaggle)
* Link: https://www.kaggle.com/datasets/yamaerenay/spotify-dataset-19212020-600k-tracks?select=tracks.csv
* Size: ~586,000 tracks
* Time Range: 1920–2020

### Features include:

* Popularity (0–100)
* Danceability
* Energy
* Loudness
* Acousticness
* Instrumentalness
* Valence
* Tempo
* Release Date

>  Note: Dataset (~111MB) is not included in this repository due to GitHub size limits.

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
* Handled invalid/missing values using safe conversion
* Created `duration` feature from milliseconds

### 2. Exploratory Data Analysis

* Selected numerical features
* Generated correlation heatmap

### 3. Feature Relationships

* Analyzed relationships between:

  * Energy vs Loudness
  * Acousticness vs Popularity

### 4. Time-Based Analysis

* Extracted release year
* Analyzed growth of music production over time

---

##  Key Insights

*  Energy and loudness are strongly positively correlated (~0.76)
*  Higher energy tracks consistently exhibit higher loudness
*  Acoustic songs tend to be less popular
*  Tracks with very high acousticness rarely achieve high popularity
*  Danceability and valence show moderate positive correlation
*  Music production increased significantly after 1980
*  Peak song releases occurred between 2000–2020
*  Dataset is skewed toward modern music, which may influence analysis

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

##  How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/varshaponnaganti7/spotify-data-analysis.git
   ```

2. Navigate to the project folder:

   ```bash
   cd spotify-data-analysis
   ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Open the notebook:

   ```bash
   jupyter notebook spotify_analysis.ipynb
   ```

---

##  Project Structure

```
spotify-data-analysis/
│
├── images/
│   ├── heatmap.png
│   ├── energy_loudness.png
│   ├── acoustic_popularity.png
│   └── year_distribution.png
│
├── spotify_analysis.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

---

##  Impact

* Helps understand key features influencing music characteristics
* Provides insights useful for music recommendation systems
* Forms a foundation for predictive modeling of song popularity

---

##  Future Work

* Build a machine learning model to predict song popularity
* Perform genre-based or artist-based analysis
* Develop an interactive dashboard (Streamlit / Power BI)

---

##  Conclusion

This project demonstrates how data analysis can uncover meaningful insights in music trends using real-world data. It highlights the importance of feature relationships and temporal patterns in understanding modern music.

---

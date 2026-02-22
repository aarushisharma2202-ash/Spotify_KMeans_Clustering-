
# Mining Hidden Patterns in Music Listening Data Using K-Means Clustering 🎵

## Project Overview

This project explores **hidden patterns in music listening data** using **K-Means clustering**. The goal is to group songs based on audio features and popularity to uncover insights that can support **playlist generation, recommendations, and music categorisation**.

**Key Skills Demonstrated:**

* Data cleaning and preprocessing
* K-Means clustering and Elbow Method
* Data visualisation in Python
* Dashboarding and report generation
* Translating analytical results into actionable insights

---

## Dataset

The dataset contains numerical features for over 50 songs, including:

* `track_duration` – Duration of the song (ms)
* `energy` – Intensity and activity level
* `tempo` – Beats per minute (BPM)
* `loudness` – Overall loudness (dB)
* `popularity_score` – Popularity of the song

> Non-numeric features like song names and track IDs were removed before clustering. Data was normalized using **min-max scaling** to ensure all features contributed equally.

---

## Methodology

1. **Data Cleaning & Preprocessing**

   * Merged multiple CSV files by `track_id`
   * Removed non-numeric columns
   * Applied min-max normalization to scale features

2. **K-Means Clustering**

   * Determined optimal number of clusters using the **Elbow Method**
   * Applied K-Means clustering with the chosen k value
   * Analysed clusters for patterns in audio features and popularity

3. **Visualization & Interpretation**

   * Scatter plots to visualise clusters
   * Feature distributions by cluster to identify unique characteristics

4. **Tools & Libraries**

   * Python (Google Colab)
   * pandas, scikit-learn, matplotlib, seaborn

---

## Results

**Clusters Identified (k = 4):**

* **Cluster 1:** Upbeat popular songs – high energy, louder, ideal for sports/party playlists
* **Cluster 2:** Moderate-energy mainstream tracks – balanced audio properties and popularity
* **Cluster 3:** Low energy / low tempo tracks – suitable for relaxing or concentration playlists
* **Cluster 4:** Less popular but musically strong – high danceability/tempo, lower popularity, good for exploration

These clusters can help streaming platforms **curate playlists, recommend songs**, and identify **underrated tracks with strong musical qualities**.

---

## 📊 Visualisations

### Elbow Method Plot

Determined the optimal number of clusters (k) using the Elbow Method. The plateau point indicates the best k value.

![Elbow Method Plot](![image](https://github.com/user-attachments/assets/6dd33f90-b9fb-4a8c-bf07-82c5020a5d4e)
)

---

### Cluster Scatter Plot

Shows how songs are grouped into clusters based on their audio features and popularity.

![Cluster Scatter Plot](![image](https://github.com/user-attachments/assets/7c7991b9-bfa5-4126-ae99-a483cdb93a1d)
)


---

## How to Run the Code

1. Open the Jupyter Notebook (`.ipynb`) in **Google Colab** or locally.
2. Make sure you have installed the following Python libraries:

   ```bash
   pip install pandas matplotlib seaborn scikit-learn
   ```
3. Run all cells to preprocess data, perform clustering, and generate visualisations.

---

## Repository Structure

```
├── images/
│   ├── elbow_plot.png
│   ├── cluster_scatter.png
├── kmeans_music_analysis.ipynb
├── README.md
└── dataset.csv
```

---

## Key Insights

* K-Means clustering effectively groups songs based on audio features and popularity.
* Popularity does not always correlate with musical characteristics, highlighting underrated songs.
* Clusters can inform **playlist creation, music recommendations, and digital content strategies**.



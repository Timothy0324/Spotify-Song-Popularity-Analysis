# 🎵 Spotify-Song-Popularity-Analysis
**Author:** Timothy Liu  

---

## Dataset Source & Files

Spotify Tracks Dataset — Kaggle

🔗 [https://archive.ics.uci.edu/ml/datasets/Chronic_Kidney_Disease](https://www.kaggle.com/datasets/maharshipandya/-spotify-tracks-dataset)


**Full Report (PDF):**  
[View Presentation](What%20Makes%20a%20Song%20Popular_1128.pdf)

**Jupyter Notebook:**  
[Open Notebook](What%20makes%20a%20song%20popular%20(Spotify)%20-%20Timothy%20Liu.ipynb)

---

## Project Overview
This analysis investigates:

- The distribution of song popularity on Spotify  
- Correlations between audio features and popularity  
- Genre-level differences  
- Whether explicit content influences performance  
- Predictive modeling using **Random Forest Regression**

The goal is to understand which musical characteristics (if any) meaningfully contribute to high popularity—and what this means for artists, producers, and streaming platforms.

---

## Dataset
- **Source:** Spotify tracks dataset  
- **Size:** ~114,000 songs  
- **Target variable:** `popularity` (0–100)  
- **Features analyzed:**  
  - danceability  
  - energy  
  - loudness  
  - acousticness  
  - speechiness  
  - valence  
  - instrumentalness  
  - tempo  
  - explicit (True/False)  
  - genre  

---

## Key Findings

### Popularity Distribution  
As shown in *page 4 of the PDF*, most songs are **not popular**.  
Only a small fraction reach a popularity score above 80.

### Correlation Insights  
Based on the heatmap in *page 5*, **no single audio feature strongly predicts popularity**.  
- Loudness has the highest correlation (~0.05), but still weak.  
- Danceability and energy show only slight positive trends.

**Implication:**  
Popularity depends more on **external forces** than on audio composition alone.

### Danceability  
Scatterplot in *page 6* shows weak correlation.  
Danceable songs *may* perform better, but there is huge variance.

### Energy  
From *page 7*, high-energy songs are not necessarily more popular.  
Soft ballads and high-energy EDM can both be hits.

### Explicit Content  
Box plot on *page 8* shows **no advantage** for explicit songs.  
Hits can be clean or explicit.

### Top Genres  
From *page 9*:  
- **Pop-film** and **K-pop** top the list  
- Chill/sad genres perform well  
- Anime/Indian music are *fast-growing opportunities*

---

## Predictive Modeling
Model: **Random Forest Regression**  
- **MAE ≈ 10.78**

Conclusion from *page 10*:  
Audio features alone **cannot reliably predict popularity**.  
Future models should incorporate:
- Social media engagement  
- Artist fame  
- Playlist exposure  
- Release timing  

---

## Conclusion
Key business implications (page 11):

- No musical feature guarantees popularity  
- Popularity is shaped by marketing, playlisting, and artist reputation  
- Genre-based promotion works better  
- Mood-driven playlists (chill, sad, study) are increasingly important  

Future research should integrate **external features** like TikTok trends, follower count, and streaming momentum.

---

## 🛠️ Tools Used
- Python (pandas, numpy, seaborn, matplotlib, sklearn)  
- Random Forest Regression  
- Data cleaning & wrangling  
- Correlation and exploratory data analysis  
- Visual storytelling & business insights  

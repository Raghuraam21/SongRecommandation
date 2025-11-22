# 🎵 Spotify Listening Data Analysis & BERT-Based Song Recommendation

This project analyzes personal Spotify listening history and uses a BERT-based model to recommend similar tracks based on your listening behavior and track metadata.

---

## 📌 Features

* 📊 Exploratory Data Analysis:

  * Most listened artists and albums
  * Listening patterns by time
  * Track skip rate
  * User behavior insights

* 📈 Visualizations:

  * Artist frequency bar plots
  * Listening time histograms
  * Hourly activity line plots
  * Pie charts of listening reasons

* 🧠 BERT-Based Recommendation System:

  * Uses BERT embeddings to find similar tracks
  * Generates song recommendations based on cosine similarity
  * Engagement label prediction (Low, Medium, High)

---

## 🗂️ Dataset

* **File Used:** `spotify_history.csv` which is in kaggle
* Contains:

  * `track_name`, `artist_name`, `album_name`
  * `ms_played`, `ts` (timestamp), `reason_start`, `reason_end`, `skipped`

---

## 🛠️ Tech Stack

* Python 🦀
* pandas, numpy
* matplotlib, seaborn
* PyTorch, HuggingFace Transformers 🤗
* scikit-learn

---

## 🚀 How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/Raghuraam21/SongRecommandation.git
   ```



## 🧠 How It Works

1. **Preprocessing**:

   * Extracts features like hour, minute, and total play time
   * Generates a text field from track, artist, album
   * Labels engagement levels (Low < 10s, Medium, High > 60s)

2. **BERT Embedding**:

   * Uses `bert-base-uncased` to generate vector embeddings from text
   * Compares track embeddings using cosine similarity

3. **Recommendation**:

   * Given a seed song, finds top-k most similar tracks

---

## 📌 Example Output

```
Based on your listening to: 'Born To Die' by Lana Del Rey  
Recommended tracks:  
1. Summertime Sadness by Lana Del Rey (similarity: 0.943)  
2. Young and Beautiful by Lana Del Rey (similarity: 0.938)  
3. Video Games by Lana Del Rey (similarity: 0.927)
```




## 📬 Contact

Made by Raghuraam


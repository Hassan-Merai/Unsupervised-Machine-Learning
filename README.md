# Unsupervised-Machine-Learning
🎧 Smart Playlist Generation using Machine Learning &amp; Spotify Audio Features  
This project demonstrates how to automatically cluster 5,000 Spotify tracks into human-like playlists using unsupervised learning. It leverages weighted audio features, MinMax scaling, and KMeansConstrained to generate 45 musically coherent playlists.


[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![Spotify API](https://img.shields.io/badge/Spotify%20API-Enabled-brightgreen)](https://developer.spotify.com/documentation/web-api/)

Automatically group 5,000 Spotify songs into **human-like playlists** using unsupervised learning, custom feature weighting, and clustering with size constraints. This project generates **45 coherent playlists**, each between 50 and 250 songs, by using only the audio features from the Spotify API.

---

## 📈 Demo Preview

![Clustering Results Presentation](https://docs.google.com/presentation/d/1Supwql6Tjsp6WrbA1mp9ue9IY_zc4JSq/edit?usp=sharing&ouid=108748831738353750828&rtpof=true&sd=true) <!-- Replace with your own image -->

---

## 🌐 Live Article

Read more on Medium: [Teaching Machines to Curate Music](https://medium.com/@hassanmerai79/teaching-machines-to-curate-music-smart-playlist-generation-using-clustering-and-spotify-audio-6dc1444e0063) <!-- Replace with your actual Medium link -->

---

## 📊 Features

* Pulls audio features from Spotify API
* Scales and applies feature weighting
* Uses KMeansConstrained to enforce playlist size constraints
* Generates clusters that reflect musical similarity
* Creates Spotify playlists via the Spotipy client

---

## 🚀 Tech Stack

* **Python 3.8+**
* `pandas`, `scikit-learn`, `k-means-constrained`
* `Spotipy` for Spotify API access
* `matplotlib`, `seaborn` for visualization

---

## 🔎 How It Works

```bash
1. Collect Spotify audio features using Spotipy
2. Scale features using MinMaxScaler
3. Apply custom weights to audio features
4. Use KMeansConstrained to cluster songs
5. Evaluate clusters using silhouette score
6. Generate playlists and push to Spotify
```

---

## 💡 Example Playlist Clusters

| Playlist   | Characteristics                     | Sample Use Case       |
| ---------- | ----------------------------------- | --------------------- |
| Cluster 14 | High danceability, upbeat valence   | Summer vibes playlist |
| Cluster 22 | Low energy, acoustic & instrumental | Focus / chill mix     |

---

## 📑 Project Structure

```
├── data/                 # (Optional) Audio data or backup CSVs
├── notebooks/            # Google Colab notebooks for development
├── images/               # Visuals and charts for documentation
├── LICENSE
├── README.md
```

---

## 🔧 Setup Instructions

1. **Clone the repository**

```bash
git clone https://github.com/Hassan-Merai/Unsupervised-Machine-Learning.git
cd Unsupervised-Machine-Learning
```

2. **Set up Spotify API credentials**
   Create a `.env` file or insert directly into your script:

```env
SPOTIPY_CLIENT_ID=your_id
SPOTIPY_CLIENT_SECRET=your_secret
SPOTIPY_REDIRECT_URI=https://example.com/callback/
```

4. **Run the notebook** or script to generate playlists

---

## 📅 Future Improvements

* Add NLP-based lyrics clustering
* Integrate genre detection
* Improve playlist naming with GPT
* Build a web app interface for users

---

## 🎓 License

This project is licensed under the [MIT License](LICENSE).

---

## 👋 Contact

**Hassan Merai (Fred)**
[LinkedIn](https://linkedin.com/in/hassan-merai-nickname-fred/) | [Medium](https://medium.com/@hassanmerai79)
Want to collaborate or learn more? Reach out anytime!

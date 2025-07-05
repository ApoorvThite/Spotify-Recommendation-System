# 🎧 VibeTune: Spotify-Based Music Recommendation System

VibeTune is an intelligent music recommendation system that leverages Spotify's audio features to suggest songs based on mood and musical similarity. It combines traditional similarity metrics, machine learning, and clustering techniques to deliver highly relevant music suggestions.

## 🚀 Features

- 🎼 Cleans and merges multiple Spotify datasets
- 📊 Performs Exploratory Data Analysis (EDA) on audio features
- 🤝 Implements 3 unique recommendation techniques:
  - **Cosine Similarity** (Content-Based Filtering)
  - **K-Nearest Neighbors** (Machine Learning)
  - **KMeans + t-SNE Clustering** (Mood-Based Grouping)

## 📁 Project Structure

Spotify_Recommendation_System.ipynb
data/
│ ├── Spotify Audio Features Dataset
│ └── Spotify Artist-Song Dataset
README.md

markdown
Copy
Edit

## 🛠️ Techniques Used

### 1. Data Preprocessing
- Normalized inconsistent song names and artists
- Merged audio feature dataset with metadata (song name, artist)
- Removed noise such as "Explicit Version" annotations

### 2. Exploratory Data Analysis (EDA)
- Analyzed distributions of audio features (e.g., energy, danceability)
- Examined correlations between variables
- Visualized feature spaces using histograms and pair plots

### 3. Recommendation Engines

#### 📌 Technique 1: Cosine Similarity
- Uses cosine distance between audio features
- Returns musically similar songs to a given input

#### 📌 Technique 2: K-Nearest Neighbors (KNN)
- Standardized features like danceability and acousticness
- Used Euclidean distance to recommend similar songs

#### 📌 Technique 3: Clustering + Mood Mapping
- Applied KMeans clustering to group songs
- Used t-SNE to visualize clusters
- Assigned mood-based labels (e.g., "Chill", "Party", "Energetic")

## 📊 Requirements

- Python 3.x
- pandas, numpy, scikit-learn, seaborn, matplotlib
- Jupyter Notebook

```bash
pip install pandas numpy scikit-learn seaborn matplotlib jupyter
▶️ Getting Started
Clone the repo:

bash
Copy
Edit
git clone https://github.com/yourusername/vibetune.git
cd vibetune
Launch the notebook:

bash
Copy
Edit
jupyter notebook Spotify_Recommendation_System.ipynb
```
Run cells in order to see:

Cleaned data

Audio feature visualizations

Recommendation outputs

📌 Future Work
Integrate with Spotify Web API for real-time recommendations

Build a web-based frontend using Flask or Streamlit

Deploy as a recommendation microservice

🧠 Inspiration
This project is inspired by Spotify’s goal to personalize music discovery through machine learning and the emotional connections we form with music.

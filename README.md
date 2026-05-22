# 🎬 CineYantra — AI Movie Recommendation System

<div align="center">

![CineYantra](https://img.shields.io/badge/CineYantra-AI%20Movie%20Recommendation-e50914?style=for-the-badge&logo=film)

[![Python](https://img.shields.io/badge/Python-3.10-blue?style=flat-square&logo=python)](https://python.org)
[![Flask](https://img.shields.io/badge/Flask-3.0-green?style=flat-square&logo=flask)](https://flask.palletsprojects.com)
[![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-orange?style=flat-square)](https://scikit-learn.org)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)](LICENSE)

### 🎥 Offline AI-Powered Movie Recommendation System  
Modern Netflix-inspired dark UI with Machine Learning 🤖

</div>

---

# ✨ Features

- 🤖 AI-based Movie Recommendations
- 🎬 Content-Based Filtering
- ⚡ Cosine Similarity Algorithm
- 🌙 Netflix-inspired Dark UI
- 🔍 Smart Movie Search
- 🎭 Genre Browsing
- 📱 Fully Responsive Design
- 💾 100% Offline Project
- 🚀 Fast & Lightweight
- ❤️ Watchlist Feature

---

# 🧠 How It Works

```text
Movie Selected
      ↓
TF-IDF Vectorization
      ↓
Cosine Similarity
      ↓
Similar Movie Detection
      ↓
AI Recommendations
```

### 🔬 ML Concepts Used
- TF-IDF Vectorizer
- Cosine Similarity
- Content-Based Filtering
- Feature Engineering

---

# 🛠️ Tech Stack

| Category | Technology |
|----------|-------------|
| Backend | Python, Flask |
| Machine Learning | Scikit-learn, Pandas, NumPy |
| Frontend | HTML, CSS, JavaScript |
| UI Style | Netflix Dark Theme |
| Dataset | TMDB 5000 Movies Dataset |

---

# 📁 Project Structure

```bash
CineYantra/
│
├── app.py
├── recommender.py
├── requirements.txt
├── README.md
│
├── data/
│   ├── tmdb_5000_movies.csv
│   └── tmdb_5000_credits.csv
│
├── templates/
│   ├── index.html
│   ├── movie.html
│   ├── search.html
│   └── 404.html
│
└── static/
    ├── css/
    │   └── style.css
    ├── js/
    │   └── main.js
    └── posters/
```

---

# 📥 Dataset

Download the TMDB dataset from Kaggle:

🔗 https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata

Place these files inside the `data/` folder:

- `tmdb_5000_movies.csv`
- `tmdb_5000_credits.csv`

---

# 🚀 Installation & Setup

## 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/CineYantra.git
cd CineYantra
```

---

## 2️⃣ Install Dependencies

```bash
py -m pip install -r requirements.txt
```

---

## 3️⃣ Run Project

```bash
py app.py
```

---

## 4️⃣ Open in Browser

```text
http://127.0.0.1:5000
```

---

# 🎯 API Routes

| Route | Description |
|------|-------------|
| `/` | Homepage |
| `/search` | Search Movies |
| `/movie/<id>` | Movie Details |
| `/api/recommend` | Get Recommendations |
| `/api/autocomplete` | Search Suggestions |

---

# 🖼️ UI Highlights

- 🌌 Cinematic Hero Section
- ✨ Glassmorphism Effects
- 🎞️ Animated Movie Cards
- 🌙 Dark Premium Theme
- 📱 Responsive Layout
- ⚡ Smooth Hover Animations

---

# 📊 Recommendation Algorithm

CineYantra uses:

- TF-IDF Vectorization
- Cosine Similarity Matrix
- Movie Metadata Analysis

The model compares:
- Genres
- Overview
- Keywords
- Cast
- Director

to recommend similar movies intelligently.

---

# 🔥 Future Improvements

- 🎤 Voice Search
- 🎥 Movie Trailer Support
- ⭐ User Ratings
- ❤️ Cloud Watchlist
- 🌐 Online API Integration
- 🧠 Hybrid Recommendation System

---

# 🤝 Contributing

Contributions are welcome!

```bash
Fork → Clone → Create Branch → Commit → Push → Pull Request
```

---

# 📄 License

This project is licensed under the MIT License.

---

# 👨‍💻 Author

### Bismaya Guruprasad Panda

Built with ❤️ By Bismaya Guruprasad Panda
---

<div align="center">

## ⭐ If you like this project, give it a star!

🎬 Happy Movie Watching with CineYantra 🍿

</div>

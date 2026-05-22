# 🎬 MayaFlix - AI Movie Recommendation System

<div align="center">

![MayaFlix Banner](https://img.shields.io/badge/MayaFlix-AI%20Movie%20Recommendations-e50914?style=for-the-badge&logo=film)

[![Python](https://img.shields.io/badge/Python-3.8+-blue?style=flat-square&logo=python)](https://python.org)
[![Flask](https://img.shields.io/badge/Flask-3.0-green?style=flat-square&logo=flask)](https://flask.palletsprojects.com)
[![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.3-orange?style=flat-square)](https://scikit-learn.org)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)](LICENSE)

**An offline AI-powered movie recommendation web app with Netflix-inspired dark UI**

</div>

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 🤖 **AI Recommendations** | Content-Based Filtering with Cosine Similarity |
| 🎨 **Netflix-Dark UI** | Glassmorphism, animations, cinematic design |
| 🔍 **Smart Search** | Real-time autocomplete search |
| 🎭 **Genre Browsing** | Filter movies by genre |
| 💾 **100% Offline** | No API keys needed |
| 📱 **Responsive** | Works on all screen sizes |
| ❤️ **Watchlist** | Save favorite movies locally |
| ⚡ **Fast** | Optimized TF-IDF + Cosine similarity |

---

## 🧠 How It Works
User Input (Movie Title)
↓
TF-IDF Vectorization
(Overview + Genres + Keywords + Cast + Director)
↓
Cosine Similarity Matrix
↓
Top N Similar Movies
↓
Ranked Results → UI

text


### Algorithm Details:
- **TF-IDF Vectorizer**: Converts movie metadata into numerical vectors
- **Cosine Similarity**: Measures angle between movie vectors (0=different, 1=identical)
- **Feature Weights**: Genres×3 > Keywords×2 > Overview×2 > Director×2 > Cast×1
- **Bayesian Rating**: For better top-rated movie ranking

---

## 📁 Project Structure
MayaFlix/
├── 📄 app.py # Flask application & routes
├── 🧠 recommender.py # AI recommendation engine
├── 📋 requirements.txt # Python dependencies
├── 📖 README.md # This file
│
├── 📂 data/ # Dataset directory
│ ├── tmdb_5000_movies.csv # ← Place your TMDB file here
│ └── tmdb_5000_credits.csv # ← Place your TMDB file here
│
├── 📂 templates/ # Jinja2 HTML templates
│ ├── index.html # Homepage
│ ├── movie.html # Movie detail page
│ ├── search.html # Search & browse page
│ └── 404.html # Error page
│
└── 📂 static/
├── 📂 css/
│ └── style.css # Full Netflix-dark stylesheet
└── 📂 js/
└── main.js # Interactive JavaScript

text


---

## 🚀 Setup & Installation

### Prerequisites
- Python 3.8+
- TMDB 5000 Movie Dataset from Kaggle

### Step 1: Download Dataset
1. Go to [Kaggle TMDB Dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)
2. Download `tmdb_5000_movies.csv` and `tmdb_5000_credits.csv`
3. Place both files in the `data/` folder

### Step 2: Install Dependencies

```bash
# Create virtual environment
python -m venv venv

# Activate it
# Windows:
venv\Scripts\activate
# macOS/Linux:
source venv/bin/activate

# Install requirements
pip install -r requirements.txt
Step 3: Run MayaFlix
Bash

python app.py
Step 4: Open in Browser
text

http://localhost:5000
🎯 API Endpoints
Endpoint	Method	Description
/	GET	Homepage with featured movies
/search?q=batman	GET	Search movies
/genre/Action	GET	Browse by genre
/movie/<id>	GET	Movie detail + recommendations
/api/recommend	POST	AI recommendations JSON
/api/search?q=query	GET	Search API
/api/autocomplete?q=bat	GET	Autocomplete API
API Example:
Python

import requests

response = requests.post('http://localhost:5000/api/recommend', 
    json={'title': 'The Dark Knight', 'n': 10})
print(response.json())
🛠️ Tech Stack
Layer	Technology
Backend	Python 3.8+, Flask 3.0
ML Engine	Scikit-learn, Pandas, NumPy
Algorithm	TF-IDF + Cosine Similarity
Frontend	HTML5, CSS3, JavaScript (Vanilla)
UI Style	Glassmorphism, Netflix Dark Theme
Dataset	TMDB 5000 Movies (Kaggle)
Fonts	Inter (Google Fonts)
Icons	Font Awesome 6
📊 Dataset
The TMDB 5000 Movie Dataset includes:

5000 movies with metadata
Genres, keywords, overview
Cast & crew information
Ratings, popularity, budget, revenue
Download from: https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata

🖥️ Screenshots
Homepage
Animated hero section with particle effects
Featured movies grid
Trending horizontal scroll
Top rated section
AI recommendation widget
Movie Detail
Movie metadata, rating, cast
Budget & revenue stats
AI "Find Similar Movies" button
Related movies grid
Search Page
Real-time autocomplete
Genre filter pills
Results grid with animations
🤝 Contributing
Fork the repository
Create your feature branch: git checkout -b feature/amazing-feature
Commit your changes: git commit -m 'Add amazing feature'
Push to the branch: git push origin feature/amazing-feature
Open a Pull Request
📄 License
This project is licensed under the MIT License.

👤 Author
MayaFlix - Built with ❤️ By Bismaya Guruprasad Panda

<div align="center">
🎬 Happy Movie Watching with MayaFlix!

If you found this helpful, please ⭐ the repository!

</div> ```
# 🎬 Content-Based Movie Recommendation System

<p align="center">
  <b>A Machine Learning project that recommends similar movies using Content-Based Filtering, TF-IDF Vectorization, and Nearest Neighbors.</b>
</p>

<p align="center">

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green?logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Numerical-blue?logo=numpy)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange?logo=scikitlearn)
![License](https://img.shields.io/badge/License-MIT-red)
![Status](https://img.shields.io/badge/Status-Completed-success)

</p>

---

# 📑 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Dataset](#dataset)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Project Workflow](#project-workflow)
- [Recommendation Method](#recommendation-method)
- [Sample Recommendation](#sample-recommendation)
- [Results](#results)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Future Improvements](#future-improvements)
- [Skills Learned](#skills-learned)
- [License](#license)
- [Author](#author)

---

<a name="overview"></a>
# 📌 Overview

Choosing a movie from thousands of available titles can be challenging. This project builds a **Content-Based Movie Recommendation System** that suggests similar movies based on their genres.

The recommendation engine uses **TF-IDF Vectorization** to convert movie genres into numerical features and **Nearest Neighbors (Cosine Distance)** to identify similar movies. The project also includes **Exploratory Data Analysis (EDA)** to understand rating patterns, genre distribution, and user activity.

---

<a name="features"></a>
# ✨ Features

- Content-Based Movie Recommendation
- TF-IDF Vectorization
- Nearest Neighbors Algorithm
- Exploratory Data Analysis (EDA)
- Rating Distribution Analysis
- Genre Distribution Analysis
- Movie Release Trend Analysis
- User-Movie Ratings Heatmap
- Movie Similarity Search

---

<a name="tech-stack"></a>
# 🛠 Tech Stack

| Category | Tools |
|-----------|-------|
| Programming Language | Python |
| Data Analysis | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-Learn |
| Recommendation | TF-IDF, Nearest Neighbors |
| Dataset | MovieLens |

---

<a name="dataset"></a>
# 📂 Dataset

Dataset Used: **MovieLens**

Files:

```
movies.csv
ratings.csv
```

Dataset Statistics

| Item | Count |
|------|------:|
| Movies | 62,423 |
| Ratings | 25,000,095 |

> Note: user count isn't computed in the notebook yet. Add `df_rating['userId'].nunique()` and update this table with the real figure before publishing.

---

<a name="exploratory-data-analysis"></a>
# 📊 Exploratory Data Analysis

The following analyses were performed:

- ⭐ Rating Distribution
- 🎭 Genre Distribution
- 🎬 Top Rated Movies
- 📈 Most Popular Movies
- 📅 Movies Released Per Year
- 🔥 User-Movie Ratings Heatmap

---

<a name="project-workflow"></a>
# ⚙️ Project Workflow

```
MovieLens Dataset
        │
        ▼
Data Loading
        │
        ▼
Data Cleaning
        │
        ▼
Exploratory Data Analysis
        │
        ▼
Feature Engineering
        │
        ▼
TF-IDF Vectorization
        │
        ▼
Nearest Neighbors Model
        │
        ▼
Movie Recommendation
```

---

<a name="recommendation-method"></a>
# 🤖 Recommendation Method

The recommendation system follows these steps:

1. Load movie dataset
2. Clean movie genres
3. Convert genres into TF-IDF vectors
4. Build a Nearest Neighbors model using cosine distance
5. Search for similar movies
6. Return the Top-10 recommendations

---

<a name="sample-recommendation"></a>
# 📷 Sample Recommendation

Input

```python
recommend("Jumanji (1995)")
```

Output

```
🎬 Recommended Movies for 'Jumanji (1995)'

Old Man Khottabych (1956)
Alice Through the Looking Glass (2016)
The Snow Queen (1966)
Red Riding Hood (1989)
Brothers Lionheart, The (Bröderna Lejonhjärta) (1977)
NeverEnding Story III, The (1994)
Darby O'Gill and the Little People (1959)
Ruslan and Ludmila (1972)
Santa Claus: The Movie (1985)
```

> Add a screenshot or exported plot image here once available (see Project Structure note below).

---

<a name="results"></a>
# 📈 Results

- Built a Content-Based Movie Recommendation System using genre similarity.
- Processed over **62,000 movies** and **25 million ratings**.
- Generated Top-10 similar movie recommendations based on genre overlap (TF-IDF + cosine distance).
- Visualized rating patterns, genres, and release trends through EDA.

> No formal accuracy/relevance metric (e.g. genre-overlap score, precision@k) has been computed yet. Add one before claiming recommendation quality.

---

<a name="project-structure"></a>
# 📁 Project Structure

```
Movie-Recommendation-System/

│
├── data/
│   ├── movies.csv
│   └── ratings.csv
│
├── images/
│   ├── workflow.png
│   ├── rating_distribution.png
│   ├── genre_distribution.png
│   └── heatmap.png
│
├── notebooks/
│   └── Movie_Recommendation_System.ipynb
│
├── requirements.txt
├── README.md
└── LICENSE
```

> The `images/` folder above is a template. Export your actual matplotlib/seaborn plots as PNGs into this folder (e.g. `plt.savefig("images/rating_distribution.png")`) and embed them below with `![Rating Distribution](images/rating_distribution.png)` — don't reference image files that don't exist in the repo.

---

<a name="installation"></a>
# 📦 Installation

Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/Movie-Recommendation-System.git
```

Navigate to the project folder

```bash
cd Movie-Recommendation-System
```

Install dependencies

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook

```bash
jupyter notebook
```

> Replace `YOUR-USERNAME` above with your actual GitHub username before publishing.

---

<a name="usage"></a>
# ▶️ Usage

```python
recommend("Jumanji (1995)")
```

---

<a name="future-improvements"></a>
# 📈 Future Improvements

- Hybrid Recommendation System (content-based + collaborative filtering)
- Collaborative Filtering using the ratings data
- Streamlit Web Application
- TMDB API Integration for posters and metadata
- Personalized User Recommendations
- Model Deployment

---

<a name="skills-learned"></a>
# 📚 Skills Learned

- Python Programming
- Data Cleaning
- Exploratory Data Analysis
- Feature Engineering
- TF-IDF Vectorization
- Nearest Neighbors
- Recommendation Systems
- Data Visualization
- Machine Learning Workflow

---

<a name="license"></a>
# 📄 License

This project is licensed under the **MIT License**.

---

<a name="author"></a>
# 👨‍💻 Author

**Nithish Kumar**

🎓 M.Sc. Data Science

**Skills:** Python • SQL • Power BI • Machine Learning

- GitHub: https://github.com/nithishkumarx2004-cell


> Replace `YOUR-USERNAME` and `YOUR-PROFILE` with your actual links before publishing.

---

## ⭐ Support

If you found this project useful, please consider giving it a **⭐ Star** on GitHub.

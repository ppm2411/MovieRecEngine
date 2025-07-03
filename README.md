# 🎬 Movie Recommendation System

This project is a **content-based movie recommendation system** that suggests similar movies based on user-selected input. The system leverages movie metadata such as genres, keywords, cast, crew, and more to recommend movies that are alike.

## 🔍 Key Features

- Content-based filtering using cosine similarity
- Recommendation based on movie metadata: genre, overview, cast, director, etc.
- Cleaned and merged movie data from multiple sources (e.g., TMDB)
- Fast and intuitive recommendations via precomputed similarity matrix

## 🧠 How It Works

1. Load and preprocess the movie metadata.
2. Combine important text features like overview, genre, cast, etc.
3. Vectorize the combined features using **TF-IDF** or **CountVectorizer**.
4. Compute **cosine similarity** between all movie vectors.
5. Recommend top N similar movies for a given input movie.

## 🧪 Example Output

If the user inputs **"The Dark Knight"**, the system might recommend:
- Batman Begins
- The Prestige
- Inception
- The Dark Knight Rises
- Man of Steel

## 📊 Technologies Used

- Python
- Pandas, NumPy
- Scikit-learn
- NLTK (for optional text preprocessing)
- Streamlit (for interface, if applicable)

## 📁 Dataset

Used The Movie Database (TMDb) dataset with fields like:
- `title`, `overview`, `genres`, `keywords`, `cast`, `crew`, etc.

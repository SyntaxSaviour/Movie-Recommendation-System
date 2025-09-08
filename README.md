# 🎬 Movie Recommendation System (Content-Based)

## 📌 Overview
This project is a **Content-Based Movie Recommendation System** built using the [TMDB Movie Metadata dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata).  
It recommends movies similar to a given movie by analyzing metadata such as **genres, keywords, cast, director, and overview**.



## 🚀 Steps Implemented
1. **Load Dataset** → `tmdb_5000_movies.csv` and `tmdb_5000_credits.csv`  
2. **Preprocessing** → parsed JSON-like fields, handled missing values, created a combined *"soup"* of features  
3. **Vectorization** → applied **TF-IDF** to convert text into feature vectors  
4. **Similarity Measure** → computed **Cosine Similarity** to find the most similar movies  
5. **Recommendation Function** → takes a movie title as input and outputs the **Top 5 most similar movies**



## 🛠️ Tech Stack
- **Python**
- **Pandas**
- **Scikit-learn**
- **NumPy**


## 🎯 Results
Example queries and top recommendations:  

- **Avatar** → Aliens, Star Trek Into Darkness, Predators  
- **Spectre** → Skyfall, Quantum of Solace, Casino Royale  
- **Pirates of the Caribbean: At World's End** → Other Pirates movies at the top  



## 📂 How to Run
1. Download the dataset from Kaggle and place the files inside a folder named **`data/`**:
   ```tmdb_5000_movies.csv```
   ```tmdb_5000_credits.csv```
2. Run the Jupyter Notebook or Kaggle Notebook cells step by step.  
3. Use the function:
   ```bash
   recommend("Avatar", n=5)
   ```

## ✅ Future Improvements

- Add Collaborative Filtering if user ratings are available
- Experiment with Word Embeddings or Transformers for semantic similarity
- Build a simple Streamlit Web App for interactive recommendations

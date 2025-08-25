# 🎬 MovieLens Recommender System

## 1. Project Overview
This project demonstrates how to build and evaluate a movie recommendation system using the [**MovieLens dataset**](https://www.kaggle.com/datasets/prajitdatta/movielens-100k-dataset/discussion?sort=hotness).  .  
It covers the full pipeline: data preprocessing, exploratory analysis, baseline models, collaborative filtering, and matrix factorization approaches (SVD).  
The goal is to compare different techniques and provide a unified recommendation API with ranking metrics evaluation.

---

## 2. Data Preprocessing
Implemented in **`Notebooks/DataReady.ipynb`**  
- Load raw MovieLens datasets (ratings, movies, users).  
- Convert timestamps and perform sanity checks.  
- Explore missing values and clean movie metadata.  
- Join ratings with movies to build a rich dataset.  
- Export cleaned datasets for analysis and modeling.  

---

## 3. Data Analysis
Implemented in **`Notebooks/MovieLens Data Analysis.ipynb`**  
- **Ratings distribution**: Explore how users rate movies.  
- **User activity analysis**: Identify highly/lowly active users.  
- **Movie popularity**: Most watched and most highly rated movies.  
- **Temporal analysis**: How ratings evolve over time.  
- **Genre analysis**: Popular genres and their rating trends.  
- **User demographics analysis**: Ratings across age groups and genders.  
- **Correlation analysis**: Links between popularity and ratings.  

---

## 4. Machine Learning (Recommendation Models)
Implemented in **`Notebooks/Modeling.ipynb`**  

### Baseline Models
- Global mean predictor.  
- Movie bias predictor.  
- User + Movie bias predictor.  

### Collaborative Filtering
- User–User and Item–Item CF (scikit-learn).  
- User–User and Item–Item CF (Surprise with cosine similarity).  

### Matrix Factorization
- Singular Value Decomposition (SVD) with Surprise.  

### Evaluation
- Metrics: RMSE, MAE.  
- Ranking metrics: Precision@K, Recall@K, NDCG.  
- Visualization of model performance.  

### Unified API
- Consistent interface for rating prediction.  
- Generate **Top-N personalized recommendations**.  
- Interactive widgets to explore **similar movies by title**.  

---

## 📊 Results (Sample)
- **SVD achieved the best performance** among tested models.  
- Example:  
  - `RMSE ≈ 0.93`  
  - `Precision@10 ≈ 0.71`  
  - `NDCG@10 ≈ 0.83`  

---
By **N**ourelden **H**any **E**lhakiem

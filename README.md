# Movie_Recommender_System

#  Movie Recommender System

##  Project Overview
This project builds a **content-based movie recommender system** using Python.  
It recommends similar movies based on textual metadata such as genre, cast, director, and plot keywords.  

The notebook demonstrates **end-to-end data science methodology** — from data preprocessing and feature engineering to similarity computation and evaluation.

---

##  Objective
To develop a **recommendation engine** that suggests movies similar to a user-selected film.  
This can be extended to streaming platforms or personal entertainment dashboards for better content discovery.

---

##  Methodology

### 1. Data Understanding
- Dataset contains movie titles and related attributes such as:
  - Overview / description
  - Cast
  - Crew
  - Genre
  - Keywords  
- Target task: Find and rank movies most similar to a given title.

### 2. Data Cleaning & Preprocessing
- Handled missing values in text fields.
- Combined textual columns into a single **metadata “soup”**.
- Removed punctuation and special symbols.
- Tokenized and lowercased all text.

### 3. Feature Engineering
- Applied **TF-IDF Vectorization** and **Count Vectorization** to convert text into numeric form.
- Constructed a **cosine similarity matrix** to measure movie-to-movie similarity.

### 4. Recommendation Logic
- Input: A movie title from the dataset.  
- Output: Top *N* movies ranked by cosine similarity.  
- Example:
  ```python
  recommend('Inception')

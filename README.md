# 🎵 Spotify Songs Popularity Prediction

**Author**: Neha Tiwari  
**Dataset**: [Audio Features and Lyrics of Spotify Songs (Kaggle)](https://www.kaggle.com/datasets/imuhammad/audio-features-and-lyrics-of-spotify-songs)  
**Objective**: Predict whether a Spotify song is popular based on its audio features and lyrical content  
**Problem Type**: Supervised Binary Classification  
**Tools**: Python, Pandas, Scikit-learn, NLTK, TF-IDF, Logistic Regression, XGBoost

---

## 📌 Project Overview

With music streaming dominating the audio industry, predicting what makes a song popular can be highly valuable to labels, artists, and platforms like Spotify. This project explores the use of **audio features** and **lyrics-based NLP techniques** to build a classification model for predicting whether a song will be popular or not.

---

## 📁 Dataset Summary

- **Source**: Kaggle  
- **Observations**: ~1,900 songs  
- **Features**:
  - Acousticness, Danceability, Energy, Instrumentalness, Liveness, Loudness, Speechiness, Tempo, Valence
  - Lyrics (text)
  - Target: `popularity` (binary – 1 for popular, 0 for not)

---

## 🔍 Key Steps in Workflow

### 1. **Data Cleaning & Feature Selection**
- Removed duplicates and irrelevant columns
- Engineered new features from audio metrics
- Cleaned lyrics (punctuation, stopwords, lowercasing)

### 2. **Natural Language Processing (Lyrics)**
- Tokenization using NLTK
- TF-IDF vectorization
- Combined text vectors with audio features

### 3. **Modeling**
- Tested multiple classifiers:
  - Logistic Regression
  - XGBoost Classifier
  - Random Forest
- Used GridSearchCV for hyperparameter tuning
- Performance metrics: Accuracy, Precision, Recall, F1 Score, AUC

---

## ✅ Results

- **Best Model**: XGBoost  
- **AUC**: ~0.92  
- **Top Predictors**: Energy, Danceability, Lyrics (TF-IDF), Loudness

---

## 📈 Visualizations
- Distribution plots for audio features
- Word clouds of common lyrics in popular vs. non-popular songs
- ROC and confusion matrix for model performance

---

## 📂 Repository Structure

- `HandsOn5_final.ipynb` — Full analysis and modeling notebook
- `README.md` — Project overview and details
- `data/` — (Not uploaded due to size; accessible from Kaggle)

---

## 📬 Contact

For queries or collaboration, connect on [LinkedIn](https://www.linkedin.com/in/neha-tiwarii/)

---

# 📰 Content-Based News Recommender System

This project implements a content-based filtering news recommendation system using the Microsoft News Dataset (MIND). It recommends articles to users based on their interests by analyzing text similarity using TF-IDF and cosine similarity.

---

## 📁 Project Structure

roject_root/
├── data/
│ └── news.tsv # Original raw news dataset
│ └── preprocessed_news.csv # Cleaned data with combined text
├── results/
│ └── similarity_scored_news.csv # Articles with similarity scores
│ └── sample_recommendations.csv # Top-N recommended articles
├── notebooks/
│ ├── 01_data_preprocessing.ipynb
│ ├── 02_user_profile_construction.ipynb
│ ├── 03_content_similarity.ipynb
│ └── 04_ranking_and_recommendation.ipynb
├── requirements.txt
└── README.md
How to Run the Project
Download the dataset from the MIND Kaggle page and save news.tsv in the data/ folder.

Run the notebooks in order:

01_data_preprocessing.ipynb: Loads and cleans the dataset, merges title and abstract.

02_user_profile_construction.ipynb: Defines user interests and creates a profile vector.

03_content_similarity.ipynb: Vectorizes articles and computes similarity with user profile.

04_ranking_and_recommendation.ipynb: Ranks and outputs top-N recommended articles.

Check the final recommendations in:

results/sample_recommendations.csv
 Techniques Used
TF-IDF (Term Frequency–Inverse Document Frequency)

Cosine Similarity

Text Preprocessing (lowercase, stopword removal, etc.)

Content-Based Filtering

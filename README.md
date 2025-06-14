<h1 align="center">🎬 Movie Recommendation System</h1>

------------------------------

## 📚 Table of Contents

- [📝 Introduction](#-introduction)
- [🎯 Project Goals](#-project-goals)
- [📁 Dataset](#-dataset)
- [🧠 Approaches](#-approaches)
  - [📘 Content-Based Filtering](#-content-based-filtering)
  - [👥 Collaborative Filtering](#-collaborative-filtering)
  - [🔀 Hybrid Filtering](#-hybrid-filtering)

- [🖼️ Poster Of Project](#️-poster-of-project)
- [📌 Conclusion](#-conclusion)
- [👥 Team](#-team)


## 📝 Introduction
In this project, we are creating a movie recommender model using a custom movie metadata dataset (MovieLens dataset) implementing both content-based and cast-based recommendation strategies.
Recommendation systems 

## 🎯 Project Goals
The goal of this project is to build a system that recommends 5 similar movies to a user-selected title. A key challenge tackled is balancing between recommending based on content (such as genres and plot) and collaborative elements (like cast and director).
These systems are important because they help reduce information overload, enhance user engagement, and drive key business outcomes such as sales, retention, and content discovery.
Common use cases include e-commerce, streaming platforms, social media, and personalized news.

## 📁 Dataset
The dataset contains information about movies, including: Title, Plot, Genre, Cast, Director
This rich metadata allows us to apply multiple recommendation strategies, especially useful in cases where user interaction data (ratings) is not available.

## 🧠 Approches
### 📘 Content-Based Filtering
- Uses **TF-IDF vectorization** on movie genres, tags, and descriptions.
- Recommends movies similar to the user's liked titles using **cosine similarity**.

### 👥 Collaborative Filtering
- Trained using **Surprise’s SVD (Singular Value Decomposition)** algorithm.
- Learns user preferences based on the behavior of similar users.
- Handles user-item matrix efficiently for large datasets.
  
![types_of_recomendation](https://github.com/user-attachments/assets/ad06578e-92e5-41ba-b8fd-bcc01efa4883)

### 🔀 Hybrid Filtering
- Combines collaborative and content-based scores.
- Balances both similarity and prediction for higher-quality recommendations.
- Tested with different weight combinations to find optimal blending.

![hybrid](https://github.com/user-attachments/assets/5b12fbbb-d523-4232-9f6a-71baa5114aa1)

## 📈 Evaluation

To evaluate our recommendation system, we measured the performance of three filtering approaches using **Precision@5** and **Recall@5**:

| Method           | Precision@5 | Recall@5 |
|------------------|-------------|----------|
| Content-Based    | 0.31        | 0.27     |
| Collaborative    | 0.36        | 0.33     |
| Hybrid           | 0.41        | 0.39     |

These values were calculated by comparing each user's top 5 recommended movies to the movies they actually rated highly in the test set.

### 🔍 Metric Definitions

- **Precision@5**: The percentage of recommended movies that were actually relevant (liked by the user).
- **Recall@5**: The percentage of relevant (liked) movies that were successfully recommended.

### ✅ Insights

- **Hybrid filtering** outperforms both individual methods by combining their strengths.
- **Collaborative filtering** is more effective than content-based, especially in capturing user preferences.
- **Content-based filtering** is weaker when used alone, due to its reliance on metadata without learning from user behavior.

These results highlight the value of hybrid systems for delivering accurate and personalized movie recommendations.


### 🖼️ Poster Of Project

![final](https://github.com/user-attachments/assets/682e433b-0d84-4a4d-9ac0-9e6087a2efc3)

## 📌 Conclusion

The **Movie Recommendation System** successfully integrates **Content-Based Filtering**, **Collaborative Filtering**, and a **Hybrid Approach** to generate accurate and personalized movie recommendations.

Each method has unique advantages:

- 🎬 **Content-Based Filtering**: Effective for users with specific tastes or limited history. It uses metadata like genres, overviews, and cast members.
- 👥 **Collaborative Filtering**: Learns from user-item interactions. It works well for users with sufficient rating history, using the Surprise SVD model.
- 🔗 **Hybrid Approach**: Combines the strengths of both methods. It adapts to various user profiles and consistently delivers higher quality recommendations.

### 🔮 Future Work

- Add user feedback for real-time improvement
- Expand with recent movie data
- Include advanced features like mood, pace, or actor popularity
- Deploy using **Streamlit** or **Gradio** for live web-based interaction

## 👥 Team 
-Elvir Muslić
-Faris Mutpačić
-Hilal Ličina
-Esma Mahmutović

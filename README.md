<h1 align="center">🎬 Movie Recommendation System</h1>

------------------------------
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
- 
![types_of_recomendation](https://github.com/user-attachments/assets/ad06578e-92e5-41ba-b8fd-bcc01efa4883)

### 🔀 Hybrid Filtering
- Combines collaborative and content-based scores.
- Balances both similarity and prediction for higher-quality recommendations.
- Tested with different weight combinations to find optimal blending.

![hybrid](https://github.com/user-attachments/assets/5b12fbbb-d523-4232-9f6a-71baa5114aa1)

### 🖼️ Poster Of Project

![final](https://github.com/user-attachments/assets/682e433b-0d84-4a4d-9ac0-9e6087a2efc3)


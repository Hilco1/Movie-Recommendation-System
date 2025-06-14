<p align="center">A hybrid approach combining Content-Based and Collaborative Filtering</p>

------------------------------
## 📝 Introduction
In this project, we are creating a movie recommender model using a custom movie metadata dataset (MovieLens dataset) implementing both content-based and cast-based recommendation strategies.
Recommendation systems 

## 🎯 Project Goals
The goal of this project is to build a system that recommends 5 similar movies to a user-selected title. A key challenge tackled is balancing between recommending based on content (such as genres and plot) and collaborative elements (like cast and director).
These systems are important because they help reduce information overload, enhance user engagement, and drive key business outcomes such as sales, retention, and content discovery.
Common use cases include e-commerce, streaming platforms, social media, and personalized news.

The dataset contains information about movies, including: Title, Plot, Genre, Cast, Director
This rich metadata allows us to apply multiple recommendation strategies, especially useful in cases where user interaction data (ratings) is not available.


Content-Based Filtering: Recommends movies based on metadata such as genre, director, cast, and plot keywords.

Collaborative Filtering: Optionally uses user ratings and interactions (if provided) to improve recommendations.

Similarity Metrics: Implements cosine similarity on TF-IDF vectors for textual features.

Tunable Weighting: Allows combining different recommendation strategies (e.g., 50% content + 50% cast-based similarity).



![types_of_recomendation](https://github.com/user-attachments/assets/ad06578e-92e5-41ba-b8fd-bcc01efa4883)




# News-Recommendation-System

# 📰 Python: Building a News Recommendation System

This was the final project for my Masters in Business Analytics, which I conducted in a team of 5 people.

## Introduction
**👩🏻‍💼 THE SITUATION** 

In today's fast-paced and information-rich world, staying updated with relevant news is crucial for individuals and organizations alike. However, the sheer volume and diversity of news content available can often make it challenging to find articles that align with one's interests and preferences. To address this issue, recommender systems have emerged as powerful tools for delivering personalized news recommendations to users. This project explores the development of a news recommender system for a ficticious news company Sokovia News.

**✏️ THE OBJECTIVE**
The objective of this project is to build a news recommendation system for Sokovia News. The recommender system should take into consideration user preferences, behaviors, and historical data to deliver personalized news recommendations, thereby enhancing user experience and engagement.

**🛠 THE TOOLS**

This project uses the [MIND dataset](https://msnews.github.io/) and was conducted in Python, mainly using Jupyter notebooks. The ouptuts of the project include various Jupyter notebooks, a report and a presentation.
		
## Project
The project covers preliminary data analysis, data preparation, and feature engineering for building the following recommender system models:
- **Baseline model:** random recommender
- **Model 1: frequency & category based recommendations:**
  - Provides article recommendations based on popularity and user-selected categories. Intended for new users who have read five or fewer articles, it suggests the 10 most frequently read articles within their chosen categories.
**- Model 2: content-based filtering:**
  - A content-based recommender that suggests articles to a user based on their similarity to previously read articles. There are three versions of the model: one using term frequency inverse document frequency (TF-IDF), one using the TransE embeddings, provided in the MIND dataset, and a third one using word embeddings extracted using the GloVe4 model
**- Model 3: collaborative & content-based filtering**
  - Combines user-to-user collaborative filtering with content-based recommendation. It compares articles read by a user with those read by others to identify the top 5 similar users. Then, it filters out read articles to create a reduced news dataset. Finally, it recommends the top 10 similar articles from this dataset. Variations include **TF-IDF, TransE, GloVe embeddings, and Google Word2Vec embeddings**, each with distinct embedding sources.

In addition, the project evaluates all mentioned recommendation models, discusses their business application and potential ROI, addresses model deployment considerations, and explores future improvements.

## 📚 Conclusion
The project identifies Model 3 (collaborative & content-based filtering) as the most effective recommendation model, showcasing its potential as a proof-of-concept with a tenfold improvement over the random baseline model. While it falls short of the highest-performing models on the official MIND GitHub, which use pre-trained deep neural networks, it is feasibible for business application, especially considering the absence of a current recommendation system at Sokovia News. Importantly, our models were developed from scratch, affording Sokovia News greater control and customization opportunities compared to pre-trained neural networks. This adaptability is key for future growth and refinement of the recommender system.

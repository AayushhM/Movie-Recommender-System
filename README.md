
# Sentiment Analysis and Movie Recommendation System


This repository contains two separate but related projects: Sentiment Analysis and Movie Recommendation System. Both projects are implemented in Python and utilize several NLP and machine learning libraries.

Sentiment Analysis
The Sentiment Analysis project is a classification task to determine the sentiment of a given comment as positive or negative based on its content. The machine learning algorithm used for this task is Naive Bayes, specifically the Multinomial Naive Bayes algorithm. This algorithm is a probabilistic algorithm that makes classifications based on Bayes' Theorem and is particularly suited for text data, modeling the probability of occurrence of each word in a document given a class. The reason for using Naive Bayes is its simplicity and effectiveness in text classification tasks, especially when the size of the training data is small. Additionally, Naive Bayes is computationally efficient and can handle a large number of features, making it a good choice for sentiment analysis.

The code uses the TfidfVectorizer to transform the comments into numerical features, and the trained Naive Bayes model is saved in a pickle file for future use. The accuracy of the model is evaluated using the accuracy score.

Movie Recommendation System
The Movie Recommendation System is a content-based filtering approach where the similarity between the movies is calculated using the cosine similarity between the movie descriptions (the combination of the movie's title, overview, genres, and cast details). The movie details are fetched from IMDB and stored in a csv file. The data is pre-processed and transformed using CountVectorizer and the cosine similarity calculation is done using the sklearn library. The recommendation model and the transform object (CountVectorizer) are stored in the pickle files "nlp_model.pkl" and "tranform.pkl" respectively, which are loaded into the application at the start.

The user interface of the application is created using HTML, CSS, and JavaScript and is hosted by the Flask framework. The user can search for a movie, and the application will return the top 10 most similar movies based on the content-based filtering approach. The movie details and recommendation list are displayed on the web page.





## API Reference

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `tmdb.api_key` | `string` | b5ea724214b36ca7aba111b400ffc1f9 |




## Deployment

The app has been deployed on Railway: https://movie-recommender-system-production-2b6d.up.railway.app/

## Screenshots

![App Screenshot](https://user-images.githubusercontent.com/13918412/218334281-9959323e-7358-4512-911d-245a9096d6c2.jpeg)


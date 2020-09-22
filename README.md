# Anime-Recommender-System
A hybrid recommendation system based on the user preferences and in animes he previously watched and rated.

For this project I used the animelist databased provided by https://www.kaggle.com/azathoth42/myanimelist, where I used the cleaned version of the dataset (users_cleaned, animelists_cleaned, anime_cleaned) to create a recommendation system for the user. I used KNN with cosine-similarity for the content-based recommendation step and SVD for the collaborative-filtering step. The values of similarity I obtained in the content-based step work as a value of of "how much the user's taste is similar to this anime", and I get the average between these values and the predicted ratings obtained in the collaborative-filtering algorithm to get a list of the best recommendations for the user.

I chose to not use the surprise library since I was studying the algorithms and I wanted to see if I was applying them correctly.

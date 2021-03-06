# Movie Recommendation Function

![1_N0-ikjPv4RUVvS-6KCgLPg](https://user-images.githubusercontent.com/76961031/118359877-4f3efe80-b57d-11eb-8bf2-3cfa29d11bd5.jpeg)

I have made two collaberative filtering film recommendation functions using the movielens 250k dataset which can be downloaded here: https://grouplens.org/datasets/movielens/. 

## Overview

The **first** uses a simple similarity score between groups of users:

| movieid     | user_rating | your_rating |
| ----------- | ----------- | ----------- |
| 5546      | 3       |4       |
| 4432   | 2        | 2  |


x = (user_rating - your_rating)/total_user_ratings  -----> By doing this, the number of films matching your given number of films is taken into consideration.

movie_difference = pow(x,2)            

similarity = sum(movie_difference for each movie)


By calculating similarity in this way, higher differences between film ratings of different users are penalised more and smaller differences are penalised less. we also never deal with negative numbers this way.


The **second** uses the SVD algorithm which is trained on the movielens dataset.


Please feel free to download the notebook and see which films either recommender gives you!

# Movie Recommendation Function


I have made two collaberative filtering film recommendation functions. 

The first uses a simple similarity score between groups of users:

| movieid     | user_rating | your_rating |
| ----------- | ----------- | ----------- |
| 5546      | 3       |4       |
| 4432   | 2        | 2  |


$$\frac{(user_rating - your_rating)}{2}$^2$

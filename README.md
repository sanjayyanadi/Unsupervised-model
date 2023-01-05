# Unsupervised-model
# Books Recommendation Project
**Problem Description:**
A Book Recommendation System which recommends the users a selection of books based on their interests.
#Algorithms Implemented:

***Recommendation Based on Popularity:***
* Popular in the Whole Collection: We have sorted the dataset according to the total ratings each of the books has received in non-increasing order and then recommended the top n books.
* Books by the Same Author, Publisher of the Given Book Name: For this model, we have sorted the books by rating for the same author and publisher as the given book and recommended the top n books.
* Yearly Bestsellers: This is the most basic model, in which we have grouped all the books published in the same year and recommended the top-rated book each year.

***Recommendation using an Average Weighted Rating***
We have calculated the weighted score using the below formula for all the books and recommended the ones with the highest score.
 t/(t+m)a + m/(m+t)c = score
 where,
It represents the total number of ratings received by the book.
m represents the minimum number of total ratings considered to be included.
a represents the average rating of the book and,
c represents the mean rating of all the books.

***User-Item Collaborative Filtering Recommendation***
The collaborative filtering recommendation system works by considering user ratings and finding cosine similarities in ratings by several users to recommend books. To implement this, we took only those books' ratings that had at least 50 in total.

***Correlation-Based Recommendation***
For this model, we have created the correlation matrix considering only those books that have total ratings of more than 50. Then a user-book rating matrix is created. Top books are recommended for the correlation matrix input book.

***Recommendation Based on Neighbors***
To train the Nearest Neighbors model, we have created a compressed sparse row matrix, taking ratings of each book from each user individually. This matrix is used to train the "nearest neighbors" model and then to find the n nearest neighbors using the cosine similarity metric.

***content-based recommendation***
This system recommends books by calculating similarities in book titles. For this, TF-IDF feature vectors were created for unigrams and bigrams of book titles; only those books' data that have at least 80 ratings have been considered.

 ***Recommendation for a Hybrid Approach (Collaborative and Content)***
 A hybrid recommendation system was built using the combination of both content-based filtering and collaborative filtering systems. A percentile score is given to the results obtained from both content and collaborative filtering models and is combined to recommend the top 10 books.
 
 
 
 ### ***conclusion:***
***We analysed a dataset in various scenarios for this project and came up with some recommender systems based on a few features:
This recommender system works extremely well for this dataset. When we search for a book, all of the recommenders list matches almost 70% of the time, which is extremely impressive.***


***I would appreciate any suggestions.***

***thank you.***

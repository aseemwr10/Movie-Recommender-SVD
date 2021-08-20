# Movie-Recommender-SVD
Course project to build a recommendation system using Matrix Factorization

The dataset is from GroupLens containing 1M ratings from 6040 users for 3706 movies.

Collaborative filtering is a method of making automatic predictions (filtering) about the interests of a user by collecting preferences or taste information from many users (collaborating). 

User-Based Collaborative Filtering
Finds similar users based on past ratings, then recommends items based on weighted sum of item rating from similar users. 
Removing user bias is an important step.

Item-Based Collaborative Filtering
Finds similar items based on user ratings, then recommends based on weighted sum of ratings of similar items by the user.

Matrix factorization is a class of collaborative filtering algorithms used in recommender systems. 
Singular Value Decomposition (SVD) is a Matrix Factorization technique which reduces our Ratings Matrix (R) as follows:
R = UΣVT
Where U and V are orthogonal matrices representing the relations between the users and latent features and items and latent features respectively. Σ is a diagonal matrix representing the strength of each latent feature.
We use the dot product of these three matrices to fill in the unknown ratings and make recommendations.

Use Cases:
Make User Recommendations - Calculate User Ratings using the recreated Ratings matrix build using SVD and filter out movies the User has already rated
Identify Similar Movies - Use the Item Latent Features matrix and get similar movies based on any chosen similarity metric like Pearson correlation

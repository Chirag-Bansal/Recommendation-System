# Recommendation-System
Created a recommendation system based on collaborative item filtering. Based on the past history of the user we wish to recommend products to the user similar to the ones he has already bought. From the dataset we create a user-item matrix which conatins information about every user's purchase history including the times that each item was bought.

## K-Nearest Neighbours
For each of the user we find the list of items. Each item in this list has some items similar to it. So based on which we sort the candidate items and return the top recommendations

### Cosine Similarity
We use cosine similarity for comparing the two vectors. Cosine similarity measures the similarity between two vectors of an inner product space. It is measured by the cosine of the angle between two vectors and determines whether two vectors are pointing in roughly the same direction.

### Jaccard Index
The Jaccard index, also known as the Jaccard similarity coefficient, is a statistic used for gauging the similarity and diversity of sample sets.

#### Differences between Cosine similarity and Jaccard Index
The key difference between these two is that cosine similarity has a vector for each user with values equal to number of times a user bought that product whereas jaccard only uses set of items. The information about hpw many times each product is bought is lost. Which is also shown in the results - Cosine similarity gives a precision of 0.68 whereas Jaccard Index gives a similarity of 0.55

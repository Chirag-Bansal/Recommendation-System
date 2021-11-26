# Recommendation-System
Created a recommendation system based on collaborative item filtering. Based on the past history of the user we wish to recommend products to the user similar to the ones he has already bought. From the dataset we create a user-item matrix which conatins information about every user's purchase history including the times that each item was bought.

## K-Nearest Neighbours
For each of the user we find the list of items. Each item in this list has some items similar to it. So based on which we sort the candidate items and return the top recommendations

### Cosine Similarity
We use cosine similarity for comparing the two vectors, which is defined as follows:
\begin{equation}
\cos ({\bf t},{\bf e})= {{\bf t} {\bf e} \over \|{\bf t}\| \|{\bf e}\|} = \frac{ \sum_{i=1}^{n}{{\bf t}_i{\bf e}_i} }{ \sqrt{\sum_{i=1}^{n}{({\bf t}_i)^2}} \sqrt{\sum_{i=1}^{n}{({\bf e}_i)^2}} }
\end{equation}

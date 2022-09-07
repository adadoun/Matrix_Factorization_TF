# Description

This project aims to build a recommender system for movies [Movielens data](https://grouplens.org/datasets/movielens/100k/) based on [Matrix Factorization Method](https://datajobs.com/data-science-repo/Recommender-Systems-[Netflix].pdf)

The data analysis was made using [pandas](https://pandas.pydata.org/), and the Matrix factorization implementation was done with [Tensorflow api](https://www.tensorflow.org/)

As input, we have the interaction matrix where each element of the matrix represent the rating of a user i for the item j, see matrix bellow :

    
|   |i1 |i2 |i3 |
|---|---|---|---|
|u1 | 1 | 2 | 2 |
|u2 | 5 | 2 |   |
|u3 | 3 | 3 | 4 |
|u4 | 4 |   | 3 |


As output, we obtain the latent representation of each user and item (see the paper)

Finally, in order to compute the rating for the pair (i, j), we only have to compute the dot product between latent vector of the user i and item j.

We evaluate the performance of the algorithm using RMSE metric as in the paper.

You will find the implementation + Data Analysis + Algorithm Evaluation in the [notebook](https://gitlab.eurecom.fr/amadeus/matrix_factorization/blob/master/Matrix_Facto_TF.ipynb)
# K-Means
<i>This program was part of an assignment for CSE 5334( Data Mining) at University of Texas at Arlington</i>
Give a star if using this code :)
<br><b>Function execution :</b>

1. The 2D Gaussian multivariate was generated using ​ np.random.multivariate_normal(mean1,
Sigma1, 500).T.
2. The centers and number of clusters for the sub problems are hard coded
<img src="https://github.com/adityadas8888/k-means/blob/master/im1.png" width="600"/>

They can be changed/swapped out by the values required. (Line 32:34)

3. The numpy arrays concatenated and stored in pandas Dataframes.
4. The centers are then stored in a dictionary called centroids. These are dynamic and can change
according to the number of centers given.(Max centers supported is 6)
5. The centers are then assigned to the generated dataset using center_assignment() function.
The l2 norm is found and the least distance center is assigned to the point.
6. After assignment of centers, the old centers are copied using deepcopy and a loop runs until the
difference between the old and new loops is less than 0.001 or the number of iterations reach
10000.
7. The loop updates the new centers found using the mean and assigns the new centers.
8. Finally the following graphs were generated
<img src="https://github.com/adityadas8888/k-means/blob/master/im2.png" width="600"/>
<img src="https://github.com/adityadas8888/k-means/blob/master/im3.png" width="600"/>
The above figure is 2 clustering 2 center graph.
The centers are shown in the snippet.
The number of iterations are 29.(30 including the first assignment)
<img src="https://github.com/adityadas8888/k-means/blob/master/im4.png" width="600"/>
<img src="https://github.com/adityadas8888/k-means/blob/master/im5.png" width="600"/>
The above figure is 4 clustering 4 center graph.
The centers are shown in the snippet.
The number of iterations are 19.(20 including the initial assignment)

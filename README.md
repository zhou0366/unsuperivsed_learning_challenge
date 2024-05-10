# Crypto Clustering Challenge

In this challenge, we will be following the instructions laid out in the starter code Jupyter Notebook. KMeans, PCA, and StandardScalar from sklearn will be used to cluster data.

First, the data is imported into a dataframe.

![image](https://github.com/zhou0366/unsupervised_learning_challenge/assets/22827830/e3346338-0e2b-4b67-a0a0-fa43a82e4cf7)


Summary statistics of the data are shown.

![image](https://github.com/zhou0366/unsupervised_learning_challenge/assets/22827830/611c5368-9677-4539-9494-7538c77e49c9)


The data is plotted for each coin

![image](https://github.com/zhou0366/unsupervised_learning_challenge/assets/22827830/a6f890df-4c3d-4b19-bfe1-440c8fbc3c51)


The data is then scaled using StandardScalar and saved to a new dataframe.

![image](https://github.com/zhou0366/unsupervised_learning_challenge/assets/22827830/734ca94f-09af-4cb0-b087-9729d54ca1ac)


A K means model and inertia list are generated. The results are used to create the following elbow curve. We can see that the best k value is 4.

![image](https://github.com/zhou0366/unsupervised_learning_challenge/assets/22827830/87d5bc5c-2ac1-4c81-80dc-89864010f6ec)


A k means model is created with 4 clusters. The model prediction is applied to the scaled crypto data. Cluster numbers are added to a copy of the scaled crypto dataframe.

![image](https://github.com/zhou0366/unsupervised_learning_challenge/assets/22827830/5232df2f-071f-418b-b11b-889fbd9921b3)


The dataframe with clusters is used to plot price change in 7 days vs price change in 24 hours color-coded by assigned cluster.

![image](https://github.com/zhou0366/unsupervised_learning_challenge/assets/22827830/8a1e8b32-a218-4dce-ad8d-e097c8d7af05)


PCA is applied with three columns. The result was applied to the crypto data and added to a new dataframe.

![image](https://github.com/zhou0366/unsupervised_learning_challenge/assets/22827830/2601fd2c-caaa-465c-a4c1-e9071a8272f7)


Another elbow curve is created. The best K value appears to be 4 again.

![image](https://github.com/zhou0366/unsupervised_learning_challenge/assets/22827830/4d655095-b0d0-4552-b1b9-2a58577f8bcc)


The PCA data is clustered using K means with 4 clusters.

![image](https://github.com/zhou0366/unsupervised_learning_challenge/assets/22827830/9f868e6b-cd66-44d2-b528-b72dade1912f)


The clustered PCA data is plotted.

![image](https://github.com/zhou0366/unsupervised_learning_challenge/assets/22827830/d7f6430a-eee8-4b41-9dff-0ea0fa571ccf)


Elbow curves and clustered plots are compared side by side. Impact of fewer features is that the two larger clusters for both are tighter. There are still two clusters with one point each in both.

![image](https://github.com/zhou0366/unsupervised_learning_challenge/assets/22827830/2b6db126-fcc7-4836-ac01-2ac7b05df194)

![image](https://github.com/zhou0366/unsupervised_learning_challenge/assets/22827830/b52857af-0cdb-4602-ab2c-7f54d3c49f57)

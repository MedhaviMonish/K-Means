#Clustering
Clustering is considered an unsupervised learning method, where the machine is provided data without the target labels and it 
tries to learn the differences and similarity among them.

## K-Means

K-means is one of the clustering methods that runs iteratively until the desired numbers of clusters are found.
The user will input the total number of clusters(k) to be found.


K-means is a centroid based technique. It takes total number of clusters as user input.
And tries to increase intra-cluster similarity and decrease inter-cluster similarity 

  Start(Total cluster k)
          |
          |
       Centroid <-------------
          |                   |
          |                   |
   Distance of each           |
   data with centroid         |
          |                   |
          |                   ^
    Grouping based on         |
    proximity to centre       |
          |                   |
          |                   |
      Data Moved              |
    to other group  --->---- Yes 
          |
          | No
         End


###Hand Witten digits
We will be using the hand written digits dataset provided by sklearn it has 1797 data sample of hand witten digits,
each one is image of size 8x8. But Since it has 64 attribute/dimensions (i.e. 8 * 8), we will be reducing it's dimension to 2 so that
it will be easier to display them on 2D graph. For this we need to introduce Principal component analysis (PCA)

##Principal component analysis https://en.wikipedia.org/wiki/Principal_component_analysis

Principal component analysis is an algoithm that reduces the dimension of data. For example if you have a data that has 784
attributes(i.e. dimension) then you can represent it in lower dimension like using only 10 attributes or even less. This method is not
really effective, it has high vaiance. We can use better methods like Variational Autoencoders but its too advanced to be used here, so
we will be working with PCA only.


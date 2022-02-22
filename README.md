# kNN classifier

# Task 1: Obtain dataset
  - This task is done by taking in the MNIST dataset, It is a dataset of 60,000 small square 28×28 pixel
gray scale images of handwritten single digits between 0 and 9.This dataset consists of both images and
labels.The functions LoadMNIST or LoadMNISTLables and LoadMNISTImages are used to read
both images and labels.

# Task 2:Build a kNN classifier
  - For this task a Mat lab function namely KNN is created which takes in the following arguments such
as a dataset which is divided into Training images, Training labels, Test images, Test labels and an integer
k.
  - This function checks the number of arguments received and returns an error if Required number of
arguments are not received and also checks that the number of columns of both first and second matrix are
equal or not. After the necessary conditions have been met Euclidean distance is calculated.
  - The straight line distance between two vectors using the Euclidean distance formula is calculated. It is
calculated as the square root of the sum of the squared differences between the two vectors.
  - Where x1 is the first row of data, x2 is the second row of data and i is the index to a specific column.With
Euclidean distance, the smaller the value, the more similar two records will be. A value of 0 means that
there is no difference between two vectors.
  - Next, Nearest neighbors are calculated. Neighbors for a new piece of data in the data set are the k
closest instances, as defined by our distance measure. To locate the neighbors for a new piece of data
within a data set distance is calculated between each record in the data set to the new piece of data. Once
distances are calculated, training data set is sorted by their distance to the new data depending on the
value of k.
  - Predictions are made using most similar neighbors collected from the training data set. In the case of
classification, we can return the most represented class among the neighbors.

# Task 3: Test the kNN classifier
- The results of the knn classifier are measured by calculating accuracy.

# Classification-of-noisy-MINST-dataset

This repository stores a [jupyter notebook](https://github.com/asonnellini/Classification-of-noisy-MINST-dataset/blob/main/Andrea%20Sonnellini%20-%20report%20ANN%20assignment.ipynb) with the analysis that I performed as part of the Assignment of the Artificial Neural Network class at DSTI Spring cohort 2020.

The target of this assignment was to build and train a model to classify images stored in a given dataset.
More specifically the images were a noisy version of the MINST dataset and the assignment gave us a dataset train.csv with labeled images and another dataset test.csv with unlabeled images.

The overall strategy of my work was to:

  - split the training.csv dataset (with labeled images) into a training and test set 
  - train a model on the training set 
  - evaluate its accuracy on the test set
  - try to improve the model performances adopting more sophisticated approaches in a "phased" way (i.e. from the simplest to the more sophisticated approach)
  - eventually select the model with the best performance on the test set
  - train the selected model on the whole dataset train.csv
  - predict labels on the unlabled dataset test.csv

Below a list of algos that I tested:

  - SVM with and without PCA
  - A simple CNN with 2 convolutional layers 
  - Transfer learning with VGG16 and its weights from ImageNet 
  - A CNN with 4 convolutional layers 

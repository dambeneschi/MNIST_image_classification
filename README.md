**Image classification of the MNIST dataset**

This repository hosts the machine learning models used to classify the hand-written digit images of the MNIST dataset (42 000 images).
The model has been created to participate to the corresponding Kaggle "Getting Started" competition "Digit Recognizer": https://www.kaggle.com/c/digit-recognizer.


*Best scores obtained: 97% of accuracy with SVC(), 98% with Convolutionnal Neural Network*



The notebooks contain respectively the following steps:

**EDA, Pretreatment , simple models**
- The Exploratory Data Analysis goes through a numerical an vizual analysis of the dataset in order to identify the relevant preprocessing and modelisation strategies.

- The pre traitement consists in a first reduction of the number of pixels by removing from the set the pixels whose intensities never change over the 42 000 images (always black or white pixel within the 28x28 pixels images). The ne training set is called train_changing_pixels_df.csv

- Simple classifiers have been picked-up in order to get their performances on randomly sampled data, in order to comapre them and do the first submissions. It features:
- k-NN
- Linear Discriminant Analysis
- Support Vector Machines (SVC, Linear SVC)
- Classification Tree



**Clustering & Dimension Reduction with visualizations**

- The unsupervised clustering of the data allows to see how the t-SNE model groups naturally the data together
- The Dimension Reduction using PCA is carried out with graphs in order to choose the right number of PCA features to keep for further computing


**Deep Learning**
- A comparison between a simple neural network and a convolutional neural network, using Keras & Tensorflow on GPU
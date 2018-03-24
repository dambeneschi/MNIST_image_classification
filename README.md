**Image classification of the MNIST dataset**

This repository hosts the machine learning models used to classify the hand-written digit images of the MNIST dataset (42 000 images).
The model has been created to participate to the corresponding Kaggle "Getting Started" competition "Digit Recognizer": https://www.kaggle.com/c/digit-recognizer.


The notebook contains the following steps:
**Exploratory Data Analysis**
The EDA goes through a numerical an vizual analysis of the dataset in order to identify the relevant preprocessing and modelisation strategies.


** Preprocessing **
The preprocessing consists in 2 steps with the goal to simplify the features and reduce the computing cost of the classifiers:
- Regarding the distribution of the intensities of the pixels, turns the pixels intensity into binay variables (0 for black, 1 for white)
- Remove from the set the pixels whose intensities never change over the 42 000 images (always black or white pixel within the 28x28 image)

The preprocessing created a simplified train set, containing 670 instead of 784 features, with binary values rather than int value between 0-255.


** Simple models **
Simple classifiers have been picked-up in order to get their performances on random sample data, in order to comapre them and do the first submissions. It features:
- k-NN
- Linear Discriminant Analysis
- Support Vector Machines (SVC)
- ...
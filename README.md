# Fruit_Classification
Personal project that trains various classifiers to identify several types of fruits in a data file,  and evaluates the accuracy of each classifier.

The code is broken down into several parts, with two distinct parts: 
## Part 1: Visualization and graphing of data to understand the data's contents

1. Printing out the head of the file (i.e. the total number of fruits and the number of features evaluated)
2. Printing out the number of types of fruits
3. Plotting a bar graph of each type of fruit (Note that for this step I had trouble using seaborn's countplot and instead used matplotlib's histogram to display the count of each type of fruit
4. Plotting a box plot to better visualize the distribution of each type of fruit
5. Plotting a histogram of each type of fruit
6. Plotting a scatter matrix of each feature

## Part 2: Utilization of machine learning algorithms to classify the fruits 
1. Creation of training and testing sets
2. Building of various models for machine learning algorithms
- Logistic Regression
- Decision Tree
- K-Nearest Neighbors
- Linear Discriminant Analysis
- Gaussian Naive Bayes
- Support Vector Machine
3. Plotting of Decision Boundary of the k-NN classifier

The main libraries that are required for this project are matplotlib, numpy, pandas, collections, seaborn, pylab, and matplotlib.pyplot for the first part, and sci-kit learn for the second part. 

More things to note are that I did have trouble running the program on WSL distribution with Python 3.10.8. The program only worked when I used Python 3.8.10. 

Screenshots of the bar graph, box plot, histogram, scatter matrix, 4-class classification, and accuracy graph have also been provided for visual reference. 

## Requirements
As of 5/21/2026, the package requirements are as follows:
- scikit-learn: 1.3.2
- NumPy: 1.24.4
- seaborn: 0.12.2 (seaborn had issues with importing, so matplotlib was substituted in for the histogram)
- Matplotlib: 3.7.3

Note that using the most recent version of scikit-learn is recommended to avoid the "AttributeError: module 'numpy' has not attribute 'typeDict'", which occurs when using a version of NumPy >= 1.20.0 and using a version of scikit-learn <= 1.3.0.

## Results
The most accurate model overall was the K-NN classifier, with a 0.95 accuracy on the training data and a 1.00 accuracy on the testing data, followed closely by the Decision Tree with a 1.00 accuracy on the training data and a 0.87 accuracy on the testing data. The worst performing model overall was the Logistic Regression classifier, with a 0.75 accuracy on the training data and a 0.47 accuracy on the testing data.

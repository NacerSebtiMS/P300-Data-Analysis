# Data-Analysis

+ The analysis consists in identifying the signals measured the presence of a wave called P300
+ Studying the automation of this classification and implementing several pattern recognition techniques to evaluate them.

## The dataset

+ The first category includes signals that are pre-labeled as P300 or P300-free, and should be used to design and validate the recognition system.
+ The second category includes signals for which the category to which they belong is not known a priori (unknown). The recognition system will automatically classify them into the CP300 or CP300-free class.

### Study and analysis of the distributions (probability distributions)
+ Examine the shape of the probability laws (dispersion and distribution of points);
+ Examine the eigenvalues of the covariance matrices;
+ Study the relevance of decorrelation of coordinates;
+ In order to reduce computations and the duration of treatments, study the relevance of a dimension reduction by decorrelation;
Examine again the shape of the laws of probability after decorrelation.
+ Study the visual form of the boundary equations between CP300 and Non CP300 classes;
+ From previous work, deduce the advantages and disadvantages of direct estimation of probability densities by joint probabilities or by independent likelihood estimation for each of the dimensions.

### Implementation of three Bayesian classification algorithms

All three algorithms must take into account the cost associated with poor detection of the P300. The cost of not detecting the presence of a P300 ("false negative") is 3, while the cost of not detecting the absence of a P300 ("false positive") is 1.

+ Implement a classification algorithm that uses the assumption that the laws are Gaussian;
+ Implement another algorithm that allows a classification without using the mathematical expression of the boundaries and without assuming the Gaussian character but using the risk as defined by Bayes.
+ Finally for the third algorithm use the mathematical expression of the boundaries assuming that the probability densities are Gaussian.

### Evaluation

+ Separate the data into two sets :
    + learning set;
    + Testing set.
+ With these sets, evaluate the average classification rate of the 3 systems, compare the results and comment

### K-NN & K-means

Test now and experiment with non-parametric approaches. Document the classification of the same signals as before using two methods :
+ Classification by the k-nearest neighbors (k-NN);
+ Classification according to the k-NN algorithm but first using vector quantization (k-means) in order to reduce the size of the data used for the classification.

Criticize and compare the two methods of using k-NN.

### Comparison

Based on the average misclassification rate of the different techniques you used, comment, document and discuss the results by comparing the techniques.

### Image recognition

Brain response is highly dependent on context and mood. It would therefore be important to match the EEG measurement with images from a camera to determine the person's mood (tense, angry, relaxed, etc.). We choose to classify the environments in which the subject finds himself or herself by assuming that the environment has an impact on mood. Evaluate the possibility of classifying the nature of images into three categories (beach, forest and town/road).

For simplicity, only color information be used. You will design an image recognition system that will allow to classify the nature of images in the 3 categories (beach, forest and city) with only the color information. The system must be able to operate for different codings of the color characteristics of the images.

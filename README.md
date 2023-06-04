# Movie_Classification

In this project, I built a classifier that predicts whether a movie is a comedy or a thriller based on the frequency of words in the movie's screenplay. The goal was to explore whether a bag-of-words representation, which describes only the frequencies of individual words, is sufficient to build an accurate genre classifier.

## Dataset
The dataset used in this project consists of movie screenplays. It includes a list of 5,000 words that occur in conversations between movie characters. For each movie, the dataset provides the frequency with which each of these words occurs in certain conversations in the screenplay. The dataset has been preprocessed to convert all words to lowercase and remove any inappropriate language.

## Methodology
**Word Stemming**
To preprocess the dataset, the words in the screenplay were stemmed, or abbreviated heuristically, in order to group different inflected forms of the same base word. This process helps to reduce the dimensionality of the dataset and make it easier to analyze.

**Exploratory Data Analysis: Linear Regression**
Before building the classifier, an exploratory data analysis was conducted. The relationship between different word proportions in the movies was examined. For example, the association between the proportion of words that are "outer" and the proportion of words that are "space" was investigated. The analysis involved visualizing the data and performing linear regression to understand the correlation between the variables.

**Splitting the Dataset**
To train and test the classifier, the dataset was split into two parts: a training set and a test set. The training set was used to build the classifier, while the test set was used to evaluate its performance. The splitting was done randomly, ensuring that no movies appeared in both sets.

**K-Nearest Neighbors (k-NN) Classification**
The classifier in this project is based on the k-nearest neighbors (k-NN) algorithm. The algorithm classifies a movie by finding the k movies in the training set that are most similar to it based on the chosen features. The similarity is calculated using the Euclidean distance between the movies' features. The algorithm assigns the movie to the most common category among its k nearest neighbors.

## Results
The project aimed to predict the genre of movies as either comedy or thriller based on the word frequencies in their screenplays. By applying the k-nearest neighbors classification method, the classifier was able to make predictions. The accuracy of the classifier was evaluated using the test set.


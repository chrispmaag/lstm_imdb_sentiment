# LSTM for Sentiment Analysis on IMDB Dataset

![rotten_tomatoes](https://github.com/chrispmaag/lstm_imdb_sentiment/blob/main/images/rotten_tomatoes.jpg)

In this project, we will predict the sentiment of movie reviews using a long short-term memory (LSTM) neural network. This type of network helps address the vanishing gradient problem seen in more basic RNN models by introducing forget, input, and output gates to control the flow of information between each step.

## Library Requirements
- TensorFlow and numpy

## Data
We'll use TensorFlow's built in IMDB Movie Review dataset that can be found at [https://www.tensorflow.org/api_docs/python/tf/keras/datasets/imdb](https://www.tensorflow.org/api_docs/python/tf/keras/datasets/imdb).

## Get the Code
Download the lstm_imdb_sentiment.ipynb file and run it.

## Results

After training, our model gets an f1 score of 0.87.

![model_results](https://github.com/chrispmaag/lstm_imdb_sentiment/blob/main/images/model_results.jpg)

We can then evaluate the model on random reviews from Rotten Tomatoes. The model correctly predicts negative sentiment for the following reviews:
![negative1](https://github.com/chrispmaag/lstm_imdb_sentiment/blob/main/images/negative1.jpg)
![negative2](https://github.com/chrispmaag/lstm_imdb_sentiment/blob/main/images/negative2.jpg)

It also correctly predicts positive sentiment for the following reviews:
![positive1](https://github.com/chrispmaag/lstm_imdb_sentiment/blob/main/images/postive1.jpg)
![positive2](https://github.com/chrispmaag/lstm_imdb_sentiment/blob/main/images/positive2.jpg)

There is still opportunity to improve this model. The below review is a false negative, meaning the review was actually positive, but the model predicted a negative sentiment.

![false_negative1](https://github.com/chrispmaag/lstm_imdb_sentiment/blob/main/images/false_negative1.jpg)
# Recurrent-Neural-Network-from-Scratch-in-Python
An Essential Read for Data Scientists
Flashback: A Recap of Recurrent Neural Network Concepts
Let’s quickly recap the core concepts behind recurrent neural networks.

We’ll do this using an example of sequence data, say the stocks of a particular firm. A simple machine learning model, or an Artificial Neural Network, may learn to predict the stock price based on a number of features, such as the volume of the stock, the opening value, etc. Apart from these, the price also depends on how the stock fared in the previous fays and weeks. For a trader, this historical data is actually a major deciding factor for making predictions.

In conventional feed-forward neural networks, all test cases are considered to be independent. Can you see how that’s a bad fit when predicting stock prices? The NN model would not consider the previous stock price values – not a great idea!

There is another concept we can lean on when faced with time sensitive data – Recurrent Neural Networks (RNN)!
It is now easier for us to visualize how these networks are considering the trend of stock prices. This helps us in predicting the prices for the day. Here, every prediction at time t (h_t) is dependent on all previous predictions and the information learned from them. Fairly straightforward, right?

RNNs can solve our purpose of sequence handling to a great extent but not entirely.

Text is another good example of sequence data. Being able to predict what word or phrase comes after a given text could be a very useful asset. We want our models to write Shakespearean sonnets!

Now, RNNs are great when it comes to context that is short or small in nature. But in order to be able to build a story and remember it, our models should be able to understand the context behind the sequences, just like a human brain.
Sequence Prediction using RNN
In this article, we will work on a sequence prediction problem using RNN. One of the simplest tasks for this is sine wave prediction. The sequence contains a visible trend and is easy to solve using heuristics. This is what a sine wave looks like:



We will first devise a recurrent neural network from scratch to solve this problem. Our RNN model should also be able to generalize well so we can apply it on other sequence problems.

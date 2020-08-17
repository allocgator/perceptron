# Perceptron
Project 1 for Artificial Neural Networks

The file `​dataset.py​` contains the letters A through Z as 5-by-7 dot-matrix fonts, in a format similar to the [​Hebb Net example​] for character recognition. There are two different fonts, one for training and one for test.
[​NumPy​] is to implement vector operations such as dot product, and [Matplotlib] library to generate plots.

# Training Perceptrons

There are 26 perceptrons in total, one for each letter. Each perceptron learns to output 1 for its assigned letter and 0 for all other letters. Weights and biases are initialized to random values (rather than zero) for each perceptron, following which the ​[perceptron learning algorithm​] is applied until all items in the training set are classified correctly or until it becomes clear that the weights will not converge.

The output of each perceptron, which classifies an item in the training set, is recorded for correctness. At the end of each pass through the training set, the *error rate* (number of misclassified items) of that perceptron is also recorded for that epoch.

# Testing the Learned Weights

If a letter is linearly separable from the others and the learning rate is small enough, there is a downward trend in error rate until each point is classified correctly. *matplotlib* is used to ​plot the error rate as a function of the number of epochs​ in order to visualize this trend.

Once the perceptrons have been trained (in other words, once the perceptrons for the letters which are linearly separable from other letters have converged), each trained perceptron is tested against the letters in the test set.

[​Hebb Net example​]: https://gist.github.com/ProfAvery/01fc74d75accbe3c1926550a2ca05e4d
[perceptron learning algorithm​]: https://en.wikipedia.org/wiki/Perceptron#Learning_algorithm
[Matplotlib]: https://matplotlib.org
[​NumPy​]: https://numpy.org

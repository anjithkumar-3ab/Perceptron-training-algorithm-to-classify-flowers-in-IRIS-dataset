Perceptron Classifier on Iris Dataset

This project implements a binary Perceptron classifier from scratch using NumPy, trained on a subset of the Iris dataset.

Only two classes are used:

Iris-setosa → 0

Iris-versicolor → 1

Iris-virginica is intentionally removed to keep the problem linearly separable, which is a requirement for a classic Perceptron.

What This Project Does

Loads the Iris dataset from the UCI repository

Filters it to a binary classification problem

Uses only two features:

sepal_length

sepal_width

Trains a Perceptron using:

Step activation function

Gradient-based weight updates

Prints weights and bias after each epoch

Computes final training accuracy

This is an educational implementation, not a production ML model.

Dataset

Source: UCI Machine Learning Repository

Dataset: Iris

URL:
https://archive.ics.uci.edu/ml/machine-learning-databases/iris/iris.data

Algorithm Used

Perceptron Learning Algorithm

Update rule:

w = w + η · (y − ŷ) · x
b = b + η · (y − ŷ)


Where:

η = learning rate

y = true label

ŷ = predicted label

Activation function:

step(z) = 1 if z ≥ 0 else 0

Hyperparameters

Learning rate: 0.01

Epochs: 20

Initial weights: 0

Initial bias: 0

Requirements

Install dependencies using:

pip install numpy pandas

How to Run
python perceptron.py


Make sure the script file contains the provided code.

Output

Prints weights and bias after each epoch

Displays final training accuracy

Example:

Epoch 1 : Weights=[...], Bias=...
...
Final Accuracy: 1.0


(Accuracy may vary slightly depending on convergence.)

Limitations (Don’t Ignore This)

Works only for linearly separable data

Uses no test/train split → accuracy is training accuracy only

Uses only 2 features instead of all 4

No normalization or feature scaling

This is intentional to keep the math simple.

Purpose

This project is meant to:

Understand how a Perceptron works internally

Learn weight updates and decision boundaries

Avoid black-box ML libraries

If you’re using this as a “machine learning project” without understanding it, you’re wasting your time.

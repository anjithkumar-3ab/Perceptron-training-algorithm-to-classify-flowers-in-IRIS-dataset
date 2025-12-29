# Perceptron Classifier on Iris Dataset

This project implements a **binary Perceptron classifier from scratch using NumPy**, trained on a subset of the Iris dataset.

Only two classes are considered:
- Iris-setosa → 0
- Iris-versicolor → 1

The class *Iris-virginica* is removed to ensure linear separability, which is required for a standard Perceptron.

---

## Project Overview

- Loads Iris dataset from the UCI repository
- Filters data for binary classification
- Uses two features:
  - sepal_length
  - sepal_width
- Trains a Perceptron using a step activation function
- Updates weights and bias using the Perceptron learning rule
- Prints weights and bias after each epoch
- Calculates final training accuracy

This is a **learning-focused implementation**, not a production model.

---

## Dataset

- Name: Iris Dataset
- Source: UCI Machine Learning Repository
- URL:  
  https://archive.ics.uci.edu/ml/machine-learning-databases/iris/iris.data

---

## Algorithm

**Perceptron Learning Algorithm**

Update equations:

w = w + η × (y − ŷ) × x  
b = b + η × (y − ŷ)

Activation function:

step(z) = 1 if z ≥ 0 else 0

---

## Hyperparameters

- Learning rate: 0.01
- Epochs: 20
- Initial weights: zeros
- Initial bias: 0

---

## Requirements

Install required libraries:

pip install numpy pandas

---

## How to Run

python perceptron.py

---

## Output

- Displays weights and bias after each epoch
- Prints final training accuracy

Example:

Epoch 1 : Weights=[...], Bias=...  
Final Accuracy: 1.0

(Exact values may vary slightly.)

---

## Limitations

- Works only with linearly separable data
- No train/test split (accuracy is training accuracy only)
- Uses only 2 out of 4 available features
- No feature scaling or normalization

These limitations are intentional for simplicity.

---

## Purpose

This project is designed to:
- Understand Perceptron fundamentals
- Learn manual weight updates
- Avoid black-box machine learning libraries

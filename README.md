
[![PyPI - Python Version](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue)]()
[![PyPI version](https://img.shields.io/pypi/v/openfl)]()
[![Citation](https://img.shields.io/badge/cite-citation-brightgreen)]()
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]()

# Causal Neural Network.
In this repository, we open-source the causal neural network from our paper. This library allows you to estimate the CATE of any targeting intervention.

## causal_neural_network function
We provide a function that replicates our estimator of the CATE in causal_neural_network.py. This function requires the following parameters: 

1. `X`: a numpy set of covariates.
2. `Y`: a numpy set of outcome variable (e.g., revenue).
3. `T`: a numpy vector of the treatment received.
4. `scaling`: requires whether `X` should be scaled (boolean).
5. `simulations`: requires the number of average CATE's (int).
6. `epochs`: requires the number of epochs (int).
7. `batch_size`: requires the batch size (int).
8. `folds`: requires the number of folds for K-fold cross-validation.

## Example using simulated data.
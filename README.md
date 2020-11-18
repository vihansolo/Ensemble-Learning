# Ensemble Learning

- **Ensemble learning** is the process by which multiple models, such as classifiers or experts, are strategically generated and combined to solve a particular computational intelligence problem. In this program, ensemble learning is demonstrated using Super Learner method in Mlens library.

- **The Super Learner (also known as the Stacking Ensemble)** is an supervised ensemble algorithm that uses K-fold estimation to map a training set into a prediction set, where the predictions are constructed using K-Fold splits of the features to ensure test set reflects test errors, and that applies a user-specified meta learner to predict labels from test set.

- The task has been performed using the **Adult dataset** present [here](https://archive.ics.uci.edu/ml/datasets/adult).

## Requirements and running the program

1. The required python libraries to run this program are -
    - [numpy](https://pypi.org/project/numpy/)
    - [pandas](https://pypi.org/project/pandas/)
    - [scikit-learn](https://pypi.org/project/scikit-learn/)
    - [tabulate](https://pypi.org/project/tabulate/)
    - [mlens](https://pypi.org/project/mlens/)

2. To run the jupyter notebook
    - Open the .ipynb file in Jupyter Notebook using Anaconda or in VSCode using [jupyter](https://pypi.org/project/jupyter/) package.
    - Run each cell to get results.

## Ensembler

The ensembler has been created using the following algorithms -

- KNeighbors Classifier
- Naive Bayes Classifier
- Support Vector Classifier
- Decision Tree Classifier
- Random Forest Classifier
- Adaboost Classifier
- Gradient Boosting Classifier
- Linear Discriminant Analysis Classifier
- Multilayer Perceptron Classifier
- Logistic Regression Classifier

> Note: Take note of the hyperparameters used for tuning in the jupyter notebook itself.

The Adaboost Classifier was used as the [meta algorithm](https://www.quora.com/What-is-the-common-definition-for-a-meta-algorithm#:~:text=Loosely%20speaking%2C%20a%20meta%2Dalgorithm,those%20algorithms%20on%20their%20own.).

## Accuracy

The individual accuracies of the algorithms obtained are as follows -

| Algorithms          |   Accuracy (%) |
|---------------------|----------------|
| K-Neighbors         |        79.3275 |
| Naive Bayes         |        78.8116 |
| SVM                 |        79.223  |
| Decision Tree       |        84.9429 |
| Random Forest       |        85.7525 |
| Adaboost            |        86.6732 |
| Gradient Boosting   |        86.3532 |
| LDA                 |        83.8459 |
| MLP                 |        77.016  |
| Logistic Regression |        84.8253 |

<br>

The ensemble accuracy obtained was 86.78 %.

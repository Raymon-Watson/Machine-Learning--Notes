# Machine Learning Learning Repository

This repository documents my progress learning the core concepts, techniques, and models used in machine learning.

The main goal is to develop both an understanding of how common ML methods work and practical experience applying them to real datasets using Python and scikit-learn.

## Core Machine Learning Workflow

Most projects in this repository follow the same general workflow:

1. **Understand the problem**

   * Identify the target variable
   * Determine whether the problem is classification, regression, clustering, etc.
   * Choose appropriate evaluation metrics

2. **Explore the data**

   * Inspect distributions and summary statistics
   * Identify missing values and outliers
   * Examine relationships between features and the target
   * Visualise important patterns

3. **Prepare the data**

   * Train/test splitting
   * Missing-value imputation
   * Categorical encoding
   * Feature scaling
   * Feature engineering
   * Handling class imbalance where necessary

4. **Build baseline models**

   * Start with a simple model
   * Establish a benchmark before increasing model complexity

5. **Train and compare models**

   * Fit several appropriate algorithms
   * Compare performance using cross-validation
   * Examine underfitting and overfitting

6. **Tune the model**

   * Hyperparameter optimisation
   * `GridSearchCV`
   * `RandomizedSearchCV`

7. **Evaluate the final model**

   * Evaluate once on the held-out test set
   * Analyse prediction errors
   * Interpret model performance and limitations

---

## Essential Techniques

### Data Preprocessing

Important preprocessing techniques include:

* Train/test splitting
* Stratified sampling
* Missing-value imputation
* Standardisation and normalisation
* One-hot encoding
* Ordinal encoding
* Feature transformations
* Outlier detection
* Feature engineering
* Data pipelines

Useful scikit-learn tools include:

```python
train_test_split
StandardScaler
SimpleImputer
OneHotEncoder
OrdinalEncoder
ColumnTransformer
Pipeline
```

---

## Regression

Regression models predict continuous values.

Models to understand:

* Linear Regression
* Polynomial Regression
* Ridge Regression
* Lasso Regression
* Elastic Net
* Decision Tree Regression
* Random Forest Regression
* Gradient Boosting
* XGBoost / similar boosting methods

Important concepts:

* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)
* Mean Absolute Error (MAE)
* R²
* Residual analysis
* Regularisation
* Bias-variance trade-off

---

## Classification

Classification models predict discrete classes.

Models to understand:

* Logistic Regression
* k-Nearest Neighbours
* Naive Bayes
* Support Vector Machines
* Decision Trees
* Random Forests
* Gradient Boosting
* Neural Networks

Important evaluation methods include:

* Accuracy
* Precision
* Recall
* F1 score
* Confusion matrix
* ROC curve
* ROC-AUC
* Precision-recall curves

For multiclass problems, it is also useful to understand:

* One-vs-Rest
* One-vs-One
* Macro, micro and weighted averaging

---

## Decision Trees and Ensemble Methods

Important topics include:

* Decision tree splitting
* Gini impurity
* Entropy
* Information gain
* Tree depth and pruning
* Bagging
* Random forests
* Boosting
* Gradient boosting

These methods are particularly useful for understanding the difference between individual weak models and ensembles of models.

---

## Model Selection

Important techniques include:

### Cross-Validation

Use cross-validation to estimate how well a model is likely to generalise to unseen data.

```python
cross_val_score
cross_validate
cross_val_predict
```

### Hyperparameter Tuning

Common tools include:

```python
GridSearchCV
RandomizedSearchCV
```

Model selection should generally be performed using the training data. The test set should be reserved for final evaluation.

---

## Feature Selection and Engineering

Useful techniques include:

* Correlation analysis
* Creating derived features
* Removing irrelevant features
* Feature importance
* Recursive feature elimination
* Regularisation-based feature selection
* Dimensionality reduction

Good feature engineering can sometimes improve performance more than changing the model itself.

---

## Dimensionality Reduction

Important techniques include:

* Principal Component Analysis (PCA)
* Explained variance
* Feature projection
* Visualising high-dimensional data

PCA is particularly useful for understanding how high-dimensional datasets such as image data can be represented using fewer variables.

---

## Unsupervised Learning

Unlike supervised learning, unsupervised methods do not require labelled target data.

Important techniques include:

### Clustering

* k-Means
* Hierarchical clustering
* DBSCAN

Important concepts:

* Choosing the number of clusters
* Inertia
* Silhouette score
* Cluster interpretation

### Dimensionality Reduction

* PCA
* t-SNE
* UMAP

---

## Neural Networks

Core concepts to understand include:

* Artificial neurons
* Layers
* Activation functions
* Forward propagation
* Loss functions
* Backpropagation
* Gradient descent
* Learning rate
* Batch size
* Epochs

Important architectures include:

* Multilayer Perceptrons (MLPs)
* Convolutional Neural Networks (CNNs)
* Recurrent Neural Networks (RNNs)
* Transformers

The initial focus is on understanding basic feed-forward neural networks before moving to more specialised architectures.

---

## General ML Concepts

Some concepts apply across almost every machine learning problem:

* Training, validation and test sets
* Generalisation
* Overfitting and underfitting
* Bias-variance trade-off
* Data leakage
* Feature scaling
* Regularisation
* Hyperparameters vs model parameters
* Cross-validation
* Learning curves
* Model interpretability
* Reproducibility
* Error analysis

Understanding these ideas is generally more important than memorising large numbers of algorithms.

---

## Tools

The main tools used throughout this repository are:

* Python
* NumPy
* pandas
* Matplotlib
* scikit-learn
* Jupyter Notebook

Additional libraries may be introduced for more advanced projects, including:

* XGBoost
* TensorFlow / Keras
* PyTorch

---

## Repository Goal

The aim is not simply to train models with high accuracy, but to understand:

* **why a model works**
* **when it should be used**
* **how to evaluate it correctly**
* **how to diagnose problems**
* **how to improve its performance**
* **how well it generalises to unseen data**

Each project provides an opportunity to apply these ideas to a practical machine learning problem.

# Machine Learning Learning Repository

This repository tracks my progress as I learn the main ideas, techniques, and models used in machine learning.

The aim is to build a solid understanding of the fundamentals, then apply them through small projects using Python, pandas, scikit-learn, and related tools.

Rather than trying to learn every model at once, I’m working through the topics below roughly in order.

---

## 1. Machine Learning Basics

Start with the general ideas that apply to almost every ML problem.

Topics to understand:

* Supervised vs unsupervised learning
* Classification vs regression
* Features and target variables
* Training, validation, and test sets
* Overfitting and underfitting
* Generalisation
* Bias-variance trade-off
* Model parameters vs hyperparameters
* Data leakage
* Reproducibility

The main goal here is to understand how a machine learning project should be structured before worrying too much about individual models.

---

## 2. Data Preparation

Before training models, I want to be comfortable preparing real datasets.

Topics to practise:

* Train/test splitting
* Stratified sampling
* Handling missing values
* Standardisation and normalisation
* One-hot encoding
* Ordinal encoding
* Handling categorical variables
* Outlier detection
* Basic feature engineering
* Using pipelines

Useful scikit-learn tools:

```python
train_test_split
SimpleImputer
StandardScaler
OneHotEncoder
OrdinalEncoder
ColumnTransformer
Pipeline
```

---

## 3. Regression

Regression models are used when the target is a continuous value.

Models to learn:

* Linear Regression
* Polynomial Regression
* Ridge Regression
* Lasso Regression
* Elastic Net
* Decision Tree Regression
* Random Forest Regression
* Gradient Boosting Regression

Main concepts:

* Mean Squared Error
* Root Mean Squared Error
* Mean Absolute Error
* R²
* Residual analysis
* Regularisation
* Overfitting in regression models

I want to start with linear models before moving on to tree-based and ensemble methods.

---

## 4. Classification

Classification models predict categories or classes.

Models to learn:

* Logistic Regression
* k-Nearest Neighbours
* Naive Bayes
* Support Vector Machines
* Decision Trees
* Random Forests
* Gradient Boosting

Evaluation methods:

* Accuracy
* Precision
* Recall
* F1 score
* Confusion matrix
* ROC curve
* ROC-AUC
* Precision-recall curve

For multiclass problems, I also want to understand:

* One-vs-Rest
* One-vs-One
* Macro averaging
* Micro averaging
* Weighted averaging

---

## 5. Decision Trees and Ensemble Methods

Once I am comfortable with basic regression and classification, I want to spend more time on tree-based models.

Topics to learn:

* How decision trees choose splits
* Gini impurity
* Entropy
* Information gain
* Tree depth
* Overfitting and pruning
* Bagging
* Random forests
* Boosting
* Gradient boosting

These methods are useful because they introduce many of the ideas behind modern ensemble models.

---

## 6. Model Evaluation and Selection

The next step is learning how to compare models properly.

Topics:

* Cross-validation
* Choosing suitable evaluation metrics
* Comparing training and validation performance
* Learning curves
* Detecting overfitting
* Error analysis

Useful scikit-learn tools:

```python
cross_val_score
cross_validate
cross_val_predict
```

---

## 7. Hyperparameter Tuning

After choosing a reasonable model, I want to learn how to tune it without overfitting to the test set.

Main tools:

```python
GridSearchCV
RandomizedSearchCV
```

Topics to understand:

* Parameter grids
* Cross-validation during tuning
* Choosing a scoring metric
* Inspecting validation results
* Selecting the best model
* Keeping the test set separate until final evaluation

---

## 8. Feature Engineering and Feature Selection

Once the basic workflow is familiar, I want to focus more on improving the input data.

Topics:

* Creating useful new features
* Transforming existing features
* Removing unnecessary features
* Correlation analysis
* Feature importance
* Recursive feature elimination
* Regularisation-based feature selection

The goal here is to understand how better features can sometimes improve a model more than simply choosing a more complicated algorithm.

---

## 9. Dimensionality Reduction

For datasets with many features, I want to learn methods for reducing the number of dimensions.

Main topics:

* Principal Component Analysis
* Explained variance
* Choosing the number of components
* Visualising high-dimensional data

Main method to learn:

* PCA

Later I may also explore:

* t-SNE
* UMAP

---

## 10. Unsupervised Learning

After supervised learning, I want to cover the main unsupervised learning techniques.

### Clustering

Methods to learn:

* k-Means
* Hierarchical clustering
* DBSCAN

Concepts to understand:

* Choosing the number of clusters
* Inertia
* Silhouette score
* Interpreting clusters

### Dimensionality Reduction

Methods:

* PCA
* t-SNE
* UMAP

---

## 11. Neural Networks

Once I am comfortable with traditional machine learning, I want to move on to neural networks.

Start with:

* Artificial neurons
* Layers
* Activation functions
* Loss functions
* Forward propagation
* Backpropagation
* Gradient descent
* Learning rate
* Batch size
* Epochs

Then move on to:

* Multilayer Perceptrons
* Convolutional Neural Networks
* Recurrent Neural Networks
* Transformers

The priority is to understand simple feed-forward neural networks first before moving on to more specialised architectures.

---

## 12. Machine Learning Workflow

For most projects, I want to follow roughly the same structure:

1. Understand the problem
2. Load and inspect the data
3. Perform exploratory data analysis
4. Clean and prepare the data
5. Split into training and test sets
6. Build a simple baseline model
7. Train several suitable models
8. Compare them using cross-validation
9. Tune the strongest candidates
10. Evaluate the final model on the test set
11. Analyse errors and limitations
12. Summarise the results

Using a consistent workflow should make it easier to compare projects and build good habits.

---

## Tools

The main tools used throughout this repository are:

* Python
* NumPy
* pandas
* Matplotlib
* scikit-learn
* Jupyter Notebook

Later projects may also use:

* XGBoost
* TensorFlow / Keras
* PyTorch

---

## Current Goal

The main aim of this repository is not to memorise as many algorithms as possible.

Instead, I want to be able to:

* understand how the main models work
* know when to use them
* prepare data correctly
* evaluate models properly
* recognise overfitting and data leakage
* tune models effectively
* interpret results
* apply the full ML workflow to new datasets

The projects in this repository will gradually build up these skills.

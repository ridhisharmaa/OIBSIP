# Iris Flower Classification

This project uses machine learning to predict the species of an iris flower (Setosa, Versicolor, or Virginica) based on its sepal and petal measurements.

## Dataset

The Iris dataset comes built into scikit-learn, so there's no need to download anything separately. It has 150 rows and 4 features: sepal length, sepal width, petal length, petal width.

## What's in the notebook

- Loading the dataset with `load_iris()`
- Basic EDA (shape, data types, null check, describe)
- Pairplot and box plots to see how the features differ by species
- Train/test split (80/20)
- Two models trained: Logistic Regression, KNN, and Decision Tree
- Accuracy, confusion matrix, and classification report for each model
- Final comparison and best model pick

## How to run

1. Make sure you have Python installed with these packages:
   ```
   pandas
   numpy
   matplotlib
   seaborn
   scikit-learn
   ```
   You can install them with:
   ```
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```
2. Open `iris_classification.ipynb` in Jupyter Notebook or JupyterLab.
3. Run all cells from top to bottom.

## Result

Petal length and petal width turned out to be the most useful features for telling the species apart. Logistic Regression and KNN both performed really well on this dataset.

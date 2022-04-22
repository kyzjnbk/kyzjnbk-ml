# Supervised Learning

## Decision Tree

A Decision Tree algorithm is one of the most popular machine learning algorithms. It uses a tree like structure and their possible combinations to solve a particular problem. It belongs to the class of supervised learning algorithms where it can be used for both classification and regression purposes.

??? cite "Tutorial on Karggle"
    - [Karggle](https://www.kaggle.com/code/prashant111/decision-tree-classifier-tutorial)
    - [Download notebook](supervised.asserts/decision-tree-classifier-tutorial.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kyzjnbk/kyzjnbk-ml/blob/master/docs/diagram/supervised.asserts/decision-tree-classifier-tutorial.ipynb)
    - [Download data for this tutorial](supervised.asserts/data/car_evaluation.csv)


### Quick References

#### Entropy

$$ \text{Entropy} = \sum_{i=1}^c - p_i \log_2(p_i) $$
where $c$ is the number of classes and $p_i$ is the probability associated with the ith class.

#### Gini index

$$ \text{Gini} = 1- \sum_{i=1}^c p_i^2 $$
where $c$ is the number of classes and $p_i$ is the probability associated with the ith class.

#### Python

??? note "Category Encoders"

    ```bash
    pip install category_encoders
    ```

    or

    ```bash
    conda install -c conda-forge category_encoders
    ```

    To use:

    ```py
    import category_encoders as ce

    encoder = ce.BackwardDifferenceEncoder(cols=[...])
    encoder = ce.BaseNEncoder(cols=[...])
    encoder = ce.BinaryEncoder(cols=[...])
    encoder = ce.CatBoostEncoder(cols=[...])
    encoder = ce.CountEncoder(cols=[...])
    encoder = ce.GLMMEncoder(cols=[...])
    encoder = ce.HashingEncoder(cols=[...])
    encoder = ce.HelmertEncoder(cols=[...])
    encoder = ce.JamesSteinEncoder(cols=[...])
    encoder = ce.LeaveOneOutEncoder(cols=[...])
    encoder = ce.MEstimateEncoder(cols=[...])
    encoder = ce.OneHotEncoder(cols=[...])
    encoder = ce.OrdinalEncoder(cols=[...])
    encoder = ce.SumEncoder(cols=[...])
    encoder = ce.PolynomialEncoder(cols=[...])
    encoder = ce.TargetEncoder(cols=[...])
    encoder = ce.WOEEncoder(cols=[...])
    encoder = ce.QuantileEncoder(cols=[...])

    encoder.fit(X, y)
    X_cleaned = encoder.transform(X_dirty)
    ```

    - https://contrib.scikit-learn.org/category_encoders/

??? note "sklearn.tree.DecisionTreeClassifier"

    - [scikit-learn: sklearn.tree.DecisionTreeClassifier](https://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeClassifier.html)


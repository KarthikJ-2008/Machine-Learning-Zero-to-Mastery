# Introduction to Random Forest

**Random Forest** is a supervised machine learning algorithm used for both **classification and regression** problems.

It is an ensemble learning algorithm that combines multiple Decision Trees to make better predictions.

Instead of depending on a single decision tree, Random Forest uses many trees and combines their results.

**Example:** Predicting whether a customer will buy a product based on age, income, and shopping habits.

##  What is Random Forest?

Random Forest creates multiple Decision Trees using different random samples of the training data and random subsets of features.

The final prediction is made by combining the predictions of all trees.

- **Classification:** Uses majority voting.
- **Regression:** Uses the average of all tree predictions.

![Random Forest Algorithm](https://media.geeksforgeeks.org/wp-content/uploads/20251216121929631349/random_forest_algorithm.webp)

## How Does Random Forest Work?

Random Forest works by building multiple decision trees and combining their predictions.

### Steps Involved:

1. **Collect Data:** Start with the training dataset.
2. **Random Sampling:** Create different random samples from the original dataset using sampling with replacement (Bootstrap Sampling).
3. **Build Decision Trees:** Train a separate decision tree using each sample.
4. **Random Feature Selection:** Each tree considers a random subset of features when splitting nodes.
5. **Make Predictions:** Each decision tree makes its own prediction.
6. **Combine Results:** Combine all predictions to get the final output.

## How Does Random Forest Make Predictions?

### 1. Classification

- Each decision tree predicts a class.
- The class receiving the most votes becomes the final prediction.

**Example:**

Suppose five decision trees predict:

- Tree 1: Yes
- Tree 2: No
- Tree 3: Yes
- Tree 4: Yes
- Tree 5: No

**Final Prediction: Yes** (3 votes).

### 2. Regression

- Each decision tree predicts a numerical value.
- Random Forest calculates the average of all predictions.

**Example:**

Suppose three trees predict house prices:

- Tree 1: ₹20 lakh
- Tree 2: ₹25 lakh
- Tree 3: ₹30 lakh

Final Prediction:

$Prediction = \frac{20 + 25 + 30}{3} = 25$

**Final Prediction: ₹25 lakh**

##  Key Components of Random Forest

### 1. Bagging (Bootstrap Aggregation)

- Creates different random samples from the original dataset.
- Sampling is done with replacement.
- Each decision tree is trained independently using a different sample.

### 2. Random Feature Selection

- Each tree considers a random subset of features when splitting nodes.
- This makes the trees less similar to each other.
- It helps improve the overall performance of the model.

##  Important Parameters of Random Forest

### 1. n_estimators

- Specifies the number of decision trees in the forest.
- Example: `n_estimators=100` creates 100 decision trees.

### 2. max_depth

- Controls the maximum depth of each decision tree.
- Helps prevent overfitting.

### 3. max_features

- Specifies the number of features considered when searching for the best split.

### 4. random_state

- Controls randomness to help produce reproducible results.

##  Advantages of Random Forest

- Provides good prediction accuracy.
- Works for both classification and regression.
- Reduces overfitting compared to a single decision tree in many cases.
- Handles large datasets with many features.
- Provides feature importance to identify useful features.

##  Disadvantages of Random Forest

- Requires more memory because it stores multiple trees.
- Can be slower than a single decision tree.
- Difficult to interpret compared to a single decision tree.
- Requires parameter tuning for better performance.

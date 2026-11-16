# Introduction to Decision Tree

A **Decision Tree** is a supervised machine learning algorithm used for both **classification and regression** problems.

It works like a flowchart, making decisions based on different conditions or questions. Each decision leads to another branch until the final prediction is reached.

**Example:** Predicting whether a customer will buy a product based on their age, income, and other details.

##  Structure of a Decision Tree

A decision tree consists of three main components:

- **Root Node:** The starting point of the tree. It represents the entire dataset.
- **Decision Node:** A node where a condition or question is checked to split the data.
- **Leaf Node:** The final output or prediction of the decision tree.

![Decision Tree Structure](https://media.geeksforgeeks.org/wp-content/uploads/20251216110915386263/decision_tree.webp)

## 2. Types of Decision Trees

Decision Trees are mainly divided into two types:

### 1. Classification Tree

- Used to predict categorical or class-based outputs.
- The output belongs to a particular category.
- Example: Predicting whether an email is Spam or Not Spam.

### 2. Regression Tree

- Used to predict continuous numerical values.
- The output is a number.
- Example: Predicting house prices based on area, location, and number of rooms.

##  Working of a Decision Tree

A Decision Tree works by dividing the dataset into smaller groups based on conditions.

### Steps involved:

1. **Start with the Root Node:** The algorithm starts with the complete training dataset.
2. **Select the Best Feature:** It selects the feature that creates the best split.
3. **Split the Data:** The dataset is divided into smaller groups based on conditions.
4. **Repeat the Process:** The algorithm continues splitting the groups into branches.
5. **Reach the Leaf Node:** The final leaf node provides the predicted output.

### Example of Working
![Working of Decision Tree](https://media.geeksforgeeks.org/wp-content/uploads/20250408153824016146/predicting_whether_a_customer_will_buy_a_product.webp)

### Steps Involved:

1. **Root Node (Income):** The tree first checks whether the customer's income is greater than 50,000.
   - Yes: Move to the next decision.
   - No: Predict No Purchase.

2. **Internal Node (Age):** If income is greater than 50,000, check whether the customer's age is greater than 30.
   - Yes: Move to the next decision.
   - No: Predict No Purchase.

3. **Internal Node (Previous Purchase):** If the customer's age is greater than 30, check whether they have made any previous purchases.
   - Yes: Predict Purchase.
   - No: Predict No Purchase.

4. **Leaf Node:** The final result is either Purchase or No Purchase.

### Example:

- Income = 60,000
- Age = 35
- Previous Purchases = 2

**Prediction: Purchase**

##  Splitting Criteria

A Decision Tree uses different methods to select the best feature for splitting the dataset.

### 1. Gini Impurity

Gini Impurity measures how mixed the classes are in a node.

A lower Gini value indicates a better split.

Formula:

$Gini = 1 - \sum_{i=1}^{n} p_i^2$

Where:
- $p_i$ = Probability of each class.
- $n$ = Number of classes.

### 2. Entropy

Entropy measures the uncertainty or impurity in a dataset.

Lower entropy means the data is more organized into a single class.

Formula:

$Entropy = -\sum_{i=1}^{n} p_i \log_2(p_i)$

Where:
- $p_i$ = Probability of each class.
- $n$ = Number of classes.

### 3. Information Gain

Information Gain measures how much uncertainty is reduced after splitting the dataset.

Formula:

$Information\ Gain = Entropy(Parent) - Weighted\ Entropy(Children)$

A feature with higher Information Gain is preferred for splitting.

##  Advantages of Decision Tree

- Easy to understand and implement.
- Easy to visualize using a tree structure.
- Can be used for classification and regression.
- Requires less data preprocessing.
- Can handle numerical and categorical features, depending on the implementation.

##  Disadvantages of Decision Tree

- Can overfit the training data.
- Small changes in data may produce a different tree.
- Deep trees can become complex.
- May be biased when some classes dominate the dataset.

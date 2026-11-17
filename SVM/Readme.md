#  Introduction to Support Vector Machine (SVM)

**Support Vector Machine (SVM)** is a supervised machine learning algorithm mainly used for classification problems. It can also be used for regression.

SVM works by finding the best decision boundary (hyperplane) that separates different classes of data.

**Example:** Classifying emails as Spam or Not Spam.

##  What is a Support Vector Machine?

SVM tries to find the best hyperplane that separates two classes of data.

There can be many possible hyperplanes, but SVM selects the one that has the **maximum margin** between the two classes.

A larger margin generally helps the model classify new data more effectively.

![Support Vector Machine](https://miro.medium.com/v2/resize:fit:1358/1*VIlQzoYj5MsOqFgLO0mq3Q.png)

##  Important Terms in SVM

### 1. Hyperplane
A hyperplane is a decision boundary that separates different classes of data.

- In 2D, it is a straight line.
- In 3D, it is a plane.
- In higher dimensions, it is called a hyperplane.

### 2. Support Vectors
Support Vectors are the data points closest to the hyperplane.

These points help determine the position of the decision boundary.

### 3. Margin
Margin is the distance between the hyperplane and the nearest data points from both classes.

SVM tries to find the maximum possible margin.

## 4. Hyperplane Equation

The equation of a hyperplane is:

$w^T x + b = 0$

**Where:**

- `w` = Weight vector.
- `x` = Input feature vector.
- `b` = Bias value.

##  How Does SVM Work?

SVM works by finding the best boundary to separate different classes.

### Steps Involved:

1. **Collect Data:** Start with a dataset containing different classes.
2. **Plot Data Points:** Represent the data points based on their features.
3. **Find Possible Boundaries:** Identify different possible decision boundaries that separate the classes.
4. **Find Support Vectors:** Identify the closest data points to the decision boundary.
5. **Maximize the Margin:** Select the boundary with the maximum margin.
6. **Make Predictions:** Use the selected boundary to classify new data points.

##  Types of SVM

### 1. Linear SVM

- Used when data can be separated using a straight line or flat hyperplane.
- Example: Separating two classes using a straight line.

### 2. Non-Linear SVM

- Used when data cannot be separated using a straight line.
- Uses the Kernel Trick to create a non-linear decision boundary.

## 7. Important Parameters of SVC()

SVC stands for Support Vector Classifier. It is available in the Scikit-learn library.

### 1. C (Regularization Parameter)

- Controls the penalty for misclassifying training data.
- A small C allows a wider margin but may misclassify some points.
- A large C tries to classify training points correctly, which may result in a narrower margin.

### 2. Gamma

- Controls how far the influence of a single training point reaches.
- A small gamma creates a smoother decision boundary.
- A large gamma creates a more complex decision boundary and may cause overfitting.

### 3. Kernel

- Specifies the type of decision boundary used by SVM.
- Common kernels include:
  - `linear`
  - `poly`
  - `rbf`
  - `sigmoid`

## 8. Advantages of SVM

- Works well with high-dimensional data.
- Effective when there is a clear margin between classes.
- Can handle both linear and non-linear classification.
- Uses support vectors to determine the decision boundary.

## 9. Disadvantages of SVM

- Can be slow for large datasets.
- Choosing the correct kernel and parameters can be difficult.
- Sensitive to feature scaling.
- Not always suitable when classes overlap heavily.

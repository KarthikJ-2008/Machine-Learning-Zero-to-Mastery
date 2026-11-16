# Introduction to Logistic Regression

**Logistic Regression** is a supervised machine learning algorithm used for classification problems. Unlike Linear Regression, which predicts continuous numerical values, Logistic Regression predicts the probability that an input belongs to a particular class.

- It is mainly used for binary classification, where the output has two possible categories, such as Yes/No, True/False, or 0/1.
- It uses the **Sigmoid Function** to convert the model's output into a probability between 0 and 1.
- It is commonly used in spam detection, disease prediction, fraud detection, and student pass/fail prediction.

**Example:**

Suppose we want to predict whether a student will pass or fail based on the number of hours studied.

- **Input (Independent Variable):** Hours studied.
- **Output (Dependent Variable):** Pass or Fail.
- **Prediction:** If the predicted probability is 0.5 or above, classify the student as Pass (1). Otherwise, classify the student as Fail (0).

---

## Understanding the Sigmoid Function

The **Sigmoid Function** is the most important component of Logistic Regression. It converts any real-valued input into a probability between 0 and 1.

![Sigmoid Function](https://miro.medium.com/0*KZu2_AY6Oxr86dWd.png)

### Characteristics of the Sigmoid Function

1. It converts any real number into a value between 0 and 1.
2. It produces an S-shaped curve called the sigmoid curve or logistic curve.
3. It is used to calculate the probability of an input belonging to a particular class.

## Sigmoid Function Equation

**σ(z) = 1 / (1 + e⁻ᶻ)**

Where:

- **σ(z)** – Predicted probability
- **z** – Linear combination of input features
- **e** – Euler's number (approximately 2.718)

### How Does It Work?

- When \(z\) is very large, the sigmoid output approaches 1.
- When \(z\) is very small, the sigmoid output approaches 0.
- When \(z=0\), the sigmoid output is 0.5.

### Classification Using Threshold

A threshold is used to convert the predicted probability into a class label. The default threshold is usually **0.5**.

- If probability is greater than or equal to 0.5, classify it as **Class 1**.
- If probability is less than 0.5, classify it as **Class 0**.

**Example:**

Suppose the model predicts a probability of 0.85.

Since 0.85 is greater than 0.5, the input belongs to Class 1.

---

## Linear Regression vs Logistic Regression

| Linear Regression                    | Logistic Regression                                        |
| ------------------------------------ | ---------------------------------------------------------- |
| Used for regression problems         | Used for classification problems                           |
| Predicts continuous numerical values | Predicts class probabilities                               |
| Uses a linear prediction equation    | Uses a logistic/sigmoid function for binary classification |
| Commonly uses Mean Squared Error     | Commonly uses Log Loss                                     |
| Example: House Price Prediction      | Example: Spam Email Detection                              |

## Types of Logistic Regression

![Types of Logistic Regression](https://media.geeksforgeeks.org/wp-content/uploads/20251216101013765543/types_of_logistic_regression.webp)

Logistic Regression has three main types:

### 1. Binomial Logistic Regression

Used when the dependent variable has only two possible categories.

**Examples:**

- Yes / No
- Pass / Fail
- 0 / 1
- Spam / Not Spam

### 2. Multinomial Logistic Regression

Used when the dependent variable has three or more unordered categories.

**Examples:**

- Classifying animals as Cat, Dog, or Sheep.
- Classifying products as Electronics, Clothing, or Furniture.

### 3. Ordinal Logistic Regression

Used when the dependent variable has three or more categories with a natural order.

**Examples:**

- Low / Medium / High
- Poor / Average / Good / Excellent
- Small / Medium / Large

---

## Assumptions of Logistic Regression

1. **Independent Observations:** Each observation should be independent of the other observations.

2. **Binary Dependent Variable:** For binomial logistic regression, the target variable must have two possible values, such as 0 and 1. Multinomial and ordinal extensions handle other types of categorical targets.

3. **Linearity of Log-Odds:** There should be a linear relationship between the independent variables and the log-odds of the dependent variable.

4. **No Extreme Outliers:** Extreme outliers can affect model coefficients and reduce prediction accuracy.

5. **Large Sample Size:** A sufficiently large dataset helps produce more reliable and stable model estimates.

6. **No Perfect Multicollinearity:** Independent variables should not have perfect linear relationships with each other.

---

## Evaluation Metrics

The performance of Logistic Regression can be evaluated using the following classification metrics:

- **Accuracy:** Measures the percentage of correctly predicted observations.
- **Precision:** Measures how many predicted positive observations are actually positive.
- **Recall:** Measures how many actual positive observations are correctly identified.
- **F1-Score:** Harmonic mean of Precision and Recall.
- **Confusion Matrix:** Shows the number of correct and incorrect predictions.
- **ROC-AUC:** Measures how well the model distinguishes between different classes.

---
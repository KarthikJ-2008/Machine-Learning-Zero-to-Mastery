## 📈 What is Logistic Regression in Machine Learning?

**Logistic Regression** is a supervised machine learning algorithm used to predict categorical outcomes by calculating the probability of an input belonging to a particular class.

Despite its name, Logistic Regression is mainly used for **classification problems**, not regression.

It uses a **Sigmoid Function** to convert predicted values into probabilities between **0 and 1**.

**Examples:**
- Predicting whether an email is Spam or Not Spam
- Predicting whether a student will Pass or Fail
- Predicting whether a customer will Buy or Not Buy
- Predicting whether a transaction is Fraudulent or Genuine

## 📊 Sigmoid Function (S-Curve)

The **Sigmoid Function** is a mathematical function that converts any real number into a probability between 0 and 1.

It produces an **S-shaped curve**.

![Logistic Regression Sigmoid Curve](https://upload.wikimedia.org/wikipedia/commons/8/88/Logistic-curve.svg)

### Sigmoid Function Equation

**σ(z) = 1 / (1 + e⁻ᶻ)**

Where:
- **σ(z)** – Predicted probability
- **z** – Linear combination of input features
- **e** – Euler's number (approximately 2.718)

The linear equation is:

**z = b₀ + b₁X₁ + b₂X₂ + ... + bₙXₙ**

### Classification Threshold

Logistic Regression commonly uses a threshold of **0.5** to classify predictions.

- **Probability ≥ 0.5** → Class 1
- **Probability < 0.5** → Class 0

**Example:**

If the predicted probability of passing an exam is **0.85**, the model predicts **Pass (1)**.

If the probability is **0.25**, the model predicts **Fail (0)**.

## ⚙️ How Logistic Regression Works

**Step 1: Collect Data**

Collect input features and their corresponding class labels.

**Step 2: Preprocess Data**

Handle missing values, encode categorical variables, and scale numerical features when necessary.

**Step 3: Split the Dataset**

Divide the dataset into training and testing sets.

**Step 4: Train the Model**

The algorithm learns the coefficients and intercept from the training data.

**Step 5: Apply Sigmoid Function**

Convert the linear output into a probability between 0 and 1.

**Step 6: Classify the Output**

Use a classification threshold to assign the predicted class.

**Step 7: Evaluate the Model**

Evaluate classification performance using suitable metrics.

### 🔄 Workflow

```text
       Collect Dataset
              |
              v
       Data Preprocessing
              |
              v
        Train/Test Split
              |
              v
     Train Logistic Regression
              |
              v
       Linear Combination
              |
              v
        Sigmoid Function
              |
              v
      Probability (0 to 1)
              |
              v
     Apply Decision Threshold
              |
              v
       Predicted Class
              |
              v
       Model Evaluation
```

## 📚 Types of Logistic Regression

### 1. Binary Logistic Regression

Binary Logistic Regression is used when the target variable has **only two classes**.

**Examples:**
- Spam or Not Spam
- Pass or Fail
- Yes or No

**Output:** Class 0 or Class 1

### 2. Multinomial Logistic Regression

Multinomial Logistic Regression is used when the target variable has **more than two unordered classes**.

**Examples:**
- Predicting transport type: Car, Bus, or Bike
- Classifying fruits: Apple, Banana, or Orange

**Output:** One class among multiple categories.

### 3. Ordinal Logistic Regression

Ordinal Logistic Regression is used when the target variable has **three or more ordered categories**.

**Examples:**
- Customer satisfaction: Low, Medium, High
- Product rating: Poor, Average, Good, Excellent

**Output:** One of the ordered categories.

## 📉 Loss Function

Logistic Regression commonly uses **Log Loss (Binary Cross-Entropy)** for binary classification.

The loss function measures the difference between actual labels and predicted probabilities.

**Log Loss:**

L = -(1/n) × Σ[y log(p) + (1-y) log(1-p)]

Where:
- **n** – Number of observations
- **y** – Actual class label (0 or 1)
- **p** – Predicted probability of Class 1

The goal is to **minimize Log Loss** to improve model predictions.

## 📏 Evaluation Metrics

Logistic Regression can be evaluated using:

- **Accuracy** – Percentage of correctly classified predictions
- **Precision** – Proportion of predicted positives that are actually positive
- **Recall** – Proportion of actual positives correctly identified
- **F1-Score** – Harmonic mean of precision and recall
- **Confusion Matrix** – Shows correct and incorrect classifications
- **ROC-AUC** – Measures how well the model separates classes across different thresholds


## 🌍 Applications

- 📧 Email Spam Detection
- 🏦 Fraud Detection
- 🎓 Student Placement Prediction
- 🛒 Customer Purchase Prediction
- 📉 Customer Churn Prediction
- 🏥 Disease Risk Classification

## 🔍 Linear Regression vs Logistic Regression

| Linear Regression | Logistic Regression |
|---|---|
| Used for regression problems | Used for classification problems |
| Predicts continuous numerical values | Predicts class probabilities |
| Uses a linear prediction equation | Uses a logistic/sigmoid function for binary classification |
| Commonly uses Mean Squared Error | Commonly uses Log Loss |
| Example: House Price Prediction | Example: Spam Email Detection |

## ⭐ Support

If you find this repository useful for learning Machine Learning, consider giving it a **⭐ Star** on main repository!

---

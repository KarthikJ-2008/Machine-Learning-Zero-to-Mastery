
# 📈 Linear Regression – Machine Learning

A beginner-friendly guide to understanding **Linear Regression**, one of the simplest and most important supervised machine learning algorithms.

## 📌 What is Linear Regression?

**Linear Regression** is a supervised machine learning algorithm used to predict continuous numerical values by finding a linear relationship between input and output variables.

It finds the **best-fit straight line** through the data points to make predictions.

**Example:**
- Predicting house prices based on area
- Predicting student marks based on study hours
- Predicting salary based on years of experience

## 📊 Best Fit Line

The **best-fit line** is a straight line that represents the relationship between input (X) and output (Y) values.

The main goal is to find a line that minimizes the difference between actual and predicted values.

![Linear Regression Best Fit Line](https://upload.wikimedia.org/wikipedia/commons/3/3a/Linear_regression.svg)

### Linear Regression Equation

**Y = mX + c**

Where:
- **Y** – Predicted output
- **X** – Input feature
- **m** – Slope of the line
- **c** – Intercept (value of Y when X = 0)

## ⚙️ How Linear Regression Works

**Step 1: Collect Data**

Collect input and output data, such as study hours and exam marks.

**Step 2: Plot Data Points**

Plot the data points on a graph to understand their relationship.

**Step 3: Find the Best-Fit Line**

The algorithm finds the straight line that minimizes prediction errors, usually using the least squares method.

**Step 4: Train the Model**

The model learns the slope and intercept from the training data.

**Step 5: Make Predictions**

The trained model predicts output values for new inputs.

### 🔄 Workflow

```text
      Collect Dataset
            |
            v
      Preprocess Data
            |
            v
      Train/Test Split
            |
            v
    Train Linear Regression
            |
            v
      Find Best-Fit Line
            |
            v
       Make Predictions
            |
            v
      Evaluate Model
```

## 📚 Types of Linear Regression

### 1. Simple Linear Regression

Simple Linear Regression uses **one independent variable** to predict a dependent variable.

**Example:** Predicting salary based on years of experience.

**Equation:**

Y = mX + c

### 2. Multiple Linear Regression

Multiple Linear Regression uses **two or more independent variables** to predict a dependent variable.

**Example:** Predicting house prices based on area, number of bedrooms, and age of the house.

**Equation:**

Y = b₀ + b₁X₁ + b₂X₂ + ... + bₙXₙ

Where:
- **b₀** – Intercept
- **b₁, b₂, ...** – Regression coefficients
- **X₁, X₂, ...** – Input features

## 📉 Cost Function

Linear Regression commonly uses **Mean Squared Error (MSE)** to measure prediction errors.

**MSE = (1/n) × Σ(Actual − Predicted)²**

The goal is to minimize the MSE and find the best-fit line.

## 📏 Evaluation Metrics

- **MAE** – Mean Absolute Error
- **MSE** – Mean Squared Error
- **RMSE** – Root Mean Squared Error
- **R² Score** – Measures how well the model explains variation in the output

## 🌍 Applications

- 🏠 House Price Prediction
- 💰 Salary Prediction
- 📊 Sales Forecasting
- 🎓 Student Marks Prediction
- 📈 Business Trend Analysis
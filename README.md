# Titanic Survival Prediction Challenge

## 📋 Overview

You are a Data Scientist at **Maritime Safety Analytics**, a consulting firm specializing in passenger safety systems. A major cruise line company has approached you with a critical request:

The company is developing a new **emergency response AI system** that needs to predict passenger survival likelihood during maritime emergencies. Your task is to build a classification model using historical maritime incident data and predict survival outcomes for passengers in an emergency scenario.

---

## 📊 Dataset Description

### Training Data: `data/train.csv`

This dataset contains historical maritime incident data with known survival outcomes for each passenger.

#### Features:

| Feature | Description |
|---------|-------------|
| **Survived** | Target variable (0 = died, 1 = survived) |
| **Pclass** | Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd) |
| **Sex** | Gender of the passenger |
| **Age** | Age of the passenger in years |
| **SibSp** | Number of siblings/spouses aboard |
| **Parch** | Number of parents/children aboard |
| **Fare** | Passenger fare |
| **Embarked** | Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton) |

### Test Data: `data/test_inputs.csv`

This dataset contains features for passengers in a recent emergency scenario. Your model must predict survival outcomes for these passengers.

---

## 🎓 Challenge Requirements

### 1. Model Development

Build a Machine Learning classification model using the training data to predict passenger survival outcomes.

### 2. Evaluation Criteria

Your model will be evaluated based on **F1 Score**:

- **Minimum F1 Score Required: 0.70**

### 3. Prediction Output

Your predictions must be stored in a variable called `predictions` as a NumPy array:

```python
predictions = array([0, 0, 0, 0, 1, 0, ...])

# Task 6: K-Nearest Neighbors (KNN) Classification

---

## 🎯 **Objective**
Implement **K-Nearest Neighbors** for multi-class classification using the classic **Iris Dataset**.
- Normalize features to work with distance metrics.
- Train KNN models for different values of **K**.
- Evaluate accuracy and performance.
- Visualize **decision boundaries** to see how KNN classifies new points.
- Understand how **instance-based learning** and **Euclidean distance** work.

---

## 📁 **Dataset**
- **Name:** Iris Species
- **Source:** [Kaggle Iris Dataset](https://www.kaggle.com/datasets/uciml/iris)
- **File Used:** `Iris.csv`
- **Classes:** `Iris-setosa`, `Iris-versicolor`, `Iris-virginica`

---

## ✅ **What I Did**

### 1️⃣ Data Preparation
- Loaded the Iris dataset with 150 samples and 4 features.
- Checked for missing values (none found).
- Selected **features**: `sepal length`, `sepal width`, `petal length`, `petal width`.
- Encoded the **target**: `Species` with 3 labels.
- Normalized all features using **StandardScaler** to ensure distance calculations are fair.

---

### 2️⃣ KNN Model
- Used **`KNeighborsClassifier`** from scikit-learn.
- Split the data: 80% training, 20% testing.
- Trained the initial KNN with **K = 3**.

---

### 3️⃣ Model Evaluation
- Evaluated using **accuracy**, **confusion matrix**, and **classification report**.
- **Initial accuracy** for K = 3:  
  ✅ ~96% on test data.
- Confusion matrix showed almost perfect classification for all three species.

---

### 4️⃣ K Value Testing
- Ran experiments for **odd K values from 1 to 19**.
- Plotted **Error Rate vs. K**.
- Found best K with minimum error was around **K = 5 or 7** for stable performance.

---

### 5️⃣ Decision Boundary Visualization
- For clear visuals, selected **2 features**: `PetalLengthCm` and `PetalWidthCm`.
- Trained KNN with K = 5 on these two features.
- Plotted **2D decision boundary**:
  - Regions clearly showed **three separate areas** for each species.
  - The scatter plot confirmed how test samples fall within the correct class regions.

---

## 📊 **Key Outputs**
- **Accuracy:** ~96% (high accuracy due to well-separated Iris classes).
- **Confusion Matrix:** Clear class separations with very few or no misclassifications.
- **Error vs. K Plot:** Shows how increasing K reduces variance but too large K can reduce accuracy.
- **Decision Boundary Plot:** Clearly illustrates KNN’s instance-based decision logic.

---

## 📌 **Concepts Covered**
- **Instance-based learning:** KNN stores all training data, no training equation.
- **Euclidean distance:** Used to find nearest neighbors.
- **K selection:** Demonstrated effect of K on model performance and bias-variance tradeoff.
- **Decision Boundaries:** Show how KNN divides feature space.

---

## 📚 **Tools Used**
- Python
- Pandas
- scikit-learn
- Matplotlib
- Seaborn

---



The KNN classifier predicts Iris species accurately, demonstrates how to normalize features, experiment with K values, and visualize decision boundaries for clear interpretation of how the model works.




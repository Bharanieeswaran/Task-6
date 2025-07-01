# 📊 Task 6: K-Nearest Neighbors (KNN) Classification

**AI & ML Internship Project**  
Implemented using: Scikit-learn, Pandas, Matplotlib, NumPy

---

## ✅ Objective

The goal of this task is to understand and implement the **K-Nearest Neighbors (KNN)** algorithm for a classification problem using the **Iris Dataset**.

---

## 🛠️ Tools & Libraries Used

- Python
- Scikit-learn
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

## 📁 Files Included

- `knn_classification.ipynb` – Main code notebook
- `README.md` – Project documentation

---

## 📌 Key Concepts Covered

- **Instance-based learning**
- **Euclidean distance**
- **Effect of K-value selection**
- **Feature normalization**
- **Confusion matrix and accuracy evaluation**
- **K vs Accuracy graph**
- (Optional) Decision boundary visualization for 2D data

---

## 📈 Workflow Steps

1. **Load Dataset**  
   Used the built-in Iris dataset from `sklearn.datasets`.

2. **Normalize Features**  
   Applied `StandardScaler` to standardize feature values (important for KNN).

3. **Train-Test Split**  
   Split the dataset into 80% training and 20% testing data.

4. **Train the KNN Classifier**  
   Used `KNeighborsClassifier` with various values of `k` (1 to 10).

5. **Evaluate the Model**  
   Measured performance using:
   - Accuracy
   - Confusion Matrix
   - Classification Report

6. **Visualizations**  
   - Plotted **Accuracy vs K**
   - (Optional) Visualized 2D **decision boundaries** using the first two features

---

## 📊 Results

| K Value | Accuracy (%) |
|--------:|--------------|
| 1       | 96.67        |
| 3       | 100.00       |
| 5       | 96.67        |
| 7       | 96.67        |
| 9       | 96.67        |

- **Best Accuracy**: Achieved at **K = 3**

---

## 🧠 Interview Questions & Answers

1. **How does the KNN algorithm work?**  
   KNN classifies a data point by looking at the 'K' nearest labeled training examples and choosing the majority class among them.

2. **How do you choose the right K?**  
   By plotting validation accuracy for different values of K and selecting the one with the best performance.

3. **Why is normalization important in KNN?**  
   KNN is distance-based; features on different scales can bias the model if not normalized.

4. **What is the time complexity of KNN?**  
   **O(n × d)** per query, where `n` = number of training samples and `d` = number of features.

5. **What are pros and cons of KNN?**  
   ✅ Simple and effective  
   ❌ Slow with large datasets, sensitive to irrelevant/noisy features

6. **Is KNN sensitive to noise?**  
   Yes. Outliers and noise can affect the voting result significantly.

7. **How does KNN handle multi-class problems?**  
   It supports multi-class classification by majority vote among the K neighbors.

8. **What’s the role of distance metrics in KNN?**  
   Distance metrics (like Euclidean, Manhattan) determine which neighbors are considered "closest".

---

## 📌 Conclusion

- KNN is a simple yet powerful classification algorithm.
- Proper **feature scaling** and **k selection** are crucial.
- Visualizations help in better understanding the decision boundaries and model behavior.

---

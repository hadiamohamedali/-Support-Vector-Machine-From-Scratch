# 🚀 Support Vector Machine (SVM) from Scratch

A **Linear Support Vector Machine (SVM)** implemented from scratch using **NumPy**. This project demonstrates how SVM learns the optimal separating hyperplane using **Gradient Descent** without relying on machine learning libraries for the model implementation.

---

## ✨ Features

- 📌 Linear SVM implementation from scratch
- 🧮 Gradient Descent optimization
- 🛡️ L2 Regularization
- 📈 Prediction using the learned hyperplane
- 📊 Decision boundary visualization
- 🎯 Synthetic dataset generation with Scikit-learn

---

## 📂 Project Structure

```
.
├── svm.py
└── README.md
```

---

## 📦 Requirements

Install the required libraries:

```bash
pip install numpy matplotlib scikit-learn
```

---

## 🧠 Algorithm

The classifier learns the hyperplane:

\[
w \cdot x - b = 0
\]

Where:

- ⚖️ **w** → Weight vector
- 📍 **b** → Bias
- 📊 **x** → Feature vector

Labels are converted to:

- 🔴 **-1**
- 🟢 **+1**

The model minimizes the **Hinge Loss** with **L2 Regularization**.

---

## 🚀 Training

```python
clf = svm(
    learning_rate=0.001,
    lambda_param=0.01,
    n_iters=1000
)

clf.fit(X, y)
```

---

## 🔮 Prediction

```python
predictions = clf.predict(X)
```

Returns:

- 🔴 -1
- 🟢 +1

---

## 📊 Visualization

The project visualizes:

- 🔵 Training samples
- 📏 Decision boundary
- ➕ Positive margin
- ➖ Negative margin

---

## ⚙️ Hyperparameters

| Parameter | Description | Default |
|-----------|-------------|---------|
| 📉 learning_rate | Gradient descent learning rate | 0.001 |
| 🛡️ lambda_param | Regularization strength | 0.01 |
| 🔄 n_iters | Number of training iterations | 1000 |

---

## 🛠️ Methods

### 📌 `fit(X, y)`

Trains the SVM model.

---

### 🎯 `predict(X)`

Predicts the class labels for new samples.

Returns:

- 🔴 -1
- 🟢 +1

---

## 📚 Dataset

Generated using:

```python
datasets.make_blobs()
```

Configuration:

- 📄 50 samples
- 📌 2 features
- 🎯 2 classes
- 🎲 Random state = 40

---

## 📚 Libraries Used

- 🧮 NumPy
- 📊 Matplotlib
- 🤖 Scikit-learn *(dataset generation only)*

---

## 🎓 Learning Objectives

This project demonstrates:

- 🧠 Linear Classification
- 📏 Maximum Margin
- 📉 Hinge Loss
- ⚡ Gradient Descent
- 🛡️ Regularization
- 📊 Decision Boundary Visualization
- 💻 Building Machine Learning algorithms from scratch

---

## 🚀 Future Improvements

- 🌟 Soft Margin SVM
- 🌟 Kernel SVM
- 🌟 Polynomial Kernel
- 🌟 RBF Kernel
- 🌟 Accuracy Evaluation
- 🌟 Support Vector Identification
- 🌟 Model Saving & Loading

---

## 👩‍💻 Author

**Hadia Mohamed**

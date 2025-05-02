# Task_6
Iris flower classification using the K-Nearest Neighbors (KNN) algorithm. Includes data preprocessing, evaluation with multiple K values, confusion matrix, and 2D decision boundary visualization.
#Iris Flower Classification using K-Nearest Neighbors (KNN)

This project implements the **K-Nearest Neighbors (KNN)** algorithm to classify **Iris flowers** into three species based on their sepal and petal dimensions.

This project is part of **Task 6** of the **AI & ML Internship Program**.

---

##Dataset Details

- **Dataset**: Iris Dataset (`Iris.csv`)
- **Records**: 150 flower samples
- **Classes**:
  - `Iris-setosa`
  - `Iris-versicolor`
  - `Iris-virginica`
- **Features**:
  - `SepalLengthCm`
  - `SepalWidthCm`
  - `PetalLengthCm`
  - `PetalWidthCm`

---

##Objectives

- Preprocess and encode the dataset
- Normalize the features
- Train and test a **KNN classifier**
- Evaluate model accuracy for different values of **K**
- Identify the best-performing K
- Visualize classification decision boundaries (2D)
- Interpret model performance using:
  - Confusion Matrix
  - Classification Report

---

##Tools and Libraries

- Python 3.x
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

---

##Project Workflow

### ✅ Step 1: Data Preprocessing
- Removed the `Id` column
- Converted `Species` labels into numerical categories
- Split the dataset into training and testing sets

### ✅ Step 2: Feature Scaling
- Standardized all features using `StandardScaler`

### ✅ Step 3: KNN Classification
- Trained `KNeighborsClassifier` on the training set
- Evaluated test accuracy for **K = 1 to 10**
- Plotted accuracy vs. K graph

### ✅ Step 4: Final Model Selection
- Chose the **best K** based on accuracy
- Evaluated using:
  - Confusion Matrix
  - Classification Report

### ✅ Step 5: Bonus Visualization
- Plotted **2D decision boundary** using `PetalLength` and `PetalWidth` features

---

##Model Performance

- **Best Accuracy**: ~100% for `K = 3` (may vary slightly on re-runs)
- **Classes Well Separated**: KNN performs well on this clean and balanced dataset

---

##Files Included

| File Name | Description |
|-----------|-------------|
| `Iris_KNN_Classification.ipynb` | Jupyter Notebook with full implementation |
| `Iris.csv` | Iris dataset |
| `README.md` | This file |

---

##How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/iris-knn-classification.git
   cd iris-knn-classification

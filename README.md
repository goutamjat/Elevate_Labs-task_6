# 🌸 K-Nearest Neighbors (KNN) Classification - Iris Dataset

## 📌 Objective
To implement the K-Nearest Neighbors (KNN) algorithm on the Iris dataset and evaluate its classification performance, including visualization of decision boundaries.

---

## 🧰 Tools & Libraries Used
- Python
- `pandas`, `numpy`
- `matplotlib`, `seaborn`
- `scikit-learn`

---

## 📁 Files Included
| File Name            | Description                                 |
|----------------------|---------------------------------------------|
| `Iris.csv`           | Original dataset used for training/testing  |
| `Task6_Intern.ipynb` | Jupyter Notebook containing all code, plots, and outputs |

---

## 📊 Dataset Information
The dataset contains **150 samples** of iris flowers classified into 3 species:
- *Iris-setosa*
- *Iris-versicolor*
- *Iris-virginica*

Each sample contains 4 features:
- SepalLengthCm
- SepalWidthCm
- PetalLengthCm
- PetalWidthCm

---

## 🧪 Steps Performed

### ✅ 1. Data Loading & Preprocessing
- Loaded the Iris dataset from `Iris.csv`
- Removed the unnecessary `Id` column
- Normalized the feature data using `StandardScaler`

### ✅ 2. Train-Test Split
- Split the dataset into 80% training and 20% testing
- Stratified split used to maintain class balance

### ✅ 3. KNN Model Training
- Used `KNeighborsClassifier` from `sklearn`
- Experimented with K values from 1 to 20
- Selected the **optimal K = 1** based on lowest error rate

### ✅ 4. Model Evaluation
- Evaluated using accuracy, confusion matrix, and classification report

**Final Evaluation Results:**

```
Optimal K is: 1
Accuracy: 0.9666666666666667

Confusion Matrix:
[[10  0  0]
 [ 0 10  0]
 [ 0  1  9]]

Classification Report:
                  precision    recall  f1-score   support

    Iris-setosa       1.00      1.00      1.00        10
Iris-versicolor       0.91      1.00      0.95        10
 Iris-virginica       1.00      0.90      0.95        10

       accuracy                           0.97        30
      macro avg       0.97      0.97      0.97        30
   weighted avg       0.97      0.97      0.97        30
```

### ✅ 5. Visualization
- Plotted **error rate vs K** to choose optimal K
- Visualized **decision boundaries** using `PetalLengthCm` and `PetalWidthCm`

---

## 📌 How to Run

1. Clone the repository or download the files.
2. Make sure you have Python installed with the following libraries:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```
3. Open `Task6_Intern.ipynb` in Jupyter Notebook or any compatible IDE.
4. Run all the cells sequentially.

---

## 📈 Sample Plots Included
- Error Rate vs. K
- Confusion Matrix
- KNN Decision Boundary using 2 Features

---

## ✍️ Author
**Your Name**

---

## ✅ Status
✔️ Completed as part of internship Task 6: KNN Classification

# 🌸 Iris Flower Classification using Neural Networks (MLP)
 
A beginner-friendly machine learning project that classifies Iris flower species using a **Multi-Layer Perceptron (MLPClassifier)** from scikit-learn, paired with exploratory data analysis and visualizations.
 
---
 
## 📌 Objective
 
To classify Iris flower species (*Setosa*, *Versicolor*, *Virginica*) using a neural network model and analyze feature relationships through data visualization.
 
---
 
## 📂 Project Structure
 
```
Day1_MLP_Project.ipynb   # Main Jupyter Notebook
README.md                # Project documentation
```
 
---
 
## 🛠️ Tech Stack
 
| Library | Purpose |
|---|---|
| `numpy` | Numerical operations |
| `pandas` | Data manipulation |
| `matplotlib` | Plotting |
| `seaborn` | Statistical visualizations |
| `scikit-learn` | Dataset, preprocessing, model, evaluation |
 
---
 
## 📊 Dataset
 
- **Source:** `sklearn.datasets.load_iris` (built-in dataset)
- **Samples:** 150
- **Features:** Sepal length, Sepal width, Petal length, Petal width (all in cm)
- **Target Classes:** 3 (Setosa = 0, Versicolor = 1, Virginica = 2)
- **Missing Values:** None
---
 
## 📈 Exploratory Data Analysis
 
Five charts are created to understand the data:
 
1. **Pairplot** — Shows class separability; petal features clearly separate species
2. **Heatmap** — Reveals high correlation between petal length and petal width
3. **Boxplot** — Displays feature distributions; few outliers present
4. **Histogram** — Shows different distributions across measurements
5. **Countplot** — Confirms balanced class distribution (50 samples each)
---
 
## 🧠 Model
 
- **Algorithm:** `MLPClassifier` (Multi-Layer Perceptron)
- **Architecture:** 2 hidden layers with 10 neurons each — `hidden_layer_sizes=(10, 10)`
- **Max Iterations:** 1000
- **Random State:** 42
---
 
## 🔄 Pipeline
 
```
Load Data → EDA & Visualization → Train/Test Split (80/20)
→ Feature Scaling (StandardScaler) → Train MLP → Evaluate
```
 
> ⚠️ `fit_transform()` is applied **only on training data**; `transform()` on test data to prevent data leakage.
 
---
 
## ✅ Evaluation Metrics
 
- Accuracy Score
- Classification Report (Precision, Recall, F1-score)
- Confusion Matrix (visualized as heatmap)
---
 
## 🚀 Getting Started
 
### Prerequisites
 
```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
```
 
### Run the Notebook
 
```bash
jupyter notebook Day1_MLP_Project.ipynb
```
 
---
 
## 💡 Key Insight
 
> *"The most surprising thing found in this data was how clearly petal features separate the flower species."*
 
Petal length and petal width are the most discriminative features for classifying Iris species.
 
---
 
## 📝 License
 
This project is open-source and free to use for learning purposes.

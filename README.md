# 🌸 Iris Species Classifier — Machine Learning Demo

A Machine Learning project that trains a model to identify the species of an Iris flower based on its physical measurements.

## 📋 About

This project was developed as part of the **Oracle Cloud Infrastructure (OCI)** course and demonstrates the complete Machine Learning workflow, from loading data to making predictions.

## 🔄 Project Flow

```
Load Data → Preprocess → Train Model → Evaluate → Predict
```

## 📊 Dataset

The dataset used is the famous **Iris Dataset**, containing 150 flower samples from 3 different species:

- 🌸 *Iris Setosa*
- 🌺 *Iris Versicolor*
- 🌼 *Iris Virginica*

Each sample has 4 features:

| Feature | Description |
|---|---|
| `sepal_length` | Sepal length (cm) |
| `sepal_width` | Sepal width (cm) |
| `petal_length` | Petal length (cm) |
| `petal_width` | Petal width (cm) |

## 🛠️ Technologies

- **Python 3.13**
- **Pandas** — data manipulation
- **Scikit-learn** — Machine Learning model
- **Jupyter Notebook** — development environment

## ⚙️ How to Run

### 1. Clone the repository
```bash
git clone https://github.com/your-username/ml-iris-demo.git
cd ml-iris-demo
```

### 2. Install dependencies
```bash
conda install pandas scikit-learn
```

### 3. Open the notebook
```bash
jupyter notebook MLDemo1.ipynb
```

### 4. Run all cells in order

> The `iris.csv` dataset is downloaded automatically by the notebook — no manual download needed.

## 🤖 Model

The algorithm used is **Logistic Regression**, a classifier that learns patterns from training data and can predict the species of new flowers.

```python
model = LogisticRegression(max_iter=200)
model.fit(X, y)
```

## 🔮 Prediction Example

```python
new_flower = pd.DataFrame([[5.1, 3.5, 1.4, 0.2]], 
              columns=['sepal_length', 'sepal_width', 'petal_length', 'petal_width'])

model.predict(new_flower)
# Output: array(['setosa'])
```

## 📁 Project Structure

```
ml-iris-demo/
├── MLDemo1.ipynb   # Main notebook
├── iris.csv        # Dataset
└── README.md       # This file
```

## 👨‍💻 Author

Developed during the Oracle Cloud Infrastructure (OCI) course.

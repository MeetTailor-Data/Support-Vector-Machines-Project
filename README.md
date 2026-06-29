# Support Vector Machines Project

## Project Description

This project implements a Support Vector Machine (SVM) classifier on the Iris dataset using Scikit-learn. The objective is to classify iris flowers into their respective species and improve the model's performance using hyperparameter tuning with Grid Search.

---

## Dataset

Dataset: Iris Dataset (loaded using Seaborn)

Target Variable:

* `species`

Features:

* sepal_length
* sepal_width
* petal_length
* petal_width

---

## Project Workflow

### Exploratory Data Analysis (EDA)

The notebook includes:

* Displaying sample images of the three Iris species:

  * Iris Setosa
  * Iris Versicolor
  * Iris Virginica
* Loading the Iris dataset using Seaborn.
* Viewing dataset information using `info()`.
* Pairplot visualization with species as the hue.
* KDE plot for the Setosa species using:

  * Sepal Width
  * Sepal Length

---

## Train-Test Split

* Features (`X`): All feature columns except `species`
* Target (`y`): `species`
* Test Size: 30%

---

## Machine Learning Model

Algorithm:

* Support Vector Classifier (SVC)

Steps:

1. Train the SVC model on the training dataset.
2. Predict the species on the test dataset.
3. Evaluate model performance.

---

## Model Evaluation

The model was evaluated using:

* Confusion Matrix
* Classification Report

---

## Hyperparameter Tuning

The notebook improves the model using `GridSearchCV`.

Parameter Grid:

```python
param_grid = {
    'C': [0.1, 1, 10, 100],
    'gamma': [1, 0.1, 0.01, 0.001]
}
```

After Grid Search:

* Best model is trained automatically (`refit=True`).
* Predictions are generated on the test dataset.
* Performance is evaluated again using:

  * Confusion Matrix
  * Classification Report

---

## Concepts Used

* Exploratory Data Analysis (EDA)
* Pairplot
* KDE Plot
* Train-Test Split
* Support Vector Machine (SVM)
* Support Vector Classifier (SVC)
* GridSearchCV
* Hyperparameter Tuning
* Confusion Matrix
* Classification Report

---

## Project Structure

```text
Support-Vector-Machines-Project/
│
├── 02-Support Vector Machines Project.ipynb
└── README.md
```

---

## Requirements

* Python 3.x
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

## How to Run

1. Clone this repository.
2. Open `02-Support Vector Machines Project.ipynb`.
3. Run all cells from top to bottom.

---

## Author

Meet Tailor — Data Science Learner

GitHub: https://github.com/MeetTailor-Data

---

## License

Created for learning and educational purposes only.

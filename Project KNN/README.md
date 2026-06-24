# 🚢 Titanic Survival Prediction

A machine learning project that predicts whether a passenger survived the Titanic disaster, based on features like age, sex, passenger class, and fare. Built as an end-to-end binary classification workflow.

## 📊 Results

| Model | Accuracy |
|-------|----------|
| KNN | 80.6% |
| Decision Tree | 80.2% |
| **SVM (best)** | **81.7%** |

> Baseline (always guessing "died") would be ~62%, so the models clearly learned real patterns from the data.

## 🔑 Key Insights

- **Sex** was the strongest predictor — females had a far higher survival rate ("women and children first").
- **Passenger class** mattered — 1st class passengers survived at a much higher rate than 3rd class.
- **Age** played a role — children had a relatively higher chance of survival.

## 🛠️ Workflow

1. **Data exploration** — inspect structure, data types, and missing values
2. **EDA** — visualize survival patterns by sex, class, and age
3. **Data cleaning** — handle missing values, encode categorical features, drop noise columns
4. **Preprocessing** — train/test split + feature scaling (avoiding data leakage)
5. **Modeling** — train & compare KNN, Decision Tree, and SVM
6. **Evaluation** — accuracy, confusion matrix, classification report

## 💻 Tech Stack

- Python
- pandas, NumPy
- matplotlib, seaborn
- scikit-learn

## 🚀 How to Run

```bash
# install dependencies
pip install -r requirements.txt

# open the notebook
jupyter notebook Titanic_Survival_Prediction.ipynb
```

Make sure `Titanic-Dataset.csv` is in the same folder as the notebook.

## 📁 Files

- `Titanic_Survival_Prediction.ipynb` — main notebook (analysis + models)
- `Titanic-Dataset.csv` — the dataset
- `requirements.txt` — dependencies

## 📌 Possible Improvements

- Feature engineering (e.g. combine `SibSp` + `Parch` into "family size")
- Hyperparameter tuning with `GridSearchCV`
- Try ensemble models (Random Forest, Gradient Boosting)

---

*This project was built as part of my machine learning learning journey, demonstrating a complete supervised-learning pipeline on a real, messy dataset.*

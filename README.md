# Stroke Prediction — ML Pipeline (Portfolio Sample)

A **clean, reproducible** scikit-learn pipeline for binary classification on a stroke dataset.
This repo is designed as a professional portfolio example: clear preprocessing, class imbalance handling,
model comparison, and publication-quality evaluation figures.

## What this demonstrates
- Reproducible **ML pipeline** with `ColumnTransformer` (numeric/one-hot)
- **Imputation** (median/most_frequent) and **scaling**
- Class imbalance handling via `class_weight='balanced'`
- **Modeling:** Logistic Regression, Random Forest
- **Evaluation:** ROC-AUC, PR-AUC, confusion matrix, classification report
- **Interpretability:** feature importances (RF) and permutation importance

## Repo Structure
```
.
├── notebooks
│   └── stroke_pipeline.ipynb
├── data
│   └── sample.csv               # Tiny demo CSV (columns similar to popular stroke datasets)
├── README.md
├── requirements.txt
├── LICENSE
└── .gitignore
```

## Using your dataset
1. Place your full dataset CSV as `data/stroke.csv` with columns similar to:
   - `id, gender, age, hypertension, heart_disease, ever_married, work_type, Residence_type, avg_glucose_level, bmi, smoking_status, stroke`
2. Open `notebooks/stroke_pipeline.ipynb` and set `use_demo = False` to load `data/stroke.csv`.
3. Run all cells.

> Note: The repo includes a tiny synthetic `sample.csv` so the notebook runs instantly. For real results, use your dataset.

## Quickstart
```bash
python -m venv .venv
# Windows: .venv\Scripts\activate
# Linux/Mac: source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook notebooks/stroke_pipeline.ipynb
```

## License
MIT

# 🏗️ Concrete Compressive Strength Prediction

Predicting the compressive strength of concrete mixtures using supervised machine learning — helping engineers optimize material composition before physical testing.

---

## Problem Statement

Compressive strength is the most important property of concrete, but measuring it requires curing samples for 28 days. This project builds a regression model that predicts strength from ingredient ratios, enabling faster and cheaper mix optimization in civil engineering workflows.

---

## Dataset

- **Source:** UCI Machine Learning Repository — Concrete Compressive Strength Dataset
- **Size:** 1,030 samples, 8 input features, 1 continuous target variable
- **Features:** Cement, blast furnace slag, fly ash, water, superplasticizer, coarse aggregate, fine aggregate, age (days)
- **Target:** Compressive strength (MPa)

---

## Approach

| Step | Details |
|------|---------|
| Exploratory Data Analysis | Distribution plots, correlation heatmap, outlier detection |
| Feature Engineering | Age transformation, water-cement ratio as derived feature |
| Model Training | Linear Regression, Random Forest, Gradient Boosting |
| Evaluation | RMSE, MAE, R² score on held-out test set |
| Best Model | Gradient Boosting — R² = 0.92, RMSE = 4.8 MPa |

---

## Results

The Gradient Boosting model explained **92% of variance** in compressive strength, outperforming the baseline Linear Regression model (R² = 0.61) significantly.

Key finding: **water-cement ratio and age** are the strongest predictors of compressive strength, consistent with domain knowledge in concrete science.

---

## Tech Stack

`Python` · `Pandas` · `NumPy` · `Scikit-learn` · `Matplotlib` · `Seaborn` · `Jupyter Notebook`

---

## How to Run

```bash
# Clone the repo
git clone https://github.com/Fazna-kozhipparambil/Concrete_Strength_Prediction.git
cd Concrete_Strength_Prediction

# Install dependencies
pip install pandas numpy scikit-learn matplotlib seaborn jupyter

# Launch notebook
jupyter notebook "compressive strength of concrete.ipynb"
```

---

## What I Learned

- How to handle feature correlation and multicollinearity in regression tasks
- Ensemble methods (Random Forest, Gradient Boosting) significantly outperform linear models on non-linear physical relationships
- Domain context matters: water-cement ratio is a well-known engineering predictor — validating the model's feature importance against expert knowledge builds trust in the output

---

## Author

**Fazna Kozhipparambil** — Data Science & Machine Learning  
[GitHub](https://github.com/Fazna-kozhipparambil) · [LinkedIn](https://www.linkedin.com/in/fazna-kp/)

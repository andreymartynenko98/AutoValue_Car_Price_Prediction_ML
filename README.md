# CleanRooms: Tabular ML with Scikit‑Learn

This repository contains **Project One** for my portfolio: an end‑to‑end machine‑learning analysis implemented in a Jupyter notebook using **Python** and **scikit‑learn**. The project focuses on a tabular dataset (e.g., sourced from the UCI Machine Learning Repository) and demonstrates a clear workflow from exploratory analysis to model training and evaluation.

> Notebook file: `ProjectOne_ML.ipynb`

---

## 📌 Edited Assignment Requirements (No Video)

**Goal.** Use a dataset that I have **not** previously used in this course (i.e., not the dataset from the prior 5–7 minute presentation and not my main course project dataset). A good source is the **UCI Machine Learning Repository**.

**Deliverables.**
1. A Jupyter notebook (`ProjectOne_ML.ipynb`) that:
   - Loads and explores the dataset (EDA, handling missing values, feature preparation).
   - Implements **at least two** machine‑learning models (e.g., decision tree, SVM, neural network, naïve Bayes, clustering, or other appropriate models) and **justifies** the algorithm choices based on the **data characteristics** and/or **domain**.
   - Clearly calls out **three course concepts** applied in the analysis. Each concept should be explicitly labeled in the notebook (e.g., **Concept #1:** “When the dependent variable is skewed, evaluate with a confusion matrix and class‑wise metrics, not only accuracy.”). These must be **my own independent analysis**.
2. A `README.md` (this file) summarizing the project, environment setup, how to run the notebook, and results.
3. `requirements.txt` (and optional `environment.yml`) for reproducibility.
4. The repository should be original work; do not reuse another student’s concepts or analysis.

**Removed requirement.**
- The original requirement to **create and upload a video** is **omitted**. All demonstration and explanations are provided inside the notebook and this README.

---

## 🧠 Project Overview

- **Objective.** Build and compare regression models to predict **used car prices**.
- **Dataset.** A tabular car listings dataset (e.g., make, model, year, mileage, transmission, fuel type, condition, region). Use a dataset **not** previously used in this course.
- **Problem type.** **Regression** (target = price). If price has heavy tails or outliers, consider robust metrics (MAE, MedAE) and transformations (log-price).
- **Models to consider.** Linear Regression (with regularization), Random Forest Regressor, Gradient Boosting (e.g., XGBoost/LightGBM if allowed), SVR, MLPRegressor.
- **Key concepts (examples).**
  - **Concept #1 (Data leakage prevention via proper CV and preprocessing pipelines).**
  - **Concept #2 (Feature encoding & scaling for mixed numeric/categorical data).**
  - **Concept #3 (Evaluation with regression metrics beyond R²—MAE, RMSE, MedAE).**

> Replace the placeholders above with the specifics of your chosen car dataset and final chosen models.

---


## 🔧 Setup

### Option A — `pip`

```bash
# from repo root
python -m venv .venv
# Windows: .venv\Scripts\activate
# macOS/Linux:
source .venv/bin/activate

pip install --upgrade pip
pip install -r requirements.txt

jupyter notebook
# Open ProjectOne_ML.ipynb
```

### Option B — Conda

```bash
conda env create -f environment.yml
conda activate project-one-ml
jupyter notebook
```

---

## ▶️ How to Run

1. Activate your environment (pip or conda).
2. Launch Jupyter and open `ProjectOne_ML.ipynb`.
3. Run the cells sequentially. Fill in any dataset‑specific steps (path, preprocessing) and ensure figures are saved to `figures/` if desired.

---

## 📂 Repository Structure

```
.
├── ProjectOne_ML.ipynb      # Main notebook (provided)
├── data/                    # Optional sample/synthetic data (empty placeholder)
├── figures/                 # Exported charts (empty placeholder)
├── requirements.txt         # Python dependencies
├── environment.yml          # Conda environment (optional)
├── .gitignore               # Ignore caches, venvs, checkpoints, outputs
├── LICENSE                  # MIT
└── README.md                # This file
```

---

## ✅ Submission / Portfolio Checklist

- [ ] Notebook executes top‑to‑bottom without errors.
- [ ] At least **two ML models** implemented with **justification**.
- [ ] **Three course concepts** clearly labeled and explained.
- [ ] `requirements.txt` accurate; `environment.yml` optional but current.
- [ ] README updated with dataset details, results, and next steps.
- [ ] Repo public and linked from the portfolio website.

---

## 🔒 License

Released under the **MIT License** (see `LICENSE`).

© 2025 Andrey Martynenko

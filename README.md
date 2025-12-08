# Spotify Popularity Analysis

This project investigates which musical attributes are most associated with track popularity on Spotify.  
Using exploratory data analysis, PCA, hierarchical clustering, linear regression, and XGBoost, the analysis evaluates how audio features relate to popularity and how well they can be used to predict it.

---

## 📊 Contents
- `notebooks/main_report.ipynb` — Full workflow and main analysis
- `notebooks/eda_supporting_material.ipynb` — Extended EDA
- `notebooks/supporting_cluster_material.ipynb` — PCA and hierarchical clustering
- `notebooks/predictions_and_cv_supporting_material.ipynb` — Testing predictions and cross-validation
- `notebooks/xgboost_supporting_material.ipynb` — Nonlinear modeling using XGBoost

---

## 📄 HTML Reports

HTML-rendered versions of all notebooks are available in the `html/` folder:

- `html/main_report.html`
- `html/eda_supporting_material.html`
- `html/supporting_cluster_material.html`
- `html/predictions_and_cv_supporting_material.html`
- `html/xgboost.html`

---

## 📚 Dataset
The dataset comes from the TidyTuesday Spotify Songs dataset:
https://github.com/rfordatascience/tidytuesday

---

## 📊 Methods and Workflow

- **Exploratory Data Analysis (EDA)**  
  Visualized distributions, transformations, and relationships between audio features and popularity.

- **Dimensionality Reduction (PCA)**  
  Reduced the high-dimensional feature set and interpreted component structure.

- **Hierarchical Clustering (Ward’s method)**  
  Identified four clusters driven mostly by continuous audio features rather than genres.

- **Linear Regression Models**  
  Compared multiple additive, interaction, and categorical modeling strategies.

- **XGBoost Regression**  
  Applied nonlinear modeling with cross-validation and feature importance evaluation.

---

## 🔎 Key Findings
- Continuous audio features drive most of the variation in popularity, such as loudness, tempo, energy, and acousticness.
- Categorical features (genre, mode, key) contributed very little to predictive power, confirmed by EDA, clustering, and XGBoost.
- PCA + Ward clustering revealed structure driven by audio features rather than genre.
- Linear models performed modestly; XGBoost improved slightly, but was still limited by noisy popularity data.

---

## 📦 Requirements
See `requirements.txt` for package versions used in the analysis.

---

## ▶️ How to Run the Project

1. **Clone the repository**
   ```
   git clone https://github.com/<your-username>/<your-repo-name>.git
   cd <your-repo-name>
   ```

2. **Install the Required Packages**
   ```
   pip install -r requirements.txt
   ```

3. **Launch Jupyter Notebook**
   ```
   jupyter notebook
   ```

4. **Open the Main Report**
    * Navigate to `notebooks/main_report.ipynb`
    * Run all cells to reproduce the whole workflow
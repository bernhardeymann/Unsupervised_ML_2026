# Semantic Structural Analysis of the Basel-Stadt Law Collection (SGBS)

**Course:** Unsupervised Machine Learning — University of Lucerne (LUMACSS), FS 2026  
**Lecturers:** Sandro Cilurzo, Arthur Habicht (Sedimentum)  
**Assessment:** Written Report (4.5 Credits)

## Project Description

This project applies unsupervised machine learning techniques to the *Systematische Gesetzessammlung Basel-Stadt (SGBS)*, sourced from the open data portal [data.bs.ch](https://data.bs.ch). The goal is to discover latent semantic structures within the legal corpus — testing whether algorithmic clustering can validate existing human-made categories and uncover new, cross-sectoral themes (e.g., digitalization) that traditional silo-structures might overlook.

## Workflow

| Step | Description | Notebook |
|------|-------------|----------|
| 1.1 | Data Sourcing — Load from data.bs.ch | `notebooks/01_1_data_sourcing.ipynb` |
| 1.2 | Cleaning — Remove legal boilerplate vocabulary | `notebooks/01_2_legal_stopwords.ipynb` |
| 1.3 | NLP — Lemmatization | `notebooks/01_3_lemmatization.ipynb` |
| 2 | Feature Engineering (Text → Vectors) | `notebooks/02_feature_engineering.ipynb` |
| 3.1 | Preprocessing — Scaling | `notebooks/03_1_scaling.ipynb` |
| 3.2 | Preprocessing — Outlier Detection | `notebooks/03_2_outlier_detection.ipynb` |
| 4.1 | Dimensionality Reduction (PCA / t-SNE) | `notebooks/04_1_dimensionality_reduction.ipynb` |
| 4.2 | Visualization — Legal Landscape Plot | `notebooks/04_2_visualization.ipynb` |
| 5.1 | Clustering — K-Means | `notebooks/05_1_kmeans.ipynb` |
| 5.2 | Clustering — DBSCAN | `notebooks/05_2_dbscan.ipynb` |
| 6 | Iteration & Improvement | `notebooks/06_iteration.ipynb` |

## Repository Structure

```
├── data/
│   ├── raw/            # Raw data from data.bs.ch (not versioned)
│   └── processed/      # Cleaned and processed data
├── notebooks/          # One notebook per workflow sub-step
├── report/
│   ├── chapters/       # LaTeX chapter files
│   ├── figures/        # Plots and visualizations
│   └── main.tex        # Main LaTeX document
├── .gitignore
└── README.md
```

## Setup

```bash
# Activate the virtual environment (Windows CMD)
uml_env\Scripts\activate.bat

# Install dependencies
pip install numpy pandas matplotlib seaborn scikit-learn notebook gensim torch torchvision
```

# Semantic Structural Analysis of the Basel-Stadt Law Collection (SGBS)

**Course:** Unsupervised Machine Learning — University of Lucerne (LUMACSS), FS 2026  
**Lecturers:** Sandro Cilurzo, Arthur Habicht (Sedimentum)  
**Assessment:** Written Report (4.5 Credits)

## Project Description

This project applies unsupervised machine learning techniques to the *Systematische Gesetzessammlung Basel-Stadt (SGBS)*, sourced from the open data portal [data.bs.ch](https://data.bs.ch). The goal is to discover latent semantic structures within the legal corpus — testing whether algorithmic clustering can validate existing human-made categories and uncover new, cross-sectoral themes (e.g., digitalization) that traditional silo-structures might overlook.

## Workflow

| Step | Description | Notebook |
|------|-------------|----------|
| 1 | Data Sourcing & Cleaning | `notebooks/01_data_sourcing.ipynb` |
| 2 | Feature Engineering (Text → Vectors) | `notebooks/02_feature_engineering.ipynb` |
| 3 | Preprocessing (Scaling & Outlier Detection) | `notebooks/03_preprocessing.ipynb` |
| 4 | Dimensionality Reduction (PCA / t-SNE) | `notebooks/04_dimensionality_reduction.ipynb` |
| 5 | Clustering Experiments (K-Means & DBSCAN) | `notebooks/05_clustering.ipynb` |
| 6 | Iteration & Improvement | `notebooks/06_iteration.ipynb` |

## Repository Structure

```
├── data/
│   ├── raw/            # Raw data from data.bs.ch (not versioned)
│   └── processed/      # Cleaned and lemmatized data
├── notebooks/          # One notebook per workflow step
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

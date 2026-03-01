# Unsupervised Clustering

This repository contains the code and final report for an exam project developed for the Unsupervised Learning course in the Master's Degree in Artificial Intelligence for Science and Technology.

## Project Overview

The goal of the project is to cluster a diabetes dataset using three target variables:

- Diabetes
- Hypertension
- Stroke

Because the dataset contains mixed-type features, the analysis uses Gower's distance to build the distance matrix used throughout the clustering workflow.

The project also explores dimensionality reduction methods, but no dimensionality reduction was applied in the final analysis because FAMD and UMAP were found to be ineffective for this dataset.

Anomaly detection was performed with the k-Nearest Neighbor algorithm, identifying approximately 2,000 outliers.

Clustering was then carried out with three different methods:

- Hierarchical clustering
- Density-based clustering (DBSCAN)
- k-Prototypes

After hyperparameter tuning, the best-performing solutions were:

- Hierarchical clustering with Ward's method
- k-Prototypes

Both of these solutions produced three clusters.

The clustering quality was evaluated with both unsupervised and supervised metrics, including:

- Silhouette coefficient
- Dunn index
- Rand score
- Adjusted Rand Index (ARI)
- Fowlkes-Mallows index

The final conclusion of the project is that none of the tested clustering solutions produced strong or clearly meaningful cluster structures on this dataset.

## Repository Contents

- `The_Diabetes_Dataset_Project_Unsupervised_CASATI_DENTI.ipynb`: Jupyter notebook containing the full analysis
- `The_Diabetes_Dataset_Project_Unsupervised_CASATI_DENTI.pdf`: final report with detailed discussion of methods and results

## Running the Notebook

The notebook is designed to download the dataset directly and then execute the analysis pipeline.

It uses Python packages such as:

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `scipy`
- `prince`
- `umap-learn`
- `gower`
- `kneed`
- `kmodes`
- `gdown`

Some of these dependencies are installed directly inside the notebook with `pip`.

## Authors

- Rebecca Casati
- Giulia Denti

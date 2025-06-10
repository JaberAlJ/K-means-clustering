# 📡 Live K Means Clustering

This repository applies the K-Means Clustering algorithm to a live streaming dataset to identify meaningful customer or user segments. It involves preprocessing, clustering, and visualizing insights from the dataset.

> Written by: [*JaberAlJ*](https://github.com/JaberAlJ)

---

## 1. 📝 Repository Overview

The aim of this repository is to implement K-Means Clustering on live-streaming-related data to discover natural groupings or clusters in the dataset. The clustering results can be useful for audience segmentation, content optimization, or marketing analysis.

---

## 2. 📦 Library Imports

The following Python libraries are used:

- `pandas` – Data manipulation
- `numpy` – Numerical computations
- `matplotlib.pyplot` and `seaborn` – Data visualization
- `sklearn.cluster.KMeans` – K-Means algorithm
- `sklearn.preprocessing.StandardScaler` – Data normalization
- `sklearn.decomposition.PCA` – Dimensionality reduction (if applied)

---

## 3. 📊 Dataset Description

The dataset contains features related to live streaming metrics such as:

- `watch time`  
- `like ratio`  
- `engagement rate`  
- `views`  
- `comments`  
- `shares`  

Each row represents a single streaming instance or session with various performance metrics.

---

## 4. 🔍 Initial Data Assessment

Initial analysis includes:

- Viewing dataset shape and column names
- Checking for null values
- Inspecting data types and distributions
- Using visualization (e.g., `pairplot`, `heatmap`) to explore relationships

---

## 5. 🧹 Data Cleaning

Cleaning steps include:

- Handling missing or zero values
- Removing duplicates if any
- Filtering outliers (if necessary)

---

## 6. 🔢 Data Encoding

Since the dataset primarily contains numeric features, encoding may not be necessary. If categorical data exists, encoding methods such as Label Encoding or One-Hot Encoding can be applied.

---

## 7. 🛠️ Data Preparation

- Selected relevant features for clustering
- Applied `StandardScaler` to normalize feature values
- (Optional) Used `PCA` for dimensionality reduction and visualization

---

## 8. 🤖 Model Selection & Evaluation

- Used `KMeans` clustering from `sklearn.cluster`
- Determined optimal number of clusters using the **Elbow Method**
- Fitted the model on scaled data
- Visualized cluster assignments using 2D scatter plots or PCA components
- Interpreted clusters based on centroid analysis

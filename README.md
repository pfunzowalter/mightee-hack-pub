# Classification of MIGHTEE Sources Using Machine Learning

## Overview

Welcome to the MIGHTEE Hackathon!

In this project, you will apply modern data science and machine learning techniques to tackle a real astrophysical classification problem using data from one of the deepest radio continuum surveys.

Radio emission from galaxies is primarily powered by two physical processes: **star formation** and **accretion onto supermassive black holes**. Distinguishing between sources dominated by these mechanisms is essential for understanding galaxy evolution and maximizing the scientific return of current and future radio surveys.

Through a series of guided Jupyter notebooks, you will build a complete machine learning workflow, from data exploration and preprocessing to dimensionality reduction, clustering, and supervised classification. Along the way, you will gain hands-on experience with astronomical datasets while developing practical machine learning skills.

By the end of this project, you will have:

* Explored and cleaned a Multi-wavelength MIGHTEE dataset.
* Applied dimensionality reduction techniques to high-dimensional data.
* Investigated both linear and non-linear feature representations.
* Built and evaluated machine learning classifiers.
* Interpreted model performance using standard diagnostic metrics and visualizations.

---

## Project Structure

The project is organized into three core notebooks:

### Notebook 1: Data Exploration

* Data inspection and quality assessment
* Handling missing values
* Exploratory data analysis (EDA)
* Feature normalization and preprocessing

### Notebook 2: Dimensionality Reduction

* Principal Component Analysis (PCA)
* Non-linear dimensionality reduction using:

  * t-SNE
  * UMAP
* Visualization of reduced feature spaces
* Comparison of linear and non-linear representations

### Notebook 3: Classification

* Binary classification using Logistic Regression
* Model evaluation and validation
* Performance comparison across different feature representations

---

## Dataset

This project uses data from the **MIGHTEE (MeerKAT International GigaHertz Tiered Extragalactic Exploration)** survey.

The dataset contains **5,224 radio sources**, each labelled as one of the following classes:

* [Star-Forming Galaxies (SFGs)](https://www.cfa.harvard.edu/news/understanding-star-forming-galaxies)
* [Active Galactic Nuclei (AGNs)](https://en.wikipedia.org/wiki/Active_galactic_nucleus)

Each source is described by a collection of astrophysical features, including:

* Multi-wavelength flux measurements
* Morphological properties
* Structural parameters
* Derived physical quantities

The goal is to determine whether machine learning techniques can successfully distinguish between AGN- and SFG-dominated sources.

---

## Repository Structure

```text
├── 1-Data_Exploration.ipynb
├── 2-Dimension_Reduction.ipynb
├── 3-Classification_Logistic_Regression.ipynb
└── data/
    ├── normalized_mightee.csv
    └── y.csv
```

Where:

* `normalized_mightee.csv` contains the preprocessed feature matrix generated in Notebook 1.
* `y.csv` contains the corresponding class labels.

---

## Hackathon Challenge

Your task is to investigate how different feature representations affect classification performance.

### Part 1: Data Exploration

1. Complete all exercises in **Notebook 1**.
2. Familiarize yourself with the dataset and preprocessing pipeline.

### Part 2: Dimensionality Reduction

Using the processed data:

1. Apply **PCA** and investigate how much variance can be retained using a reduced number of components.
2. Apply **t-SNE**, **UMAP**, or both to obtain low-dimensional representations of the data.
3. Visualize the resulting feature spaces and compare the separation between AGNs and SFGs.

### Part 3: Classification

Train and evaluate a Logistic Regression classifier using:

* The original normalized feature set
* PCA-transformed features
* t-SNE embeddings
* UMAP embeddings

Compare the performance of each representation using appropriate evaluation metrics.

### Part 4: Model Optimization

1. Identify the best-performing feature representation.
2. Perform hyperparameter optimization on the Logistic Regression model.
3. Determine whether optimization improves classification performance.

### Part 5: Advanced Investigation

Train and evaluate an alternative machine learning model, such as:

* Support Vector Machine (SVM)
* Random Forest
* Gradient Boosting
* Neural Network

Compare its performance against Logistic Regression and discuss any improvements.

---

## Report Requirements

Prepare a short report summarizing your methodology, results, and conclusions.

Your report should include:

* Description of preprocessing steps
* Dimensionality reduction results
* Classification performance comparison
* Hyperparameter optimization results
* Discussion of model strengths and weaknesses

Include the following diagnostic visualizations where appropriate:

* Confusion Matrix
* ROC Curve
* Precision–Recall Curve
* Feature-space visualizations (PCA, t-SNE, UMAP)

---

## Key Scientific Question

Can machine learning distinguish between radio sources powered by star formation and those powered by supermassive black hole activity, and which feature representation provides the most effective separation?

Good luck, and happy hacking!

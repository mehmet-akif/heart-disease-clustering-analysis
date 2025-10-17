# Heart Disease Clustering Analysis

## Overview

This project applies **unsupervised machine learning** to cluster patients based on clinical features from a **heart disease dataset**.  
Using **K-Means** and **Agglomerative Clustering**, the analysis explores patient groupings, similarities, and potential hidden patterns.

The project demonstrates the use of **scikit-learn**, **data preprocessing**, **feature scaling**, and **cluster evaluation techniques** (Elbow Method, Silhouette Score, Dendrogram).

---

## Table of Contents
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Results](#results)
- [Technologies Used](#technologies-used)
- [Usage](#usage)

---

## Dataset

- **File:** `heart-disease-dataset.csv`  
- **Description:** Contains anonymized patient data including age, blood pressure, cholesterol, resting ECG results, and target (presence/absence of heart disease).  
- **Goal:** Identify natural clusters among patients to understand health patterns beyond binary classification.

---

## Methodology

1. **Data Preprocessing**
   - Handled missing values and standardized numerical features using `StandardScaler`.
   - Removed irrelevant or constant columns to improve clustering quality.

2. **Exploratory Data Analysis (EDA)**
   - Visualized feature distributions and relationships.
   - Checked correlations between attributes.

3. **K-Means Clustering**
   - Determined optimal number of clusters via **Elbow Method** and **Silhouette Score**.
   - Assigned labels and visualized cluster separation.

4. **Agglomerative Clustering**
   - Applied hierarchical clustering for comparison.
   - Generated **Dendrogram** to visualize hierarchical relationships.

5. **Evaluation**
   - Compared both models using silhouette coefficients.
   - Interpreted cluster characteristics (e.g., age, cholesterol, blood pressure trends).

---

## Results

- Optimal number of clusters found: **3**
- **K-Means** produced distinct, compact clusters.
- **Agglomerative Clustering** revealed hierarchical grouping consistency.
- High silhouette score (~0.52) indicates good intra-cluster similarity.
- Visualization showed clear separation of clusters in principal components.

*(Visual outputs — scatter plots, dendrograms, and metrics — are displayed directly in the notebook.)*

---

## Technologies Used

- **Language:** Python 3.9+  
- **Libraries:**
  - Pandas
  - NumPy
  - Matplotlib / Seaborn
  - Scikit-learn
  - Scipy (for hierarchical clustering)
- **Tools:**
  - Jupyter Notebook  

---

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/mehmet-akif/heart-disease-clustering-analysis.git
   cd heart-disease-clustering-analysis
   ```

2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn scipy
   ```

3. Launch Jupyter Notebook:
   ```bash
   jupyter notebook Lab-5-AKIF_SIPAHI.ipynb
   ```

4. Run all cells to:
   - Perform K-Means and Agglomerative clustering.
   - Visualize dendrograms and scatter plots.
   - Compare cluster performance metrics.

---


## License

© 2025 Mehmet Akif Sipahi. All rights reserved.  
This project is shared for educational and portfolio demonstration purposes only.  
Reproduction, redistribution, or submission of this material for academic credit is strictly prohibited.

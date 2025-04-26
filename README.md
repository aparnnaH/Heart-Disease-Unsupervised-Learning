# Heart Disease Clustering using Unsupervised Learning

## Overview
This project applies unsupervised learning techniques to the UCI Heart Disease dataset to uncover hidden patient profiles. The goal is to explore potential patient subgroups based on cardiovascular risk factors such as age, blood pressure, cholesterol levels, and exercise response. 

## Problem Statement
Heart disease is one of the leading causes of death worldwide. Early detection and profiling of patients based on risk factors can help in formulating personalized treatment and prevention strategies. This project aims to uncover potential patient subgroups that could inform medical decision-making and preventive care strategies.

## Machine Learning Approach
The dataset was preprocessed, standardized, and reduced to two dimensions using PCA for visualization. Three clustering algorithms were applied to the data:

- **K-Means**: Provides a clean separation of clusters, though it requires specifying the number of clusters beforehand.
- **DBSCAN**: Performs density-based clustering, allowing it to detect clusters of varying shapes and handle noise points.
- **Agglomerative Clustering**: A hierarchical clustering method that groups patients in a tree-like structure.

### Results Summary:
- **DBSCAN** achieved the highest silhouette score after filtering noise points, making it the best-performing algorithm in terms of cluster separation.
- **K-Means** provided distinct cluster assignments, but required pre-specifying the number of clusters.
- **Agglomerative Clustering** showed reasonable but less distinct groupings, making it less reliable compared to the other two methods.

### Results & Demo
Silhouette scores were used to evaluate the clustering performance. DBSCAN provided the best natural clustering of patients. Further analysis included profiling the clusters based on cardiovascular risk factors.

**Watch the demo video here**: [YouTube Link](https://youtu.be/your_video_link)

## Running the Notebook

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/heart-disease-prediction.git
   cd heart-disease-prediction
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
4. Open the Jupyter Notebook:
   ```bash
   jupyter notebook

5. Run the notebook to see data preprocessing, model training, and evaluation.

### Dataset
The project uses the UCI Heart Disease dataset from Kaggle: [Heart Disease Dataset on Kaggle](https://www.kaggle.com/datasets/redwankarimsony/heart-disease-data?resource=download)
### Future Improvements
- Tuning DBSCAN parameters with grid search for optimal clustering.
- Trying advanced clustering techniques like Gaussian Mixture Models (GMM).
- Using domain knowledge to engineer additional risk features for clustering.

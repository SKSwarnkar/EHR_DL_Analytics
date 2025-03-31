# EHR_Analytics_with_DeepLearning

A repository that leverages machine learning and deep learning techniques to analyze MIMIC-IV EHR data, cluster patient trajectories, and extract actionable clinical insights.

## Overview
This project preprocesses and transforms raw EHR data from MIMIC-IV, constructs patient trajectories, and applies both classical clustering (using PCA and KMeans) and contrastive learning to generate robust patient embeddings. The clusters are evaluated using various metrics and visualized to derive clinical insights.

## Features
- **Data Acquisition & Preprocessing:**  
  Read raw EHR files, perform cleaning, and standardize data.
- **Feature Engineering & Data Merging:**  
  Create new features and merge datasets to build comprehensive patient trajectories.
- **Temporal Aggregation & Tensor Formation:**  
  Pivot, reindex, and reshape data into a uniform time-series tensor.
- **Modeling & Clustering:**  
  Apply PCA for dimensionality reduction, followed by KMeans clustering; implement contrastive learning for robust embedding generation.
- **Visualization:**  
  Generate PCA, silhouette, t-SNE, and average trajectory plots to evaluate and interpret clusters.
- **Optimization Techniques:**  
  Utilize feature grouping, memory management, and hyperparameter tuning to improve model performance.

## Requirements
- Python 3.8+
- pandas, numpy, scikit-learn, matplotlib, seaborn
- PyTorch
- Additional packages: tqdm, python-pptx (optional for generating presentations)

## Installation
Clone the repository and install the required dependencies:
```bash
git clone https://github.com/yourusername/EHR_Analytics_with_DeepLearning.git
cd EHR_Analytics_with_DeepLearning
pip install -r requirements.txt

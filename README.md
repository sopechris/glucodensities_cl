# 📊 Glucodensities Day Clustering Analysis

This Jupyter Notebook analyzes **daily glucose distributions** using clustering and statistical methods. It is designed for exploratory data analysis of continuous glucose monitoring (CGM) data, with a focus on **day-level glucodensity patterns** and variability.

---

## 🔍 Features

### 🧹 Data Cleaning
- Handles `NaN`, `inf`, and extreme glucose values
- Optional cap for glucose values > 400 mg/dL

### 📈 Visualization
- KDE plots of glucose values by day
- Glucodensity visualizations for each day
- Dendrograms for cluster exploration

### 📊 Clustering
- Hierarchical clustering using **2-Wasserstein distance**
- Optional 1-Wasserstein alternative
- Cluster assignment + cluster-wise visualizations

### 📊 Statistical Testing
- Kolmogorov–Smirnov (KS) test between clusters
- Daily count of values above 75th percentile
- Ranking-based daily pattern analysis (e.g., median, skewness, kurtosis)

---

## 📚 Methodology

This notebook uses the concept of **glucodensities**—day-level glucose distribution representations based on kernel density estimation (KDE). This approach captures intra-day glucose variability in a nonparametric way, preserving subtle features such as multimodality or skewness.

The concept is inspired by:

> Müller I, Borgmann S, Wagner R, et al. *Glucodensities: a new approach to visualizing and analyzing continuous glucose monitoring data*. Diabetologia. 2023.  
> [https://doi.org/10.1007/s00125-023-05990-y](https://doi.org/10.1007/s00125-023-05990-y)

## 🛠️ Requirements

- Python 3.x  
- pandas  
- numpy  
- seaborn  
- matplotlib  
- scipy  
- scikit-learn  
- python-dateutil  

📦 Install dependencies with:

```bash
pip install pandas numpy seaborn matplotlib scipy scikit-learn python-dateutil



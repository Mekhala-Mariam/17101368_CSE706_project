# 17101368_CSE706_project
Project CSE 706: An optimized, high-performance implementation of the k-Means clustering algorithm designed for fast image segmentation, feature extraction, and cross-image pixel cluster analysis. Features vectorized distance computations and accelerated convergence metrics.
# Accelerated $k$-Means Algorithm for Processing Clusters Across Images

[![Course](https://img.shields.io/badge/Course-CSE%20706-blue.svg)](https://github.com/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-brightgreen.svg)](https://www.python.org/)

This repository contains the official implementation of the M.Sc. degree project for **CSE 706**. The project focuses on optimizing and accelerating the $k$-Means clustering algorithm to efficiently process, segment, and analyze pixel and feature clusters across single and multi-image datasets.

---

## **Key Features**
* **Accelerated $k$-Means:** Implements optimized distance calculations (e.g., Triangle Inequality bounds, vectorized NumPy/PyTorch operations) to speed up standard Lloyd's algorithm convergence.
* **Multi-Image Processing:** Performs joint feature extraction and cross-image cluster consistency across batch image datasets.
* **Image Segmentation:** Supports spatial and color-space image quantization, foreground/background extraction, and feature-based cluster mapping.
* **Performance Benchmarks:** Includes evaluation metrics for execution time, convergence rate, and cluster quality (Inertia, Silhouette Score).

---

## **Project Structure**

```text
├── data/                  # Sample images and dataset scripts
├── notebooks/             # Jupyter notebooks for visual experiments and plots
├── src/
│   ├── kmeans_fast.py     # Accelerated k-Means core implementation
│   ├── image_utils.py     # Image loading, preprocessing, and reshaping utilities
│   └── evaluation.py      # Metrics (Inertia, execution time, cluster metrics)
├── main.py                # Pipeline execution script
├── requirements.txt       # Python dependencies
└── README.md              # Project documentation

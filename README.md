 # Sonar Signal Classification: Rock vs. Mine

A comprehensive Machine Learning pipeline and GUI-based diagnostic tool designed to classify sonar returns from the seafloor. This project utilizes supervised learning techniques to distinguish between metal cylinders (simulated mines) and rocks based on spectral envelopes.

---

## Executive Summary

This repository implements a data-driven classification system for underwater object detection. By leveraging the **K-Nearest Neighbors (KNN)** algorithm, the system performs binary classification on 60-feature sonar signal vectors. 

The project demonstrates a full ML lifecycle:
* **Data Ingestion:** Processing high-dimensional sonar datasets.
* **Feature Engineering:** Scaling and normalizing numerical input vectors.
* **Model Optimization:** Implementing distance-based classification.
* **Evaluation:** Analyzing performance via Accuracy Scores and Confusion Matrices.
* **Deployment:** A custom Tkinter-based GUI for real-time inference and visualization.

---

## Technical Architecture

## The Machine Learning Core
The model relies on **Statistical Inference** to identify patterns within 60 different frequency bands to determine the material composition of an object.

1.  **Preprocessing:** Feature scaling using `scikit-learn` to ensure uniform distance weighting.
2.  **Algorithm:** K-Nearest Neighbors (KNN) for non-parametric classification.
3.  **Split Strategy:** 80/20 Train-Test split for robust validation.
4.  **Inference:** Statistical similarity mapping between new inputs and the training manifold.

## Interactive GUI Capabilities
The system includes a production-ready interface for testing and analysis:
* **Randomized Sampling:** Instantly pull and classify samples from the test set.
* **Manual Feature Input:** Full control over 60 numeric features for custom signal testing.
* **Real-time Analytics:** Integrated Matplotlib/Seaborn plots for Confusion Matrix rendering.
* **Dynamic Feedback:** Color-coded UI indicators for "Mine" (Risk) vs. "Rock" (Safe) predictions.

---

## Technology Stack

* **Language:** Python 3.x
* **Data Processing:** Pandas, NumPy
* **Machine Learning:** Scikit-learn
* **Visualization:** Matplotlib, Seaborn
* **Interface:** Tkinter

---

## Performance Evaluation

The model provides a transparent look at its predictive capabilities through standard industry metrics:

| Metric | Description |
| :--- | :--- |
| **Accuracy Score** | Percentage of correctly classified sonar returns. |
| **Confusion Matrix** | Granular view of True Positives, True Negatives, False Positives, and False Negatives. |
| **Inference Latency** | Near-instantaneous prediction suitable for real-time sonar monitoring. |

---
## Installation & Usage

## 1. Clone the Repository
```bash
git clone [https://github.com/Muhammad-Israr-baig/sonar-classification.git](https://github.com/Muhammad-Israr-baig/sonar-classification.git)
cd sonar-classification


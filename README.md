# Pulsar Candidate Classification – UE23CS352A Mini Project

## Overview

This mini-project applies **Machine Learning methods** to the problem of identifying pulsar candidates from the **HTRU2 dataset**.
Pulsars are rare astrophysical objects whose detection is important in astronomy. Manual inspection of pulsar survey data is impractical due to millions of candidates, so automated ML methods are essential.

In this project, we:

* Implement **Gaussian Discriminant Analysis (GDA)** as a baseline.
* Train and tune a **Random Forest Classifier** as the main model.
* Evaluate models on **recall, accuracy, ROC, and PR curves**.
* (Optional) Explore **unsupervised methods (KMeans, SOM)** and **PCA visualization**.

---

## Repository Structure

```
Pulsar-Candidate-Classification-UE23CS352A-Mini-Project-/
│── data/
│   └── HTRU_2.csv              # Dataset (UCI ML Repository)
│
│── notebooks/
│   └── baseline_models.ipynb   # GDA + Random Forest (main notebook)
│   └── unsupervised.ipynb      # Optional: KMeans, SOM
│
│── results/
│   └── figures/                # ROC, PR, confusion matrix plots
│   └── metrics.txt             # Accuracy, recall, F1-scores
│
│── writeup/
│   └── mini_project_summary.pdf  # One-page project summary
│
│── slides/
│   └── pulsar_presentation.pptx  # Presentation slides
│
│── README.md
│── requirements.txt
│── .gitignore
```

---

## Setup & Requirements

Install dependencies:

```bash
pip install -r requirements.txt
```

Required Python libraries:

* pandas
* numpy
* scikit-learn
* matplotlib
* seaborn

---

## Running the Project

1. Open `notebooks/baseline_models.ipynb` in **Google Colab** or Jupyter.
2. Ensure `HTRU_2.csv` is present in `data/`.
3. Run all cells to:

   * Train GDA and Random Forest classifiers
   * Evaluate on test data
   * Generate metrics and plots

---

## Results (Sample)

* **Gaussian Discriminant Analysis (Baseline):**

  * Accuracy: ~96%
  * Recall: ~85%

* **Random Forest (Tuned):**

  * Accuracy: ~98%
  * Recall: ~90% (with threshold adjustment)

Plots and evaluation metrics are saved under `results/`.

---

## Team Members

* **Adishree Gupta** – Core implementation, dataset processing, Random Forest, repo setup.
* **Akash Raghavendra H V** – KMeans clustering, draft write-up, slide preparation.

---

## Timeline

* **Start Date:** Sep 29, 2025
* **Submission Deadline:** Oct 13, 2025
* **Review & Demo:** Oct 14–15, 2025

---

## References

* [HTRU2 Dataset – UCI ML Repository](https://archive.ics.uci.edu/ml/datasets/HTRU2)
* Debesai, Gutierrez, Koyluoglu (2020). *Application of machine learning methods to identify and categorize radio pulsar signal candidates.*

---

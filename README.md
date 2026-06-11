# CSB320 — Customer Segmentation with Clustering

Segment customers using K-Means and Hierarchical (Agglomerative) Clustering and evaluate cluster quality using silhouette and Davies-Bouldin scores.

---

## Datasets

| Dataset | File | Source |
|---|---|---|
| Primary | `data/credit_card.csv` | Provided by instructor |
| Secondary | `data/fraud.csv` | [Kaggle](https://www.kaggle.com) |

---

## Project Structure

```
.
├── data/
│   ├── credit_card.csv
│   └── fraud.csv
├── credit_card_analysis.ipynb
├── fraud_analysis.ipynb
├── data_dictionary.txt
├── requirements.yml
├── ai_review.md
└── README.md
```

---

## Environment Setup

This project uses Anaconda. Follow these steps to set up the environment:

**1. Clone the repository**
```bash
git clone <your-repo-url>
cd <repo-name>
```

**2. Create the Anaconda environment from `requirements.yml`**
```bash
conda env create -f requirements.yml
```

**3. Activate the environment**
```bash
conda activate clustering
```

**4. Launch Jupyter Notebook**
```bash
jupyter notebook
```

**5. Open and run both notebooks**
- `credit_card_analysis.ipynb`
- `fraud_analysis.ipynb`

Make sure all cells are executed top to bottom before reviewing results.

---

## Dependencies

All dependencies are listed in `requirements.yml`. Key packages:

| Package | Purpose |
|---|---|
| pandas | Data loading and manipulation |
| numpy | Numerical operations |
| matplotlib | Plotting and visualization |
| seaborn | Statistical visualizations |
| scikit-learn | Clustering models and evaluation metrics |
| scipy | Hierarchical clustering and dendrogram |
| jupyter | Notebook environment |

---

## Clustering Pipeline

Both notebooks follow the same pipeline:

1. **Data Loading & Cleaning** — drop identifier columns, fill nulls with column median, remove outliers via IQR
2. **Feature Scaling** — standardize all numerical features using `StandardScaler`
3. **K-Means Clustering** — use Elbow Method to find optimal k, fit model, assign labels
4. **Hierarchical Clustering** — apply Agglomerative Clustering, compare assignments to K-Means
5. **Evaluation & Visualization** — silhouette scores, Davies-Bouldin scores, scatter plots, pair plots, silhouette plot

---

## YouTube Video

[Insert unlisted YouTube link here]

---

## Academic Integrity

This repository is private. Instructor and TAs have been invited as collaborators.

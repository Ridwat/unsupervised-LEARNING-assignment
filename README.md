# Wine Clustering & Dimensionality Reduction

**Adetola Ridwat Odulaja** · Academic machine learning project

Compare two clustering methods and make high-dimensional chemical measurements easier to interpret.

**Focus:** Segmentation · Model comparison · Visual interpretation

## Question

Can wines be grouped by their chemical attributes without using their class labels?

## Dataset & method

The scikit-learn Wine dataset contains 178 samples and 13 numeric features. The notebook standardizes features, compares K-Means and agglomerative clustering across candidate cluster counts, and uses silhouette scores to assess separation. PCA and t-SNE provide two-dimensional visualizations.

## Recorded results

| Measure | Saved notebook result |
|---|---:|
| Selected clusters, K-Means | 3 |
| Selected clusters, agglomerative | 3 |
| K-Means silhouette | 0.2849 |
| Agglomerative silhouette | 0.2774 |
| Variance captured by two PCA components | 55.4% |

K-Means achieved slightly better silhouette separation in this run. The modest scores also show that cluster boundaries are not sharply separated.

## Why it matters

This is a small-scale demonstration of segmentation and model comparison. Similar methods can help explore customer or operational groupings, provided the resulting segments are validated against business needs.

## Explore the work

- [Executed notebook](Unsupervised_Clustering_Wine%20%281%29.ipynb)
- [Submitted report](Unsupervised%20learning.pdf)
- [Companion notebook version](https://github.com/Ridwat/assignment-9-ML)

## Run

Open the executed notebook in Google Colab and run sequentially. It uses NumPy, Pandas, Matplotlib, scikit-learn, and SciPy. The dataset is loaded using `load_wine()`.

## Limitations

The dataset is small. Two PCA dimensions omit some information, and visual separation alone does not establish useful segments. API deployment and monitoring are discussed as possible extensions; they are not implemented here. Metrics above come from saved outputs and were not rerun during the documentation review.

[Explore my portfolio](https://github.com/Ridwat/Ethical-AI-Analysis/blob/main/PORTFOLIO.md)

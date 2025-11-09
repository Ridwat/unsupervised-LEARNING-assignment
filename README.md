# 🧠 Unsupervised Learning on Wine Dataset (Clustering + Dimensionality Reduction)

This project demonstrates the application of **unsupervised learning techniques** — specifically **K-Means** and **Agglomerative (Hierarchical)** clustering — on the classic **Wine Dataset** from `sklearn`.  
It includes full preprocessing, model training, visualization, evaluation, and a short deployment plan.

---

## 📘 Project Overview

**Goal:**  
Use clustering and dimensionality reduction techniques to identify natural groupings in wine chemical data and visualize them in lower dimensions.

**Techniques Used:**
- **Clustering:** K-Means, Agglomerative (Ward linkage)  
- **Dimensionality Reduction:** PCA (2D), t-SNE (2D)  
- **Evaluation:** Silhouette Score, Elbow Method  
- **Visualization:** Scatter plots, dendrograms, PCA/t-SNE projections  

---

## 📊 Dataset

- **Source:** `sklearn.datasets.load_wine()`  
- **Samples:** 178  
- **Features:** 13 numeric chemical attributes of wines  
- **Target:** Ignored (unsupervised learning focus)  

**Preprocessing Steps:**
- Verified no missing values  
- Standardized numeric features using `StandardScaler`  
- No categorical variables (no encoding required)

---

## ⚙️ How to Run in Google Colab

1. Open your Google Colab account.  
2. Upload the notebook file
3. 3. If prompted for missing libraries, uncomment and run the `pip install` lines in the first code cell.
4. Run **all cells sequentially** (`Runtime → Run all`).
5. Review outputs such as:
- Elbow plot  
- Silhouette score chart  
- Dendrogram  
- PCA and t-SNE visualizations  
- Final cluster evaluations and interpretation  

---

## 📈 Results Summary

- **K-Means:** Best *k* chosen by highest Silhouette score  
- **Agglomerative Clustering:** Confirmed structure with dendrogram  
- **PCA:** Reduced dataset to 2D with explained variance ratio ~55%  
- **t-SNE:** Enhanced local cluster separability  
- **Interpretation:** Wines grouped based on alcohol, phenols, flavanoids, and color intensity.

---

## 🚀 Deployment & Monitoring (Hypothetical Scenario)

**Scenario:**  
New daily wine-chemistry data batches are clustered to support quality control and style profiling.

**Key Points:**
- Deploy saved **scaler + clustering model** via FastAPI or Flask endpoint  
- Batch or real-time inference supported  
- Monitor **Silhouette score**, **cluster distribution**, and **feature drift**  
- Automate **monthly retraining** if performance degrades  
- Use **MLflow/DVC** for versioning and reproducibility  
- Visual dashboards via **Grafana / Power BI**

---

## 🧾 Files in This Repository

| File | Description |
|------|--------------|
| `Unsupervised_Clustering_Wine.ipynb` | Google Colab notebook with complete code and visualizations |
| `Unsupervised_Wine_Report.pdf` | Two-page summary report (methods, results, and deployment plan) |
| `README.md` | Project overview and run instructions |

---

## 🧩 Tech Stack

- **Language:** Python  
- **Libraries:** NumPy, Pandas, Matplotlib, scikit-learn, SciPy  
- **Environment:** Google Colab  

---

## 📜 License

For educational use only.

---

**Author:** Adetola Odulaja_  
📅 _November 2025_


# 🏛️ Geopolitical Alignments at the United Nations (2010–2024)  
**Unsupervised clustering using UN General Assembly voting data**

![Python](https://img.shields.io/badge/Python-3.10.19-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Status](https://img.shields.io/badge/Status-Completed-success.svg)
![Model](https://img.shields.io/badge/ML-Unsupervised%20Learning-orange.svg)
![Domain](https://img.shields.io/badge/Field-Political%20Science-purple)

🌐 Available also in Spanish: [README.md](README.md)

This project analyzes **voting patterns at the UN General Assembly (2010–2024)** to identify **geopolitical blocs** and **alignment structures** among member states in the multilateral system.

Using official UN voting records, **unsupervised learning** methods were applied to uncover patterns of diplomatic similarity between countries.

---

## 🧰 Tech Stack
- **Language:** Python 3.10.19  
- **Main libraries:**  
  `pandas`, `numpy`, `scikit-learn`,  
  `matplotlib`, `seaborn`, `plotly`, `pycountry`, `pycountry-convert`, `kaleido`
- **Dataset:** *UN General Assembly Voting Data* — [Kaggle](https://www.kaggle.com/datasets/guybarash/un-resolutions)

---

## 📊 Reproducible Workflow

1️⃣ Data cleaning and numerical transformation (`Yes`=1, `Abstain`=0.5, `No`=0)  
2️⃣ Imputation of missing values and country–resolution matrix generation  
3️⃣ **Cosine Similarity** → measuring diplomatic proximity  
4️⃣ **PCA** → dimensionality reduction and 2D visualization  
5️⃣ **Hierarchical clustering (cosine distance)** → detection of geopolitical blocs  
6️⃣ Global visualizations (PCA, dendrogram, interactive map)  
7️⃣ Export of the consolidated dataset ✅

---

## 📈 Main Results

### 🔹 Model validation
The clustering model achieved a **Silhouette Score of 0.81**, indicating **clear separation** between identified geopolitical blocs.

### 🔹 Identified Blocs
| Bloc | Description |
|:----:|--------------|
| 🟣 **Bloc 1** | United States and Israel — distinctive voting behavior, consistently divergent on security and Middle East issues. |
| 🟢 **Bloc 2** | Most UN member states — broadly aligned with multilateral consensus, with moderate regional variations. |

---

## 🌍 Visualizations

### 🔹 PCA by Geographic Region  
![PCA by region](figures/pca_regiones_un_2010_2024_preview.png)  
🔗 [View interactive map](https://fernandezelias.github.io/UN_Voting_Clustering/figures/pca_regiones_un_2010_2024.html)

### 🔹 Global Geopolitical Blocs  
![UN Blocs Map](figures/mapa_bloques_un_2010_2024_preview.png)  
🔗 [View interactive map](https://fernandezelias.github.io/UN_Voting_Clustering/figures/mapa_bloques_un_2010_2024.html)

---

## 📁 Final Dataset
✔ `data/processed/un_voting_clusters_2010_2024.csv`  
Includes: country · region · PC1–PC2 · assigned bloc ✅

---

## 🚀 Next Steps
- Extend analysis to **1990–2024** to capture long-term alignment evolution.  
- Test **alternative clustering models** (DBSCAN, Affinity Propagation).  
- Enrich data with resolution metadata (topics, committees, agenda items).  
- Compare blocs with **known international alliances** (NATO, BRICS, G77, EU).

---

## ✍️ Author
**Elías Fernández**  
📧 Contact: fernandezelias86@gmail.com  
🔗 LinkedIn: www.linkedin.com/in/eliasfernandez208  

---

📌 License: **MIT**
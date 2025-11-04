# ✈️ US Aviation Network (2010)

**Author:** Ekansh Raghav  
**Course:** Networks & Complex Systems, IIT Gandhinagar  

This repository contains my analysis of the **US Airport Network (2010)** as part of my Networks course project.  
The study models airports as nodes and flight routes as weighted edges to explore connectivity, resilience, and community structure.

---

## 📁 Repository Structure
| Folder | Description |
|--------|--------------|
| **Code/** | Jupyter/Colab notebook with all analysis steps |
| **Poster/** | Final project poster summarizing results |
| **Report/** | Detailed project report (PDF) |
| **dataset/** | Raw input files (`USairport_2010.txt`, `USairport_2010_codes.txt`) |

---
## 🚀 Key Highlights
- Constructed a **weighted airport network** using U.S. Bureau of Transportation Statistics data.  
- Computed major **centrality measures** — Degree, Betweenness, Closeness, Eigenvector, and HITS.  
- Applied **Louvain community detection** to identify clusters of highly connected airports.  
- Calculated **assortativity** and **clustering coefficients** to measure structural properties.  
- Visualized **degree distributions** and **network maps** to highlight core hubs and regional sub-networks.  
- Demonstrated **scale-free characteristics**, confirming the hub-and-spoke pattern of U.S. aviation.  
- Revealed that the system is **robust to random failures** but **vulnerable to targeted attacks** on major hubs.

---
## 🧠 Methodology / End-to-End Pipeline

The overall workflow of this project follows an **end-to-end data → analysis → insight** pipeline:

graph TD;
    A[📦 Dataset (data/raw)] --> B[🧹 Data Cleaning & Preprocessing <br>(src/data_processing.py)];
    B --> C[🕸️ Network Construction <br>(src/network_analysis.py)];
    C --> D[📊 Centrality & Community Detection <br>(NetworkX + Louvain)];
    D --> E[🎨 Visualization & Insights <br>(notebooks/01-exploration.ipynb)];
    E --> F[🖼️ Exported Figures & Tables <br>(outputs/figures)];

## 🧠 Key Results
- 1,574 airports and 17,215 routes modeled
- 20 communities detected (modularity ≈ 0.2541)
- Power-law degree distribution indicates scale-free network
- Hub airports (ATL, ORD, LAX, DFW, DEN) crucial for resilience

---

## 🧩 Frameworks & Libraries
- **Python**
- **NetworkX**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Scikit-learn**
- **python-louvain**
- **Seaborn**

---

## 📬 Contact
**Ekansh Raghav**  
[LinkedIn](https://www.linkedin.com/in/ekansh-raghav-087104249) • ekansh.raghav@iitgn.ac.in

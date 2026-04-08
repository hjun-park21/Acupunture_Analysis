# Acupoint Network Analysis for Primary Dysmenorrhea

This repository contains the official code and analytical pipeline for the study on **Acupoint Network Analysis using Graph Convolutional Networks (GCN)** for primary dysmenorrhea. 

##  Repository Structure

To ensure reproducibility and logical flow, the analysis is divided into five modular Jupyter Notebooks:

* **`01_Influence_Maximization_and_Centrality.ipynb`**
  * Constructs the acupoint network, calculates topological centralities, and simulates information spread using the Independent Cascade Model (ICM).
* **`02_Louvain_Clustering.ipynb`**
  * Performs community detection on the network using the Louvain algorithm.
* **`03_GCN_Embedding_Clustering.ipynb`**
  * Extracts deep structural features using a Graph Autoencoder (GAE) with GCN layers, followed by K-Means clustering and t-SNE visualization. 
* **`04_RolX.ipynb`**
  * Extracts topological roles of acupoints using NMF-based RolX analysis.
* **`05_Temporal_Network.ipynb`**
  * Analyzes the evolutionary pattern of the acupoint network across different eras.

##  Environment Setup

All analyses were conducted in **Python 3.12**. 

```bash
pip install -r requirements.txt

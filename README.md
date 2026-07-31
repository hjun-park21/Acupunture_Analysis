# Acupoint Network Analysis for Primary Dysmenorrhea

[![DOI](https://img.shields.io/badge/DOI-10.2147%2FIJWH.S598657-blue.svg)](https://doi.org/10.2147/IJWH.S598657)
[![PubMed](https://img.shields.io/badge/PubMed-42519501-success.svg)](https://pubmed.ncbi.nlm.nih.gov/42519501)

This repository contains the official code and analytical pipeline for the study: 
**"Network-Based Identification of Core Acupoints for Primary Dysmenorrhea: A Synthesis of Randomized Trial Prescriptions"** (Published in *International Journal of Women's Health*).

* **Read the paper:** [PubMed](https://pubmed.ncbi.nlm.nih.gov/42519501) | [Publisher Site](https://doi.org/10.2147/IJWH.S598657)

## Repository Structure

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

## Environment Setup

All analyses were conducted in **Python 3.12**. 

```bash
pip install -r requirements.txt
```

## Citation

If you find this code or our paper useful in your research, please consider citing:

```bibtex
@article{lee2026network,
  title={Network-Based Identification of Core Acupoints for Primary Dysmenorrhea: A Synthesis of Randomized Trial Prescriptions},
  author={Lee, In-Seon and Park, Hyunjun and Kim, Junsuk},
  journal={International Journal of Women's Health},
  year={2026},
  publisher={Dove Medical Press},
  doi={10.2147/IJWH.S598657},
  url={https://pubmed.ncbi.nlm.nih.gov/42519501}
}
```

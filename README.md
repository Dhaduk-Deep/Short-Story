# Comparative Study of Modern Dimensionality Reduction Techniques

This repository contains my CMPE 255 (Data Mining) **short story / survey project** on modern dimensionality reduction methods, based on the 2025 survey paper:

> **A Survey: Potential Dimensionality Reduction Methods for Data Reduction**  
> Arxiv: [https://arxiv.org/abs/2502.11036](https://arxiv.org/abs/2502.11036)

The project focuses on data mining–relevant dimensionality reduction techniques such as **PCA, Kernel PCA, Sparse Kernel PCA, t-SNE, and UMAP**, and presents them in a **story-style Medium article**, a **slide deck**, and an **accompanying video presentation**.

---

## 📌 Quick Links

- 📝 **Medium Article**  
  *A Friendly Tour of Dimensionality Reduction*  
  [https://medium.com/@deepbharatbhai.dhaduk/a-friendly-tour-of-dimensionality-reduction-d1f2a98a8727?postPublishedType=initial](https://medium.com/@deepbharatbhai.dhaduk/a-friendly-tour-of-dimensionality-reduction-d1f2a98a8727?postPublishedType=initial)

- 📊 **Slideshare Presentation**  
  *Comparative Study of Modern Dimensionality Reduction Techniques*  
  [https://www.slideshare.net/slideshow/comparative-study-of-modern-dimensionality-reduction-techniques/284375883](https://www.slideshare.net/slideshow/comparative-study-of-modern-dimensionality-reduction-techniques/284375883)

- 📄 **Base Research Paper (Survey)**  
  *A Survey: Potential Dimensionality Reduction Methods for Data Reduction*  
  [https://arxiv.org/abs/2502.11036](https://arxiv.org/abs/2502.11036)

## 📚 Project Overview

High-dimensional datasets are increasingly common in modern machine learning and data mining (images, text embeddings, sensor data, logs, etc.). However, high dimensionality comes with challenges:

- High computational cost  
- Curse of dimensionality  
- Difficulty in visualization and interpretation  

This project surveys and compares several **dimensionality reduction methods** that help reduce dimensionality while preserving important structure in the data.

Methods covered:

- **PCA (Principal Component Analysis)** – Linear, fast, and widely used; great for global variance and preprocessing.  
- **Kernel PCA (KPCA)** – Uses kernel functions to capture nonlinear structure in a higher-dimensional feature space.  
- **Sparse Kernel PCA** – Approximate and more scalable version of KPCA using a subset of representative samples.  
- **t-SNE (t-Distributed Stochastic Neighbor Embedding)** – Designed for visualization; preserves local neighborhoods and reveals cluster structure in 2D.  
- **UMAP (Uniform Manifold Approximation and Projection)** – Manifold-based method that is fast, scalable, and preserves local structure with some global structure.

The emphasis is on:

- **Intuition and architecture** of each method  
- **Trade-offs**: scalability, linear vs nonlinear, local vs global structure  
- **Use cases** in data mining pipelines (visualization, preprocessing, clustering, etc.)

---

## 🧾 Repository Structure

Adjust file names as needed to match your repo.

```text
.
├── README.md                               # This file
├── Dimensionality_Reduction.pptx          # Slide deck used in the video (PowerPoint)
├── video/                                 # Folder for recorded presentation video
│   └── Dimensionality_Reduction.mp4  # 10–15 minute presentation video (optional if hosted online)
└── Research_paper.odf
   
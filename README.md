# CMPE 255 Short Story — Dimensionality Reduction for Data Mining

*A survey-style “short story” aligned with CMPE 255 (Data Mining). Focus on gist over math, with clear visuals and practical takeaways.*

**Primary source used:**  
**"A Survey: Potential Dimensionality Reduction Methods For Data Reduction."**  
*Foo Hui Mean, Yuan-chin Ivan Chang.* arXiv:2502.11036v2, 18–19 Feb 2025. (PDF in this repo’s `Research_paper.pdf`.)

---

## 🔗 Submission Links (fill these in before turning in)

- **Public GitHub repo (this repo):** <ADD URL>
- **Approved-topics spreadsheet row/link:** <ADD URL>
- **Medium article (published):** <ADD URL>
- **Slides (SlideShare, public):** <ADD URL>
- **Recording (10–15 min, public):** <ADD URL>

> Per the assignment: paste the Medium and SlideShare links into the class spreadsheet as well.

---

## 🧾 Repository Contents

| File | Description |
|------|--------------|
| `README.md` | Overview of the project and paper summary |
| `slides.pdf` | Presentation slides summarizing the research |
| `medium_article_link.txt` | Link to the Medium article |
| `video_presentation.mp4` | Recorded 10–15 minute explanation video |
| `references.txt` | Paper citation and supporting materials |

> Keep filenames exactly as above for easy grading.

---

## 🧠 Project Overview (gist over math)

This short story distills **five core dimensionality reduction methods** through a **data mining** lens—emphasizing *when to use what*, architecture-level intuition, ablation-style comparisons, and lightweight metrics:

- **PCA** — Linear, fast, interpretable; preserves **global variance**; strong first-pass for preprocessing, denoising, visualization.
- **Kernel PCA (KPCA)** — Captures **nonlinear** structure via kernels; powerful but memory/compute intensive for large *n* (Gram matrix + eigendecomposition).
- **Sparse KPCA** — Approximates KPCA using a **subset**/sparsity idea to scale better; trades exactness for efficiency.
- **t-SNE** — Excellent **local neighborhood** visualization; separates clusters well in 2D/3D; weaker global distances; sensitive to *perplexity*; higher compute.
- **UMAP** — Faster than t-SNE with a better **local/global balance**; sensitive to `n_neighbors` / `min_dist`; good default for large datasets.

### Quick comparison (rule-of-thumb)

| Method | Preserves | Typical Use | Notes |
|---|---|---|---|
| PCA | Global variance | Preprocessing; linear patterns | ~O(n d^2); very fast; interpretable components |
| KPCA | Nonlinear structure | Complex manifolds (small/med n) | ~O(n^3)/O(n^2) mem (Gram + eigendecomp) |
| Sparse KPCA | Nonlinear (approx) | Larger n than KPCA | Approximate; faster; accuracy trade-off |
| t-SNE | Local neighborhoods | 2D/3D viz & cluster separation | O(n^2) (Barnes–Hut ~O(n log n)); poor global geometry |
| UMAP | Local + some global | Large-n visualization/exploration | ~O(n log n); hyperparameter sensitive |

**Lightweight metrics to mention:** reconstruction error (PCA), trustworthiness/continuity (embedding quality), k-NN preservation, silhouette if you overlay clusters.

---

## 📰 Medium Article (what to cover)

**Suggested title:** *"Dimensionality Reduction for Data Mining: When to Use PCA, KPCA, Sparse KPCA, t-SNE, or UMAP."*

**Angle:** architecture & behavior over proofs. Include:
- PCA vs. KPCA (linear vs. kernel; inverse mapping considerations).
- Sparse KPCA’s subset/sparsity idea and trade-offs.
- t-SNE vs. UMAP: local vs. global preservation; typical pitfalls; runtime.
- Ablations: t-SNE perplexity sweeps; UMAP `n_neighbors` / `min_dist`; kernel choices for KPCA.
- Practical tips: scaling/normalization, outliers, random seeds, reproducibility.

> **Academic integrity:** Write the Medium post **from scratch** (no copying existing posts; no AI-generated text). Use your own figures or properly attributed assets.

---

## 📊 Slides (slides.pdf)

**Suggested flow (10–12 slides):**
1. Why dimensionality reduction matters for **data mining** (clustering, viz, retrieval, anomaly detection).
2. PCA in one diagram (pros/cons; when it fails).
3. KPCA intuition (kernel trick) + cost caveat.
4. Sparse KPCA (subset idea) + approximation trade-offs.
5. t-SNE visuals + pitfalls (global distortion, compute).
6. UMAP visuals + hyperparameter sensitivity.
7. Comparison table (goal, structure preserved, complexity, scalability).
8. Practical guidance (dataset size, objectives, time budget).
9. Takeaways + references.

Export to **PDF** as `slides.pdf`, upload to SlideShare, and place the public link above and in the class spreadsheet.

---

## 🎥 Recording (10–15 min)

- Present with the slides on screen and narrate *when/why* you’d pick each method.
- Show your figures/ablations; keep it practical and visual.
- Export the final recording as `video_presentation.mp4` (or link publicly if file size is large).

---

## ✅ Rubric Mapping

- **Data mining relevance:** dimensionality reduction supports clustering/viz/preprocessing at scale.
- **Recent & strong sources:** based on a 2025 survey; you may add 2024–2025 surveys or accepted ICML/NeurIPS/ICLR/KDD papers.
- **Original Medium post:** paraphrased/rewritten from scratch with your commentary and figures.
- **Slides + Recording:** clear, visual summary with public links.
- **Public GitHub + Spreadsheet:** repo is public; Medium/SlideShare links pasted in the class spreadsheet.
- **Clear README:** this file documents everything and links all artifacts.

---

## 📚 References (place full entries in `references.txt`)

Example entries you can paste into `references.txt`:

Foo Hui Mean, Yuan-chin Ivan Chang. "A Survey: Potential Dimensionality Reduction Methods For Data Reduction." arXiv:2502.11036v2, Feb 2025. 
Additional 2024–2025 survey or accepted conference papers (ICML/NeurIPS/ICLR/KDD): <Title> — <Authors>, <Venue>, <Year>. URL: <link>

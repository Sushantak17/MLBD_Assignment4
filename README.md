# CSL7110 — Assignment 4

A PySpark-based assignment covering three core data mining and graph algorithms: Clustering, Web Search (Inverted Index), and PageRank.

---

## Project Structure

```
.
├── Part1_Clustering.ipynb        # K-Center and K-Means++ clustering
├── Part2_WebSearch.ipynb         # Inverted index & search queries
├── Part3_PageRank.ipynb          # Iterative PageRank on Spark RDDs
├── M25CSA035_CSL7110_Assignment4.pdf  # Submission report
├── Q1_Clustering/                # Data folder (not included in git)
├── Q2_WebSearch/                 # Data folder (not included in git)
└── Q3_PageRank/                  # Data folder (not included in git)
```

> **Note:** The `Q1_Clustering/`, `Q2_WebSearch/`, and `Q3_PageRank/` data folders are **not tracked in this repository**. You will need to download or provide the datasets manually before running the notebooks.

---

## Parts Overview

### Part 1 — Clustering
- **Dataset:** UCI Spambase dataset (4601 points, 58 dimensions)
- **Algorithms:** Farthest First Traversal (k-center) and K-Means++
- **Goal:** Implement and compare clustering quality using the k-means objective

### Part 2 — Web Search (Inverted Index)
- **Dataset:** A collection of webpages stored in `Q2_WebSearch/webpages/`
- **Goal:** Build an inverted index over the pages and answer search queries
- Includes text normalization (lowercasing, punctuation removal, plural mapping)

### Part 3 — PageRank
- **Dataset:** `small.txt` (53 nodes) and `whole.txt` (1000 nodes, 8192 edges)
- **Goal:** Implement iterative PageRank using Spark RDDs
- **Parameters:** 40 iterations, β = 0.8, teleport probability = 0.2
- **Verification:** Top score on `small.txt` should be ~0.036

---

##  Requirements

- Python 3.x
- Apache Spark / PySpark
- NumPy

---

## Getting Started

1. Clone the repository
2. Download and place the required datasets into the respective `Q1_Clustering/`, `Q2_WebSearch/`, and `Q3_PageRank/` folders
3. Open and run the notebooks in order:
   - `Part1_Clustering.ipynb`
   - `Part2_WebSearch.ipynb`
   - `Part3_PageRank.ipynb`
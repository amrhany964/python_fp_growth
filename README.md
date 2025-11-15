# FP-Growth Algorithm Implementation

## Overview
This project implements the **FP-Growth** algorithm, one of the most efficient methods for mining **Frequent Itemsets** and **Association Rules** from large datasets.

Unlike the Apriori algorithm, which generates a huge number of candidate sets, FP-Growth uses a compressed representation of the dataset called the **FP-Tree**, allowing faster and more memory-efficient mining.

This approach is widely used in:
- Market Basket Analysis  
- Recommendation Systems  
- Pattern Recognition  

---

## How the FP-Growth Algorithm Works (Short Explanation)

### 1. Building the FP-Tree
- Count the frequency of all items.
- Remove items below the minimum support threshold.
- Sort items in each transaction by descending frequency.
- Insert each transaction into the FP-Tree while updating node counts.
- Maintain a **Header Table** linking identical items across the tree.

### 2. Mining the FP-Tree
- Start from the least frequent items.
- Build the **Conditional Pattern Base** for each item.
- Construct the **Conditional FP-Tree**.
- Recursively extract all frequent itemsets without generating candidates.

---

## Project Structure
- `DataMineTask.ipynb` — Jupyter/Colab notebook  
- `fp_growth.py` — Main FP-Growth implementation
- `dataset/` — Input datasets (Excel)

---

## Google Colab Notebook

👉 **[Open in Google Colab](https://colab.research.google.com/drive/1u1byQlP5zVVvEd3bVVmgZOPYZJCbNqCK)**

---
## 👨‍💻 Authors

**Amr Hany** <br>
**Omar Ramy** <br>
**Aya Sherif** <br>
**Jana Waleed** <br>
**Mariam Sherif** <br>
**Youssef Abd-Elhady** <br> <br>
---
Faculty of Computers and Information science – Ain Shams University

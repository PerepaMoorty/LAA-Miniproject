# Data Clustering in Social Networks Using Eigenvalues

## Overview
This project demonstrates how to identify clusters (or communities) in a social network using linear algebra concepts, particularly eigenvalues and eigenvectors.

Instead of manually analyzing connections, we represent the network as a matrix and use mathematical techniques to detect patterns and group similar nodes together.

---

## Basic Idea
In a social network:
- Some nodes (people) are more connected to each other
- These form natural groups or communities

This project uses matrix operations to automatically find those groups.

---

## How It Works

1. Represent the network as an adjacency matrix  
2. Compute the degree of each node  
3. Construct the Laplacian matrix (L = D - A)  
4. Compute eigenvalues and eigenvectors  
5. Use the second smallest eigenvector (Fiedler vector)  
6. Split nodes into clusters based on the sign of values  
7. Visualize and reorder the matrix to observe clusters clearly  

---

## What the Code Covers

- A small example graph for understanding the method  
- A real dataset (`social.mat`) for practical application  
- Clustering using eigenvectors  
- Visualization using scatter plots and matrix plots  
- Extension to multiple clusters  
- Recursive clustering of subgroups  

---

## Key Concepts Used

- Matrix representation of graphs  
- Degree matrix  
- Laplacian matrix  
- Eigenvalues and eigenvectors  
- Spectral clustering  

---

## Project Structure

```
main.ipynb       # Main implementation notebook
requirements.txt # Required Python libraries
social.mat       # Dataset used for clustering
```

---

## Requirements

Install the required libraries using:

```
pip install -r requirements.txt
```

Libraries used:
- numpy  
- scipy  
- matplotlib  
- jupyter  
- notebook  

---

## How to Run

1. Install dependencies  
2. Open the notebook:

```
jupyter notebook main.ipynb
```

3. Run all cells step by step  

---

## Output

- Clusters of nodes based on connectivity  
- Visual plots showing grouped nodes  
- Reordered adjacency matrix highlighting community structure  
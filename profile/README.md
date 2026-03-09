# LocalClustering — Local Graph Clustering Algorithms

We develop combinatorial algorithms for **local graph clustering**: given a seed node in a large graph, extract a well-characterized community around it *without processing the entire graph*.

## The Problem

Classical graph clustering partitions all nodes into groups. But in many applications — social networks, biological networks, web graphs — you only care about the community around a specific node. Local clustering solves this by exploring a small neighborhood around the seed and optimizing a quality measure called **motif conductance**, which captures how well higher-order structures (triangles) are contained within the cluster.

## Projects

| Repository | Description | Install |
|---|---|---|
| [**HeidelbergMotifClustering**](https://github.com/LocalClustering/HeidelbergMotifClustering) | Local motif clustering via graph partitioning (LMCHGP) and maximum flows (SOCIAL) | `brew install LocalClustering/motifclustering/motifclustering` |

## Quick Start

```console
brew install LocalClustering/motifclustering/motifclustering
heidelberg_motif_clustering --algorithm social --graph network.graph --seed_node 42 --output community.txt
```

## Papers

- A. Chhabra, M. Fonseca Faraj, C. Schulz. **Local Motif Clustering via (Hyper)Graph Partitioning.** ALENEX 2023. [DOI](https://doi.org/10.1137/1.9781611977561.ch9)
- A. Chhabra, M. Fonseca Faraj, C. Schulz. **Faster Local Motif Clustering via Maximum Flows.** ESA 2023. [DOI](https://doi.org/10.4230/LIPIcs.ESA.2023.34)

## Contact

Heidelberg University, Institute of Computer Science

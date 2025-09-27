# Prim's Algorithm for Minimum Spanning Tree (MST) in C

This repository contains a C implementation of **Prim's algorithm** to find the Minimum Spanning Tree (MST) of a weighted, undirected graph.

##  Description

Prim's algorithm is a greedy algorithm that finds the MST of a connected, undirected, weighted graph. It builds the tree by starting from a single vertex and incrementally adding the cheapest edge that connects a new vertex to the growing tree. This implementation uses an **adjacency matrix** to represent the graph and uses a simple array-based approach to find the minimum-weight edge.

## ⚙️ How It Works

The core logic is implemented in the `primMST` function, which leverages the following key components:

1.  **`key[]` array**: Stores the minimum edge weight required to connect a vertex to the MST.
2.  **`mstSet[]` array**: A boolean array to track vertices already included in the MST.
3.  **`minKey()` function**: A helper function that greedily selects the vertex with the minimum `key` value not yet in the MST.
4.  **Main Loop**: The algorithm iterates `V-1` times, where `V` is the number of vertices, to add each vertex to the MST. In each iteration, it finds the next vertex to add and updates the `key` values of its adjacent neighbors. 

##  How to Compile and Run

To compile the C program, use a standard C compiler like GCC.

```sh
gcc prims_algorithm.c -o prims_algorithm

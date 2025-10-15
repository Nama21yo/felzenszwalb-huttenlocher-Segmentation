https://yuminlee2.medium.com/union-find-algorithm-ffa9cd7d2dba


It is a data structure that keeps track of elements which are split into one or more disjoint sets. It has two primary operations: **find** and **union**.
- **find**: given an element it will tell you what group or set it is.
- **union**: merges two groups together.

Think of it as **magnets**.

When and where is Union Find used?
- Kruskal's minimum spanning Tree algorithm
- Grid percolation
- Network Connectivity
- Least Common ancestor in trees
- Image processing

![[Pasted image 20251014110722.png]]
* 𝜶, known as the **Inverse Ackermann function**, grows so slowly that 𝜶(All the observable particles in the universe) is approximately equal to 4.
Proof: https://codeforces.com/blog/entry/98275
- Used in Dynamic Graphs (graphs that change through time)
## Kruskal's Algorithm (Minimum Spanning Tree)
Given a (un-directed **weighted**)graph G = (V, E) we want to find a **minimum spanning tree** in the graph (it mayn't be unique). 
**Spanning tree** is a tree which we have N-nodes and N-1 edges and all nodes are reachable/connected from each other.
A **minimum spanning tree** is a subset of the edges which connect all vertices in the graph with the minimum total edge cost.
This can be solved using either **Prim's algo** or **Kruskal's algo**.
#### Algorithm Steps
1. Sort all the edges according to weight
2. - Add the smallest edge to the MST, ensuring no cycle is formed (using `union` and `find`).
3. Repeat until the MST contains `n-1` edges.
## Image Segmentation
- It is the partition of an image into a set of disjoint regions
- In order to obtain good segmentation as human perception, the determination criteria of boundary regions cannot only use local decision criteria.
### **Felzenszwalb-Huttenlocher Segmentation algorithm**

https://www.youtube.com/watch?v=iDKeR_swA8g

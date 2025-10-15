# Felzenszwalb-Huttenlocher Image Segmentation

This project implements the Felzenszwalb-Huttenlocher (FH) graph-based image segmentation algorithm, which partitions an image into perceptually uniform regions using a Union-Find data structure.

## Overview

The algorithm models an image as a graph:

- Each pixel → node
- Edges → connect neighbors
- Edge weights → color or intensity differences

Regions are merged based on internal variation and a threshold function controlled by parameter `k`.

## Parameters

- `k`: Controls segmentation scale (larger = fewer segments)
- `min_size`: Removes small regions
- `sigma`: Gaussian smoothing for noise reduction

## References

- Felzenszwalb, P.F. & Huttenlocher, D.P. (2004). _Efficient Graph-Based Image Segmentation._
  https://cs.brown.edu/people/pfelzens/papers/seg-ijcv.pdf
- Yumin Lee, _Union-Find Algorithm_
  https://yuminlee2.medium.com/union-find-algorithm-ffa9cd7d2dba
  https://github.com/Nama21yo/design_patterns_gang/blob/main/dsa_notes/union-find.ipynb
- Codeforces, _Inverse Ackermann Function_

## Description
This project implements a satellite communication network modeled as a binary tree.
Satellites are organized based on their reporting frequency using a Min-Heap strategy,
similar to Huffman tree construction.

### Requirement 
Build a binary tree from a list of satellites using a Min-Heap:
- Satellites with smaller frequencies are merged first
- The parent node stores:
  - Frequency = sum of children frequencies
  - Name = concatenation of children names
- Left child = smaller frequency (alphabetical order if equal)
- Output: level-order traversal of the final tree

Decode binary sequences:
- `0` → move left
- `1` → move right
- Output the satellite names reached by each code

Encode given satellite names into their corresponding binary paths.

Determine the Lowest Common Ancestor (LCA) of multiple satellites.

Extend the network with multi-way trees attached to the main binary tree
and compute the distance between any two nodes (main tree or multi-tree).

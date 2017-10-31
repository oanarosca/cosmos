# Breadth-first search
## Overview and example
Breadth-first search is an algorithm used for traversing a graph or tree. The search starts at the root (in case of a graph, the root is an arbitrary node) and visits all of the neighbors first befor moving to the next level neighbors. The time and space bounds are the same as for DFS, and choosing between the two depends more on the various properties and the vertex orderings, rather than on complexity. The BFS algorithm can be used in various situations, including AI, testing bipartiteness, computing the maximum flow (Ford-Fulkerson method) or finding the minimum number of edges between two nodes (an advantage over DFS).

The following example shows the order in which the nodes are visited.
```
    1
   / \
  2   3
 / \   \
4   5   6
       / \
      7   8
     /
    9
```

## Complexity
O(N+E), where N is the number of nodes and E is the number of edges. Since for each vertex all of its (not already visited) incident edges are being traversed, the complexity can be expressed as
```
V1 + incident_edges_V1 + V2 + incident_edges_V2 + ... + VN + incident_edges_VN
```
Which can be rewritten as
```
(V1 + V2 + ... + VN) + (incident_edges_V1 + incident_edges_V2 + ... + incident_edges_VN)
```
The first group's complexity is O(N). The second group's complexity is O(E).

## Further reading
[Wikipedia - Breadth-first search](https://en.wikipedia.org/wiki/Breadth-first_search)

Collaborative effort by [OpenGenus](https://github.com/opengenus)

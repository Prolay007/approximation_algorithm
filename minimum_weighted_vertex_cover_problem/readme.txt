Minimum Vertex Cover Problem - Approximation Algorithm
This project implements an approximation algorithm to solve the Minimum Vertex Cover Problem in an undirected graph. The goal is to find a set of vertices that covers all edges of the graph with minimal size.

Problem Description
In the Vertex Cover Problem, we are given an undirected graph, and the task is to find the smallest set of vertices such that each edge in the graph is connected to at least one vertex in this set. The problem is NP-hard, meaning that finding an exact solution is computationally expensive for large graphs.

This implementation uses a 2-Approximation Algorithm, which guarantees that the solution is at most twice the size of the optimal solution.

Algorithm
2-Approximation Algorithm:
Start with an empty set C (the vertex cover).
Pick any uncovered edge (u, v) from the graph.
Add both u and v to the vertex cover set C.
Remove all edges incident to either u or v from the graph.
Repeat steps 2-4 until all edges are covered.
Complexity:
Time Complexity: O(E), where E is the number of edges in the graph.
The approximation guarantee is that the size of the returned vertex cover is at most twice the size of the optimal vertex cover.
Features
Finds a near-optimal vertex cover in a given undirected graph.
Uses a greedy algorithm that runs in linear time relative to the number of edges.
Simple and efficient for practical purposes.
Requirements
Python 3.x
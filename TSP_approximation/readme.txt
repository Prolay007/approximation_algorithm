
The Traveling Salesman Problem (TSP) is a classic optimization problem where a salesman is required to visit N cities exactly once, and return to the starting city while minimizing the total distance traveled. Finding the exact solution is computationally expensive, especially for large datasets, as the problem is NP-hard.

In this implementation, we approximate the solution using the Nearest Neighbor Heuristic, which is a greedy algorithm that builds the tour by always moving to the nearest unvisited city.

Algorithm:
Nearest Neighbor Heuristic:
Start at an arbitrary city.
Find the nearest unvisited city.
Travel to that city and mark it as visited.
Repeat until all cities are visited.
Return to the starting city to complete the tour.

Complexity:
Time complexity: O(N²), where N is the number of cities.
While this is not optimal, it gives a quick approximation for the TSP and can be effective for smaller instances.

Features:
Uses Euclidean distance to calculate the distance between cities.
Generates a tour visiting all cities exactly once.
Returns the total distance of the tour and the sequence of cities visited.
Requirements
Python 3.x
## Graph Algorithms: Implementation of BFS and Dijkstra's Algorithm

## Assignment Overview

This assignment involves implementing a weighted graph and corresponding search algorithms using a vertex-centric approach rather than the traditional edge-based approach. The key distinction lies in storing adjacency information directly within the graph vertices instead of in separate edge objects.

## Key Components

### Vertex<V> Class
Represents a graph vertex with the following characteristics:
- Stores data of a generic type V
- Contains a map of adjacent vertices along with edge weights (Map<Vertex<V>, Double>)
- Provides methods for adding adjacent vertices and retrieving adjacency information
- Implements equals(), hashCode(), and toString() methods for proper vertex comparison

### WeightedGraph<V> Class
Manages the overall graph structure:
- Maintains a map of vertices for quick access by value
- Provides methods for adding vertices and edges (both directional and bidirectional)
- Includes utility methods for retrieving vertices and displaying the graph structure

### BreadthFirstSearch<V> Class
Implements the Breadth-First Search (BFS) algorithm:
- Traverses the graph starting from a specified vertex
- Returns vertices in traversal order
- Includes a method to find a path between two vertices using BFS

### DijkstraSearch<V> Class
Implements Dijkstra's algorithm for finding shortest paths:
- Computes shortest paths from a source vertex to all other vertices
- Finds the shortest path between two specified vertices
- Utilizes a priority queue for efficient selection of minimum distance vertices

### Main Class
Demonstrates the usage of all implemented classes:
- Creates example graphs with vertices and weighted edges
- Performs BFS traversal and path finding
- Executes Dijkstra's algorithm for shortest path calculations
- Displays the results of all operations

## Implementation Approach

Instead of the traditional approach using separate edge objects, this implementation follows a vertex-centric approach. Adjacency information is stored directly in the vertices, which simplifies many operations and provides a more intuitive representation of the graph. Each vertex maintains a map of its adjacent vertices along with the corresponding edge weights, allowing for efficient graph traversal and path finding.

This implementation is versatile and can work with various data types due to the use of generic types. It also provides good performance for common graph operations and demonstrates a solid understanding of BFS and Dijkstra's algorithms.

The code is organized into separate files according to Java conventions, with each public class in its own file with a matching filename. This approach follows software engineering best practices and makes the code more maintainable and readable.

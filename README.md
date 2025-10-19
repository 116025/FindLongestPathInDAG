Longest Path in a Directed Acyclic Graph (DAG)

This project provides an efficient Java implementation for finding the longest directed path from a given start vertex in a Directed Acyclic Graph (DAG).
It was developed as part of a technical assessment for Mindbank Consulting Group / U.S. Fish and Wildlife Service and demonstrates strong graph-algorithm design, scalability, and clean coding practices.


🧠 Overview
A Directed Acyclic Graph (DAG) is a structure composed of vertices and directed edges with no cycles.
This program determines the longest path length (in terms of edges) starting from a given vertex using topological sorting and dynamic programming.

⚙️ How It Works
Graph Representation:
The graph is implemented with an adjacency list, optimized for sparse and large graphs.
Topological Sort:
The vertices are ordered using a Depth-First Search (DFS)-based topological sort, ensuring all dependencies are processed before each vertex.
Longest Path Calculation:
Using dynamic programming, the algorithm iterates through the vertices in topological order, relaxing edge distances to determine the maximum distance from the start vertex to all reachable nodes.

Input Test Data
<img width="1359" height="767" alt="image" src="https://github.com/user-attachments/assets/2b017d0b-1faa-4fae-9bd2-780d03ed5728" />

Out Put For Test Data
<img width="1353" height="767" alt="image" src="https://github.com/user-attachments/assets/90853ba4-a4d6-42f6-91e1-047700b10b05" />

📈 Performance & Analysis
Category	Description
Time Complexity	O(V + E) — linear in the number of vertices and edges
Space Complexity	O(V + E) — for adjacency lists, recursion stack, and distance map
Scalability	Efficient for large DAGs (1,000+ vertices)
Graph Type	Directed, acyclic only (no cycle handling)

💡 Optimizations & Future Improvements
✅ Add memoization to cache repeated path computations
✅ Replace recursive DFS with iterative stack-based DFS for deeper graphs
✅ Enhance handling of disconnected components
✅ Extend functionality to identify multiple longest paths instead of just lengths

🧪 How to Run
Clone or download the repository.
Compile and run the program:
javac LongestPathInDAG.java
java LongestPathInDAG
The main() method contains a predefined DAG example.
Modify or add your own edges to test different scenarios.

🧍‍♂️ Author
Adonay Gebrerufael

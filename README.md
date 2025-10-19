# **Longest Path in a Directed Acyclic Graph (DAG)**

This project provides an efficient Java implementation for finding the **longest directed path** from a given start vertex in a **Directed Acyclic Graph (DAG)**.

---

## 🧠 **Overview**

A **Directed Acyclic Graph (DAG)** is a structure composed of vertices and directed edges with no cycles.  
This program determines the **longest path length (in terms of edges)** starting from a given vertex using **topological sorting** and **dynamic programming**.

---

## ⚙️ **How It Works**

### **1. Graph Representation**
The graph is implemented using an **adjacency list**, optimized for sparse and large graphs.

### **2. Topological Sort**
Vertices are ordered using a **Depth-First Search (DFS)**-based topological sort, ensuring all dependencies are processed before each vertex.

### **3. Longest Path Calculation**
Using **dynamic programming**, the algorithm iterates through the vertices in topological order, relaxing edge distances to determine the maximum distance from the start vertex to all reachable nodes.

---

## 🧪 **Input Test Data**
<img width="1360" height="768" alt="Screenshot (3)" src="https://github.com/user-attachments/assets/58507856-f69b-42fd-8a38-11e267dfe7b0" />



## 🧪 **Output Test Data**
<img width="1360" height="768" alt="Screenshot (2)" src="https://github.com/user-attachments/assets/8b27d160-a494-4903-aba5-ac0359beeaf9" />


# 🧠 Performance & Analysis

### **Category Description**

- ✅ **Time Complexity:** `O(V + E)` — linear in the number of vertices and edges  
- ✅ **Space Complexity:** `O(V + E)` — for adjacency lists, recursion stack, and distance map  
- ✅ **Scalability:** Efficient for large DAGs (1,000+ vertices)  
- ✅ **Graph Type:** Directed, acyclic only (no cycle handling)

---

# 💡 Optimizations & Future Improvements

- ✅ Add memoization to cache repeated path computations  
- ✅ Replace recursive DFS with iterative stack-based DFS for deeper graphs  
- ✅ Enhance handling of disconnected components  
- ✅ Extend functionality to identify multiple longest paths instead of just lengths  

---

# 🧩 How to Run

1. Clone or download the repository.  
2. Compile and run the program:

   ```bash
   javac LongestPathInDAG.java
   java LongestPathInDAG

🧍‍♂️ Author
Adonay Gebrerufael

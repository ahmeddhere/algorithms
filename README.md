Maximum Flow Algorithm

This project implements the Maximum Flow algorithm using the Ford-Fulkerson method (Edmonds-Karp implementation with BFS). The algorithm finds the maximum possible flow from a source node (s) to a sink node (t) in a directed graph where each edge has a capacity.

✨ Features

⚡ Ford-Fulkerson Algorithm with BFS (Edmonds-Karp).

📊 Supports graph input via adjacency matrix or adjacency list.

✅ Computes the maximum flow in a given network.

🖥 Console-based input/output.

📚 Concept

A flow network is a directed graph where each edge has a capacity.

The goal is to send as much flow as possible from source (s) to sink (t) without exceeding edge capacities.

The algorithm repeatedly finds augmenting paths using BFS until no more exist.

Each augmentation increases the total flow until the maximum is reached.

⚙️ How It Works

Build a flow network with capacities.

Start with zero flow.

While an augmenting path exists from s → t, push flow through it.

Update residual capacities.

Repeat until no path remains.



Bipartite Matching using Max Flow

This project implements Maximum Bipartite Matching using the Max Flow algorithm.A bipartite graph consists of two disjoint sets U and V. The goal is to find the maximum number of matches where each node in U is connected to exactly one node in V, without conflicts.

✨ Features

🔗 Bipartite graph matching via Max Flow reduction.

📊 Supports input via adjacency list or matrix.

✅ Finds maximum cardinality matching.

🖥 Console-based input/output.

📚 Concept

A bipartite graph is divided into two sets: U and V.

Add a super source (s) connected to all nodes in U.

Add a super sink (t) connected to all nodes in V.

Set edge capacities to 1.

Run a Max Flow algorithm.

The value of the max flow equals the maximum matching.

⚙️ How It Works

User provides a bipartite graph (edges between U and V).

Transform graph into a flow network (with super source and sink).

Apply Ford-Fulkerson (Edmonds-Karp BFS).

Extract matches from the flow.


Input

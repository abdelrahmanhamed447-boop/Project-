# Network Reachability Checker

## 📌 Overview

Python-based network reachability project simulating OSPF shortest-path calculation using Dijkstra's algorithm. The project models a router topology with weighted links and calculates the lowest-cost path between routers using a priority queue.

---

## 📑 Table of Contents

- [Project Objectives](#-project-objectives)
- [Technologies & Concepts](#-technologies--concepts)
- [Project Workflow](#-project-workflow)
  - [1. Network Topology](#1-network-topology)
  - [2. Dijkstra's Algorithm](#2-dijkstras-algorithm)
  - [3. Priority Queue](#3-priority-queue)
  - [4. OSPF Path Simulation](#4-ospf-path-simulation)
- [Configuration & Implementation](#-configuration--implementation)
- [Execution & Validation](#-execution--validation)
- [Skills Demonstrated](#-skills-demonstrated)
- [Documentation](#-documentation)
- [Project Structure](#-project-structure)
- [Project Summary](#-project-summary)

---

## 🎯 Project Objectives

- Build a Python-based network path calculation tool.
- Model a router topology using weighted links.
- Calculate the lowest-cost path between routers.
- Implement Dijkstra's shortest-path algorithm.
- Use a priority queue to process routing paths.
- Simulate OSPF shortest-path calculation.
- Analyze routing behavior and path selection.

---

## 🛠️ Technologies & Concepts

- Python
- Dijkstra's Algorithm
- `heapq`
- Priority Queue
- Graph Theory
- Weighted Graphs
- Shortest-Path Calculation
- OSPF
- Link-State Routing
- Network Path Simulation

---

# 🔄 Project Workflow

## 1. Network Topology

The project models a network topology consisting of multiple routers connected through weighted links.

Each link represents a connection between routers with an associated cost.

The topology is represented using a graph structure.

---

## 2. Dijkstra's Algorithm

Dijkstra's algorithm is used to calculate the lowest-cost path between routers.

The algorithm evaluates the available paths and continuously selects the router with the lowest known path cost.

This simulates the shortest-path calculation used in link-state routing protocols such as OSPF.

---

## 3. Priority Queue

The Python `heapq` module is used to implement a priority queue.

The priority queue allows the algorithm to process the router with the lowest current path cost first.

This improves the efficiency of the shortest-path calculation.

---

## 4. OSPF Path Simulation

The project simulates OSPF path selection by using Dijkstra's algorithm to calculate the shortest path through the network topology.

The calculated path is based on the total cost of the links between routers.

---

# ⚙️ Configuration & Implementation

The project uses Python to represent the network topology and calculate routing paths.

The implementation includes:

- Router nodes
- Weighted network links
- Graph-based topology representation
- Priority queue using `heapq`
- Dijkstra's shortest-path algorithm
- Lowest-cost path calculation

The algorithm evaluates the available routes and determines the path with the lowest total cost.
import heapq


def calculate_ospf_path(graph, start_router, end_router):
    # قاموس لتخزين أقل تكلفة للوصول لكل راوتر
    distances = {router: float('infinity') for router in graph}
    distances[start_router] = 0

    # قائمة انتظار الأولويات (Priority Queue)
    priority_queue = [(0, start_router)]

    while priority_queue:
        current_distance, current_router = heapq.heappop(priority_queue)

        # إذا وصلنا للهدف، نتوقف
        if current_router == end_router:
            return current_distance

        # البحث في الروابط المجاورة (Neighbors)
        for neighbor, cost in graph[current_router].items():
            distance = current_distance + cost

            # إذا وجدنا مساراً بتكلفة أقل، نقوم بتحديثه
            if distance < distances[neighbor]:
                distances[neighbor] = distance
                heapq.heappush(priority_queue, (distance, neighbor))

    return distances[end_router]


# تمثيل شبكة (Topology) مكونة من 4 راوترات
# الأرقام تمثل الـ Cost (مثلاً: سرعة اللينك)
network_topology = {
    'Router_A': {'Router_B': 10, 'Router_C': 2},
    'Router_B': {'Router_D': 5},
    'Router_C': {'Router_B': 3, 'Router_D': 15},
    'Router_D': {}
}

start = 'Router_A'
destination = 'Router_D'

best_cost = calculate_ospf_path(network_topology, start, destination)

print(f"--- محاكاة بروتوكول OSPF ---")
print(f"أفضل تكلفة (Cost) من {start} إلى {destination} هي: {best_cost}")

---

# 🧪 Execution & Validation

The project was validated by testing routing paths between routers in the simulated topology.

Validation included:

- Network topology processing
- Router path calculation
- Link-cost evaluation
- Lowest-cost path selection
- OSPF-style path calculation
- Verification of calculated routing paths

---

# 🧠 Skills Demonstrated

### Network Engineering

- OSPF Concepts
- Link-State Routing
- Routing Path Selection
- Network Topology Modeling
- Routing Cost Analysis

### Python

- Python Programming
- Graph Data Structures
- Dijkstra's Algorithm
- Priority Queue
- `heapq`
- Network Automation & Scripting

### Network Automation

- Network Path Simulation
- Routing Algorithm Simulation
- Automated Path Calculation
- Network Analysis

---

# 📸 Documentation

The project documentation contains evidence of the Python implementation and network path calculation logic.

The documentation demonstrates:

- Network topology
- Router connections
- Weighted links
- Dijkstra's algorithm
- Priority queue implementation
- Shortest-path calculation
- OSPF path simulation

---

# 📁 Project Structure

```text
Network-Reachability-Checker/
│
├── README.md
│
└── Network _Reachability_Checker.pdf

# Adaptive Path Planning on Dynamic Graphs

## Overview

Adaptive Path Planning on Dynamic Graphs is a simulation framework designed to study route optimization in environments where graph topology and edge costs change over time.

The project models a transportation network as a directed weighted graph and evaluates how autonomous agents adapt their navigation strategies when confronted with dynamic events such as congestion, edge failures, and directional restrictions.

The system combines shortest-path algorithms, event-driven graph updates, and real-time route replanning to emulate realistic navigation scenarios.

---

## Motivation

Most shortest-path algorithms assume a static environment. However, real-world networks such as road systems, communication networks, and robotic navigation maps continuously evolve.

This project investigates:

* Dynamic route adaptation
* Real-time shortest-path recomputation
* Event-driven graph modifications
* Multi-agent navigation behavior
* Performance of routing decisions under uncertainty

---

## Key Features

### Dynamic Graph Environment

* Directed weighted graph representation
* Configurable node and edge metadata
* Dynamic topology updates
* Temporary edge removal and restoration
* Variable edge weights

### Adaptive Route Planning

* Dijkstra's Algorithm implemented from scratch
* Multiple destination support
* Event-triggered route recomputation
* Efficient shortest-path updates

### Autonomous Agents

Agents independently navigate the graph according to their objectives.

Capabilities include:

* Goal-directed movement
* Route recalculation
* Dynamic decision making
* Environment awareness

### Event Simulation Engine

The graph evolves through temporary events:

* Traffic congestion
* Increased traversal cost
* Edge failures
* Directional restrictions

Each event has a configurable duration and automatically expires after its lifetime.

### Simulation Logging

The simulator records:

* Agent positions
* Planned routes
* Active events
* Graph modifications
* Goal completion status

This data can be used for analysis and visualization.

---

## System Architecture

Graph Engine
|
+----> Dynamic Event Manager
|
+----> Path Planning Module
|
+----> Agent Controller
|
+----> Simulation Logger

---

## Core Algorithm

### Dijkstra's Algorithm

The routing engine uses Dijkstra's shortest-path algorithm to determine optimal routes between nodes.

Features:

* Weighted graph support
* Dynamic replanning
* Multiple destination evaluation
* Event-aware route computation

---

## Project Structure

```text
.
├── graph_with_metadata.json
├── simulation.json
├── simulation_log.json
├── 23EC30067.ipynb
└── README.md
```

---

## Technologies Used

* Python
* NetworkX
* JSON
* Matplotlib
* Graph Algorithms

---

## Applications

* Autonomous Navigation Systems
* Intelligent Transportation Networks
* Robotic Path Planning
* Network Routing Simulation
* Dynamic Resource Allocation
* Multi-Agent Systems Research

---

## Future Work

* A* Search Integration
* Reinforcement Learning Based Routing
* Predictive Traffic Modeling
* Multi-Agent Coordination
* Real-Time Visualization Dashboard
* Distributed Path Planning

---

## Learning Outcomes

This project provides practical experience with graph theory, shortest-path algorithms, dynamic routing, event-driven simulation, autonomous navigation, and adaptive decision-making in evolving network environments.

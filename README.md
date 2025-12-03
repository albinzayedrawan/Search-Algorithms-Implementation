# AI Assignment 1 - Search Algorithms Implementation

This project implements and compares uninformed and informed search algorithms to solve a real-world pathfinding problem involving travel planning with constraints.

## Problem Description

The challenge involves finding optimal routes for a tourist traveling between cities (Manama to Leeds) while considering:

- Distance optimization between cities
- Entry restrictions (e.g., visa requirements for Rome)
- Multiple possible paths through various cities (Dubai, London, Venice, Rabat, Lisbon)

## Algorithms Implemented

### 1. Breadth-First Search (BFS)

- **Uninformed search algorithm**
- Guarantees shortest path in terms of number of steps/edges
- Handles barriers (restricted cities)
- Time Complexity: O(V + E)
- Space Complexity: O(V)

### 2. A* Search Algorithm

- **Informed search algorithm**
- Uses heuristic function to guide search
- Considers both actual distance traveled and estimated remaining distance
- Optimal when heuristic is admissible and consistent
- More efficient than BFS for distance-based pathfinding

## Performance Metrics

The implementation includes performance measurement tools that track:

- **Execution time** - Time taken to find the optimal path
- **Memory usage** - Space complexity in kilobytes
- **Cities visited** - Number of nodes explored during search

## Results

- **BFS**: Finds paths with fewer city visits when barriers exist, but doesn't optimize for actual distance
- **A\***: Provides superior distance-based optimization by incorporating heuristic values
- **Conclusion**: A* is the better choice for distance-based pathfinding due to its intelligent exploration strategy

## Technologies Used

- Python 3
- Google Colab
- Libraries: `queue`, `time`, `resource`, `matplotlib`

## Files

- `rawan_assignment1_cosc442.ipynb` - Main Jupyter notebook containing all implementations and analysis

## How to Run

1. Open the notebook in Google Colab or Jupyter
2. Run all cells sequentially to see:
   - Algorithm implementations
   - Performance comparisons
   - Visualization of optimal paths
   - Analysis of different heuristics

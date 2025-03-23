# ME5413_HW3

This repository contains the solutions for ME5413 Homework 3, implementing path planning algorithms (A* and Dijkstra) and solving the Travelling Shopper Problem using permutation and nearest neighbor approaches.

## Task 1: Path Planning

### A* Algorithm Results
- **Planned Paths Image:** [`planned_paths.png`](planned_paths.png)
- **Total Travel Distance:** 2815.80 meters
- **Total Cells Visited:** 53,720
- **Total Runtime:** 3.82 seconds

#### Shortest Distance Matrix (m)
|         | Start | Snacks | Store | Movie | Food |
|---------|--------|---------|--------|--------|------|
| **Start** | 0.0   | 125.2   | 131.2   | 157.8   | 197.8  |
| **Snacks**| 133.8 | 0.0     | 104.6   | 110.2   | 118.4  |
| **Store** | 132.8 | 99.6    | 0.0     | 214.0   | 104.6  |
| **Movie** | 202.8 | 97.4    | 203.4   | 0.0     | 166.8  |
| **Food**  | 197.6 | 113.2   | 105.4   | 99.2    | 0.0    |

---

### Dijkstra Algorithm Results
- **Planned Paths Image:** [`planned_paths_dijkstra.png`](planned_paths_dijkstra.png)
- **Total Travel Distance:** 2613.60 meters
- **Total Cells Visited:** 173,730
- **Total Runtime:** 10.62 seconds

#### Shortest Distance Matrix (m)
|         | Start | Snacks | Store | Movie | Food |
|---------|--------|---------|--------|--------|------|
| **Start** | 0.0   | 124.6   | 131.6   | 157.0   | 194.4  |
| **Snacks**| 124.6 | 0.0     | 99.2    | 94.4    | 113.0  |
| **Store** | 131.6 | 99.2    | 0.0     | 192.4   | 103.2  |
| **Movie** | 157.0 | 94.4    | 192.4   | 0.0     | 97.0   |
| **Food**  | 194.4 | 113.0   | 103.2   | 97.0    | 0.0    |

---

## Task 2: Travelling Shopper Problem

### Permutation Algorithm Results
- **Optimal Route Image:** [`optimal_travelling_shopper_route.png`](optimal_travelling_shopper_route.png)
- **Total Runtime:** 2.4 seconds
- **Optimal Shopping Route:** Start → Snacks → Movie → Food → Store → Start
- **Total Distance:** 550.80 meters

### Nearest Neighbor (Greedy) Algorithm Results
- **Nearest Neighbor Route Image:** [`nearest_neighbor_travelling_shopper_route.png`](nearest_neighbor_travelling_shopper_route.png)
- **Total Runtime:** 2.3 seconds
- **Nearest Neighbor Route:** Start → Snacks → Movie → Food → Store → Start
- **Total Distance:** 550.80 meters

---

## Conclusion
- **A*** achieved faster runtime but visited fewer cells compared to Dijkstra, making it more efficient for this task.
- Both the permutation and nearest neighbor approaches resulted in identical optimal shopping routes, demonstrating the efficiency of the nearest neighbor method in this scenario.

For detailed implementation and code, please refer to the provided source files.


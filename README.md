# AI Search Algorithm Implementations

A Python learning repository for exploring classical Artificial Intelligence search strategies and graph-based problem solving.

The examples use a campus-location graph to demonstrate how search algorithms explore nodes, choose paths, and differ in their use of costs and heuristics.

## Algorithms and notebooks

| Algorithm | Notebook | Search category |
| --- | --- | --- |
| Breadth-First Search (BFS) | `bfs.ipynb` | Uninformed |
| Depth-First Search (DFS) | `dfs.ipynb` | Uninformed |
| Depth-Limited Search (DLS) | `dls.ipynb` | Uninformed |
| Iterative Deepening Search (IDS) | `ids.ipynb` | Uninformed |
| Uniform-Cost Search (UCS) | `ucs.ipynb` | Uninformed, cost-based |
| Greedy Best-First Search | `greedy.ipynb` | Informed, heuristic-based |
| A* Search | `astar.ipynb` | Informed, cost and heuristic |
| Bidirectional Search | `bds.ipynb` | Uninformed, two-frontier |

The repository also includes:

- `graph.py` — shared campus graph represented as an adjacency dictionary. Each edge stores a neighboring location and a numeric cost.
- `documents.ipynb` — supporting study material.

## Technology

- Python 3
- Jupyter Notebook
- Git and GitHub

## Getting started

### 1. Clone the repository

```bash
git clone https://github.com/kura458/AI-Search-Algorithm-Implementations.git
cd AI-Search-Algorithm-Implementations
```

### 2. Create and activate a virtual environment (recommended)

On Windows:

```cmd
python -m venv .venv
.venv\Scripts\activate
```

On macOS or Linux:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Install Jupyter Notebook

```bash
python -m pip install notebook
```

### 4. Launch the notebooks

```bash
jupyter notebook
```

Open a notebook and run its cells in order. Keep `graph.py` in the repository root so notebooks that import the shared graph can find it.

## What to compare

When studying the algorithms, compare:

- **Node expansion order:** which location is explored next?
- **Path cost:** does the algorithm account for the numeric edge weights?
- **Heuristic use:** does it estimate the remaining distance to the goal?
- **Completeness and optimality:** under what assumptions can it find a solution, and is that solution guaranteed to have minimum cost?

Do not assume that every algorithm returns the same path. BFS prioritizes depth in an unweighted search, UCS prioritizes accumulated path cost, Greedy Best-First prioritizes its heuristic, and A* combines path cost with a heuristic.

## Learning objectives

- Understand graph traversal and state-space search.
- Distinguish uninformed from informed search strategies.
- Compare path selection, node expansion, and search costs.
- Practice implementing and tracing search algorithms.

## Author

[Kura Lemma](https://github.com/kura458)

---

Educational repository for Artificial Intelligence and algorithm practice.

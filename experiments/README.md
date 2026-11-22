# Project ORBIT — Experiment Index

This directory documents the experimental development of Project ORBIT.

The experiments investigate knowledge retention, transfer, adaptation, environmental change, and planning-assisted policy repair in tabular Q-learning agents.

## Experiment Groups

| Experiment Group | Focus |
|---|---|
| Experiments 011–020 | Initial Q-learning, knowledge retention, and transfer |
| Experiments 021–030 | Environmental changes, negative transfer, and recovery |
| Experiments 031–038 | Change detection, policy repair, and evaluation |
| Experiment 040C | Controlled maze complexity and adaptation |
| Experiment 041 | Repeated environmental changes and long-term adaptation |
| Experiment 042 | Robustness and generalisation across multiple maze layouts |

## Main Experimental Strategies

- **RESET:** Discards previously learned Q-values and learns again.
- **Q-LEARNING-ONLY:** Retains existing Q-values and continues learning through interaction.
- **BFS-GUIDED-REPAIR:** Uses knowledge of the maze layout and breadth-first search to guide policy repair.

## Experimental Evaluation

The experiments examine:

- Initial performance after environmental changes.
- Recovery cost and learning speed.
- Successful navigation.
- Knowledge retention and negative transfer.
- Performance across repeated environmental changes.
- Robustness across different maze layouts.

## Important Methodological Note

BFS-GUIDED-REPAIR is a model-informed planning-assisted strategy. It is not ordinary model-free Q-learning. Its results are interpreted separately from the learning-only strategies.

The experiments are computational simulations. Their findings should not automatically be generalised to physical robots or real-world environments.

See the main research report in `research/` and the technical appendix in `technical/` for detailed methodology, results, and source code.

# PROJECT ORBIT

### Investigating Knowledge Retention and Adaptation in Q-Learning Agents Under Changing Environments

**Research Area:** Artificial Intelligence and Reinforcement Learning  
**Project Type:** Computational Simulation and Experimental Investigation  
**Primary Algorithm:** Tabular Q-Learning

---

## 1. Overview

Project ORBIT investigates how reinforcement-learning agents retain and adapt previously acquired knowledge when their environments change.

The project uses gridworld simulations in which an agent learns to navigate from a starting position to a goal while avoiding obstacles.

Different adaptation strategies are compared to understand how previously acquired knowledge influences future learning.

## 2. Research Questions

- Can previously acquired knowledge improve adaptation?
- When can knowledge transfer become harmful?
- Does retaining and updating Q-values reduce relearning costs?
- Can environmental information support immediate policy repair?
- How does repeated exposure to changing environments influence adaptation?

## 3. Adaptation Strategies

| Strategy | Description |
| RETAIN   | Preserve existing learned knowledge. |
| RESET    | Discard the existing Q-table and learn again. |
| Q-LEARNING-ONLY | Retain previous knowledge and continue learning. |
| BFS-GUIDED-REPAIR | Use a search-computed route to assist policy repair. |

## 4. Experimental Development

| Experiments | Research focus |
| 001–020     | Foundational learning and knowledge transfer |
| 021–030     | Environmental changes and negative transfer |
| 031–038     | Change detection and policy repair |
| 040C        | Controlled maze complexity |
| 041         | Repeated environmental changes |
| 042         | Robustness across multiple maze layouts |

## 5. Key Findings

The final experiments produced three major observations:

1. Retaining and updating learned Q-values generally reduced recovery costs compared with resetting the Q-table.
2. BFS-guided repair achieved immediate recovery in the tested environments when complete maze information was available.
3. Retaining knowledge was not always beneficial when the environment changed.

These findings are specific to the tested gridworld simulations.

## 6. Technologies and Methods

- Python
- Tabular Q-Learning
- Epsilon-greedy exploration
- Breadth-First Search
- Gridworld simulation
- Experimental evaluation
- Statistical analysis using means and standard deviations

## 7. Research Contribution

Project ORBIT provides a controlled experimental investigation of knowledge retention, negative transfer, repeated environmental change, and planning-assisted policy repair in tabular reinforcement learning.

## 8. Repository Structure

The repository will contain:

- `research/` — Main research report.
- `technical/` — Technical appendix and methodology.
- `experiments/` — Python experiment implementations.
- `results/` — Experimental outputs.
- `figures/` — Research visualisations.

## 9. Research Scope

Project ORBIT is a computational research project. Its findings do not establish equivalent performance in robotics, autonomous vehicles, or other real-world systems.

---

**Project ORBIT — Exploring how artificial agents learn, retain, and adapt.**

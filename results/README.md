# Project ORBIT — Results Overview

## Research Findings

Project ORBIT investigates how Q-learning agents retain and adapt previously acquired knowledge when their environments change.

The experiments produced three major findings.

### 1. Knowledge Retention Can Reduce Recovery Costs

Across the repeated-environment experiments, retaining and updating learned Q-values generally required fewer recovery episodes than resetting the agent.

- Experiment 040C: Q-learning-only reduced recovery episodes compared with RESET across all four difficulty levels.
- Experiment 041: Q-learning-only reduced cumulative recovery cost by approximately 60.7% compared with RESET.
- Experiment 042: Q-learning-only reduced cumulative recovery cost by approximately 52.9% compared with RESET.

### 2. Retained Knowledge Does Not Guarantee Immediate Success

Previously learned policies can become less effective when environmental conditions change.

This demonstrates the distinction between retaining knowledge and successfully applying that knowledge in a changed environment.

### 3. Planning-Assisted Repair Can Restore Performance

BFS-GUIDED-REPAIR achieved 100% post-intervention success in the tested environments.

However, this strategy uses complete environmental information and a planning algorithm. It should therefore be distinguished from model-free Q-learning.

## Summary of Major Experiments

| Experiment | Main Investigation |
|---|---|
| 040C | Controlled maze complexity |
| 041 | Repeated environmental changes |
| 042 | Robustness across maze layouts |

## Interpretation

The findings suggest that retained knowledge can improve adaptation efficiency, while planning-assisted repair can provide immediate recovery in the tested gridworld environments.

These results are specific to the experimental conditions and do not establish universal performance guarantees.

For detailed results, methodology, and limitations, consult the main research report and technical appendix.

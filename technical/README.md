# Project ORBIT — Technical Documentation

## Overview

This directory contains the technical documentation supporting Project ORBIT.

The technical appendix describes the simulation environment, Q-learning implementation, experimental strategies, evaluation procedures, and Python source code.

## Core Components

### 1. Environment

A grid-based navigation environment in which an agent moves between a starting position and a goal while avoiding obstacles.

### 2. Learning Algorithm

The project implements tabular Q-learning using the update rule:

Q(s,a) ← Q(s,a) + α[r + γ max Q(s',a') − Q(s,a)]

### 3. Experimental Strategies

- RESET
- Q-LEARNING-ONLY
- BFS-GUIDED-REPAIR

### 4. Evaluation Metrics

- Success rate
- Successful-trip steps
- Recovery episodes
- Recovery cost
- Q-value accuracy where applicable

## Source Code

The technical appendix includes the complete Python implementations for the major experiments:

- Experiment 040C
- Experiment 041
- Experiment 042

## Reproducibility

The appendix documents the principal simulation parameters, evaluation procedures, and experimental configurations.

The results should be interpreted within the limitations of the simulated gridworld environment.

See the main research report in `research/` for the complete scientific discussion.

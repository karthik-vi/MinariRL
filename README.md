# CSE 546 RL Deep Dives: Minari Library for Offline RL

**Presenters:** Sai Karthik Varma Indukuri, Hemanth Poondla  
**Topic:** Managing and Creating Offline Reinforcement Learning Datasets using Minari

## Overview
This repository contains a guided Jupyter Notebook demonstrating the capabilities of **Minari**, the standard library for Offline Reinforcement Learning datasets maintained by the Farama Foundation. 

Unlike standard online RL, offline RL requires agents to learn policies exclusively from fixed datasets of previously recorded interactions. This notebook provides a step-by-step tutorial on how to use Minari to host, download, manipulate, and create these datasets while adhering to the standard Gymnasium API.

## Features & Walkthrough
The notebook covers the following 10 steps:
1. **Installation & Setup:** Getting started with Minari and its dependencies.
2. **CLI Exploration:** Discovering remote datasets directly from the terminal.
3. **Downloading Datasets:** Fetching standard D4RL datasets (e.g., `door-human-v2`).
4. **Dataset Inspection:** Loading local data and reviewing observation/action spaces.
5. **Episode Sampling:** Pulling batches of trajectories for offline training.
6. **Filtering:** Cleaning datasets using lambda functions (e.g., filtering by mean reward).
7. **Splitting Datasets:** Dividing data for Train/Validation/Test pipelines.
8. **Environment Recovery:** Reconstructing the original Gymnasium environment for evaluation.
9. **Combining Datasets:** Merging multiple datasets (e.g., human + expert) via the CLI.
10. **Custom Dataset Creation:** Using the `DataCollector` wrapper to record new offline datasets from live Gymnasium environments (demonstrated with `CartPole-v1`).

```bash
pip install minari[all] gymnasium

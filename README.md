# General Alpha Zero

This project is all about creating a smart game-playing computer program. It's inspired by a famous research paper from DeepMind called ["Mastering Chess and Shogi by Self-Play with a General Reinforcement Learning Algorithm"](https://arxiv.org/abs/1712.01815). The idea is to teach the program to play games by itself and get better over time.

## Overview

To make this happen, we're using a modified version of the Monte Carlo Tree Search (MCTS) algorithm. This helps the program explore different ways the game could play out and learn from them.

The key to success here is a cycle of self-play and learning. The program plays games against itself, learns from those games, and then adjusts its strategies accordingly. This loop continues, with the program improving over time until it reaches saturation.

## Key Components

- **Self-Play**: The program engages in games against itself to generate data.
- **Learning**: The program uses data from self-play to update its strategies.
- **Monte Carlo Tree Search (MCTS)**: A modified version of MCTS is used to explore potential game outcomes.

## How It Works

1. **Initialization**: The program starts with no knowledge and plays random games against itself.
2. **Self-Play**: The program plays a large number of games against itself, recording the results.
3. **Training**: The program uses the results from self-play to train its internal model.
4. **Evaluation**: The program evaluates its performance and updates its strategies.
5. **Repeat**: This cycle of self-play, training, and evaluation continues until the program reaches a satisfactory level of performance.

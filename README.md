# SC5001 Lab Assignment 1

## Overview
This repository contains the Google Colab notebook for SC5001 Lab Assignment 1.

The assignment covers two main areas:

1. Classical Search and Problem Solving
2. Applied Machine Learning with AI Copilot

## Part 1: Classical Search Algorithms

The first part explores classical search techniques namely:
- Breadth-First Search (BFS)
- A* Search
  
These are explored through classic problems:
- Graph Traversal & Admissible heuristics
- 8-Puzzle problem solving

The search algorithms were analysed using hand calculations and comparisons
of their search behaviour.

## Part 2: Machine Learning

The second part uses the California Housing dataset and Scikit-Learn to
experiment with:

- Linear Regression
- Ridge Regression
- StandardScaler
- 5-Fold Cross-Validation
- Ridge alpha tuning
- Underfitting and overfitting

### Model Results

| Model | Mean 5-Fold R² Score |
|---|---:|
| Linear Regression | 0.6457 |
| Ridge Regression (alpha = 0.1) | 0.6457 |
| Ridge Regression (alpha = 10) | 0.6443 |
| Ridge Regression (alpha = 1000) | 0.3574 |

The experiments show that moderate Ridge regularisation produces performance
similar to Linear Regression, while an extremely large alpha causes
underfitting and significantly reduces the R² score.

## Generative AI Usage

Generative AI was used as a learning and debugging assistant during the
assignment. It helped with:

- Understanding admissible heuristics
- Checking A* search calculations
- Identifying an issue with counting the blank tile in the 8-Puzzle heuristic
- Understanding feature scaling
- Explaining Ridge Regression and cross-validation
- Understanding the relationship between regularisation, underfitting and
  overfitting

## Files

- `SC5001_Lab_Assignment_1.ipynb` – Completed Google Colab notebook

## Tools Used

- Python
- Google Colab
- Scikit-Learn
- Pandas
- Matplotlib
- GitHub
- Generative AI

## Author - Khant Zay Hein

## Course - SC5001 - NTU

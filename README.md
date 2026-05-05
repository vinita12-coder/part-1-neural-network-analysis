# Part 1: Neural Network Fundamentals and Training Behavior Analysis

## Problem Statement
Build and analyze a feed-forward neural network to predict customer churn using structured data.

## Dataset
- File: customer_churn_nn.csv
- Features: 16 input columns | Target: churn (0 = retained, 1 = churned)
- Categorical features encoded using LabelEncoder
- Numerical features scaled using StandardScaler

## Steps Performed
1. Dataset Understanding — shape, types, missing values, class distribution
2. Data Preprocessing — encoding, scaling, 80/20 train-test split
3. Neural Network Model — Feed-forward NN with Dense + Dropout layers
4. Training and Evaluation — accuracy, loss curves, confusion matrix
5. Hyperparameter Experiments — 5 configurations compared

## Final Reflection
- Weights and biases: Weights control connection strength; biases shift the activation threshold
- Activation functions: Needed to introduce non-linearity; without them the network is just linear
- Learning rate too high: loss oscillates and training becomes unstable
- Learning rate too low: convergence is very slow
- Underfitting: both train and val accuracy are low
- Overfitting: train accuracy is high but val accuracy drops

## Repository Structure
part-1-neural-network-analysis/
├── README.md
├── notebook.ipynb
├── requirements.txt
└── results/
    ├── eda_plots.png
    ├── evaluation_outputs.png
    ├── model_comparison_table.png
    └── model_comparison_table.csv

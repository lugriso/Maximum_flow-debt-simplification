# Maximum Flow-based Approaches to Debt Simplification

This repository contains the implementation and datasets for a project on debt simplification using network flow models.

The project studies how to minimize the number of transactions required to settle debts within a group, modelling the problem as a flow network and leveraging maximum flow techniques.

---

## About

- Graph theory modelling
- Network flow algorithms
- Algorithmic optimization
- Data processing with Python
- Applied computational problem solving

## 📌 Project Overview

In many real-world scenarios (e.g., expense-sharing platforms such as Splitwise), a group of individuals owes money to one another. The goal is to simplify the debt structure by reducing the number of transactions required to settle all balances while preserving net positions.

This project formulates the debt simplification problem as a graph optimization problem and explores maximum flow-based solutions.

Key components:

- Representation of debts as a directed weighted graph
- Transformation into a flow network
- Application of maximum flow algorithms
- Comparison across datasets of different sizes

The full theoretical description and methodological details are provided in the accompanying report.

---

## ⚙️ Methodology

The debt structure is modelled as a directed graph:

- Nodes represent individuals.
- Directed edges represent debts.
- Edge weights represent the amount owed.

The simplification process consists of:

1. Computing net balances for each individual.
2. Constructing a flow network with:
   - A super-source connected to debtors.
   - A super-sink connected to creditors.
3. Applying a maximum flow algorithm.
4. Extracting the simplified settlement transactions from the resulting flow.

The approach ensures:

- Conservation of total debt
- Preservation of net positions
- Reduction in the number of required transactions

---

## 📊 Datasets

Three datasets are provided:

- `input-toy.csv`: small example for validation
- `input.csv`: medium-sized dataset
- `input-large.csv`: large-scale test case

They differ in graph size and density.

---

## 🚀 How to Run

1. Open the notebook:


2. Run all cells sequentially.

The notebook:
- Loads the selected dataset
- Builds the flow network
- Computes the maximum flow
- Outputs the simplified transactions

You can run it locally with Jupyter or directly in Google Colab.

---

## 📘 Report

A detailed explanation of the theoretical framework, modelling choices, and algorithmic approach is available.
---

## 📄 License

This project is for academic purposes.

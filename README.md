# Interactive Color Image Segmentation using Linear Programming (LP)

This repository contains an implementation of a **Linear Programming (LP) optimization model** for **interactive color image segmentation**, based on the original research article:

> **Interactive Color Image Segmentation with Linear Programming (LP)**  
> *Hongdong Li, Chunhua Shen* — 2008  
> DOI: https://doi.org/10.1007/s00138-008-0171-x

---

## 📌 Project Overview

Interactive image segmentation is a fundamental problem in computer vision where user-provided inputs (such as foreground/background seeds) guide the segmentation process.  
This project implements the LP-based formulation proposed by **Li & Shen (2008)**, which models color image segmentation as a global optimization problem solvable via linear programming.

The implementation focuses on:
- Modeling pixel labeling as an LP optimization problem
- Incorporating user interaction through seed constraints
- Preserving region consistency while respecting color similarity

---

## 🧠 Methodology

The segmentation task is formulated as a **Linear Programming problem**, where:
- Each pixel is assigned a label (foreground/background)
- An objective function enforces color similarity and smoothness
- Linear constraints encode user-provided seeds and labeling consistency

The optimization is solved using standard LP solvers, ensuring global optimality under the model assumptions.

---

## 🖼️ Features

- Interactive foreground/background seed selection
- LP-based global optimization for segmentation
- Color image support (RGB)
- Reproducible results aligned with the original paper
- Modular and extensible implementation

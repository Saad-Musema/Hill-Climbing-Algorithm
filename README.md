# 🧪 Hill Climbing for Root Finding of a Quadratic Function

**Name:** Saad Musema Yusuf  
**Date:** April 16, 2025  
**Task:** Use a Hill Climbing Algorithm to find the root of a quadratic function and benchmark the result using a Matplotlib plot.

---

## 🧠 Problem Overview

This project demonstrates how to apply a **Hill Climbing** algorithm to find the root of a quadratic equation:

f(x) = x² - 3x + 2


The analytical roots are **x = 1** and **x = 2**, but the aim was to approximate a root using a simple search-based optimization approach.

---

## 🔧 Approach

- Reformulated the problem as a **minimization task**: minimize `|f(x)|`.
- Used **Hill Climbing** with:
  - A small step size: `0.125`
  - A random initial starting point
  - Iterative updates to move toward the closest root
- The search continues until no better (lower `|f(x)|`) neighbor is found.

---

## 📊 Visualization

The results were visualized using `matplotlib`:
- Plotted `f(x)` from `x = -1` to `x = 4`
- Marked the **algorithm path** with red dots
- Added a **horizontal line** at `f(x) = 0` to indicate the roots

Depending on the starting point, the algorithm converged to either root (x=1 or x=2).

---

## ✅ Key Learnings

- **Hill Climbing** is effective for simple, smooth functions like quadratics.
- The result isn't always exact but gets **very close to the root** (e.g., `f(x) ≈ 0.00001`).
- **Smaller step sizes** yield better accuracy; larger ones may overshoot the minimum.
- **Visualizing** the search path helps understand the algorithm's behavior.

---

## 📌 Notes

- The algorithm **does not find all roots**, just the closest one from the start point.
- Running it multiple times with different start points can help explore different solutions.


# 📊 Blockhouse_Task

This repository contains an in-depth analysis and implementation for the Blockhouse work trial task involving limit order books, market/limit order execution, and modeling of temporary price impact functions.

---

## 🧠 Problem Overview

When executing trades—especially large market orders—**slippage** (i.e., deviation from the mid-market price) can significantly impact execution cost.  
The **temporary impact function** \\( g_t(x) \\) quantifies this cost when placing an order of size \\( x \\) at time \\( t \\).

### You are provided with:

- Per-minute **limit order book (LOB)** snapshots for 3 stocks: `CRWV`, `SOUN`, and `FROG`
- A total target of \\( S \\) shares to be bought over **390 minutes** (the trading day)

### Objectives:

- 📉 **Model** the slippage function using LOB data  
- ⚙️ **Design optimal execution strategies** to minimize the total slippage

---

## 📁 Repository Contents

| File | Description |
|------|-------------|
| `blockhouse_task.ipynb` | Demonstrates slippage modeling and compares Equal vs. Greedy execution strategies using synthetic/sample LOB data |
| `excel_slippage_analysis.ipynb` | Loads real LOB data from Excel and computes slippage for custom order sizes \\( x \\) |
| `impact_curve.png` | Sample plot of the temporary impact function \\( g_t(x) \\) |
| `README.md` | This documentation file 📘 |

---

## 🚀 How to Use

1. Clone this repository:
```bash
git clone https://github.com/yourusername/blockhouse-task.git
cd blockhouse-task

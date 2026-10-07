# 0/1 Knapsack Using Dynamic Programming

## Description

This program implements the **0/1 Knapsack problem** using Dynamic Programming. It selects projects to obtain the maximum total business value without exceeding the available development capacity.

Each project has:

* **Weight (`wt`)** – required development resources.
* **Value (`val`)** – business value of the project.
* **Capacity (`W`)** – maximum available resources.

A project can be either **selected completely or rejected**.

## Input

* Project weights: `[2, 3, 4]`
* Project values: `[40, 50, 70]`
* Maximum capacity: `5`

## Output

```text
Maximum project value: 90
```

## Approach

A 1D DP array is used to store the maximum value possible for each capacity. The capacity is processed in **reverse order** so that each project is selected at most once.

## Complexity

* **Time Complexity:** O(nW)
* **Space Complexity:** O(W)

Where:

* `n` = number of projects
* `W` = available capacity

## Result

The program finds the maximum project value as **90** without exceeding the capacity of **5 units**.

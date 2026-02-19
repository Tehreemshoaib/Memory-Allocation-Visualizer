# Memory-Allocation-Visualizer
It is a C++ project on Linux that demostrates how an Operating System allocates RAM to processes using First Fit, Best Fit and Worst Fit algorithms.The goal of the project is to demonstrate how different allocation algorithms assign processes to memory blocks and how each strategy affects memory utilization.The program takes user input for memory block sizes and process sizes, then applies each allocation algorithm separately and displays the allocation results.

# Core Concept
In operating systems, memory management is responsible for allocating available memory blocks to processes efficiently. This project compares three common allocation techniques:
First Fit – Allocates the first block that is large enough.
Best Fit – Allocates the smallest block that is sufficient.
Worst Fit – Allocates the largest available block.

## Features
Implements **First Fit**, **Best Fit**, and **Worst Fit** allocation algorithms
Number of memory blocks + sizes
Number of processes + sizes
Prints allocation tables for each algorithm:
Process number
Process size
Allocated block number or (Not Allocated)
Uses separate copies of memory blocks so each algorithm runs independently and fairly

# How It Works
# 1) First Fit
Allocates each process to the **first** memory block that is large enough.  
After allocation, the block’s remaining size is reduced.

# 2) Best Fit
Allocates each process to the **smallest** block that can still fit it.  
This aims to reduce wasted space inside blocks.

# 3) Worst Fit
Allocates each process to the **largest** available block.  
This tries to leave medium-sized blocks available for later processes.

# Technology Used
**Language:** C++ on Linux
**Type:** Console-based simulation

# How to Run
Open virtualbox
open bash
write this on terminal: g++ project.cpp -o memory_alloc
For output write: ./memory_alloc

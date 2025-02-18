# Deadlock Detection and Resource Allocation Simulator

This Python program simulates a system with N processes and M resources, where each resource has multiple instances. The program reads input files representing the allocation matrix, request matrix, and available resources, verifies their consistency, detects deadlock conditions, and provides solutions based on the system's state.

## Table of Contents
- [Project Overview](#project-overview)
- [Input Files](#input-files)
- [Functionality](#functionality)
- [How to Run](#how-to-run)
- [Technologies Used](#technologies-used)
- [License](#license)
- [Contributing](#contributing)

## Project Overview

The task involves simulating a system with N processes and M resources. Each resource can have multiple instances, and the system's state is represented by the following matrices:

- **Allocation Matrix** (N x M): Represents the currently allocated resources for each process.
- **Request Matrix** (N x M): Represents the resources each process is requesting.
- **Available Vector** (M): Represents the available resources for each resource type.

### The Program Tasks:
1. **Read the input files** and verify that the dimensions of the matrices are consistent.
2. **Detect deadlock** conditions in the system.
3. If a **deadlock is detected**, list the processes that are deadlocked.
4. If no deadlock is present, show a sequence of process executions that are possible without deadlock.

## Input Files

The program takes the following input files:

- **Allocation.csv**: Represents the NxM allocation matrix.
- **Request.csv**: Represents the NxM request matrix.
- **Available.csv**: Represents the M available vector.


## Functionality

### Deadlock Detection:
The program uses the Banker's Algorithm to determine whether there is a deadlock condition in the system. The steps include:
1. Verifying if the allocation and request matrices are valid.
2. Checking if any processes can complete based on available resources.
3. If no processes can be completed and there are processes still requesting resources, the system is considered deadlocked.

### Output:
- If a deadlock is detected, the program lists the **deadlocked processes**.
- If no deadlock is detected, the program shows a **sequence of safe executions** for the processes.

## Author 
Ali Shaikh Qasem.

# EmergingTech Notebook

## Overview
This workspace contains a single Jupyter notebook, `problems.ipynb`, that works through the Deutsch and Deutsch-Jozsa algorithm exercises using Python and Qiskit.

The notebook covers:
- generating random promised Boolean functions,
- classically classifying constant vs balanced functions,
- building Deutsch-style quantum oracles,
- running Deutsch's algorithm on single-bit functions,
- scaling the same idea to the four-bit Deutsch-Jozsa case.

## Notebook Structure

### Problem 1: Generating Random Boolean Functions
Builds a function that returns either a constant or balanced 4-input Boolean function.

### Problem 2: Classical Testing for Function Type
Implements a classical classifier that determines whether a promised function is constant or balanced.

### Problem 3: Quantum Oracles
Constructs the four possible single-input Deutsch oracles in Qiskit.

### Problem 4: Deutsch's Algorithm with Qiskit
Implements the single-query Deutsch circuit and shows how interference distinguishes constant and balanced functions.

### Problem 5: Scaling to the Deutsch-Jozsa Algorithm
Extends the approach to four input bits and demonstrates the Deutsch-Jozsa classifier on constant and balanced examples.

## Setup Guide

### 1. Install Python
Use Python 3.11 or newer. Confirm it is installed with:

```bash
python --version
```

### 2. Create a Virtual Environment
From the project folder, create and activate a virtual environment:

```bash
python -m venv .venv
.venv\Scripts\activate
```

### 3. Install Dependencies
Install the packages needed by the notebook:

```bash
pip install qiskit ipykernel
```

If you plan to run the notebook in VS Code, this is usually enough. If the kernel is missing additional packages in your environment, install them the same way.

### 4. Open the Notebook
Open `problems.ipynb` in VS Code and select the Python interpreter from your virtual environment.

### 5. Run the Cells in Order
Run the notebook from top to bottom so each problem has the definitions it depends on.

## Notes
- The notebook is written to be educational and self-contained.
- Problem 4 and Problem 5 reuse earlier oracle definitions, so the earlier cells must be executed first.
- If `qiskit` is missing from the active kernel, install it in that environment before running the quantum cells.

## Expected Outcome
When the notebook is run successfully, it should:
- generate valid promised Boolean functions,
- classify them correctly with both classical and quantum methods,
- build and display the relevant Qiskit circuits,
- demonstrate the difference between constant and balanced functions.

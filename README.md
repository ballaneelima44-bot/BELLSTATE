# Quantum Computing Assignment Part B

**Student Roll Number:** 2025BCY0004
**Repository:** BELLSTATE
**Assignment:** Quantum Computing and Post-Quantum Cryptography

## Overview

This repository contains the implementation and observations for three quantum computing and post-quantum cryptography exercises. The experiments use Python and quantum simulation tools to explore entanglement, quantum circuit design, and the mathematical principles underlying Learning With Errors (LWE).

## Tasks Implemented

### Task 1: Construction of Four Bell States

This experiment constructs the four Bell states using quantum gates:

* Phi Plus: |Φ⁺⟩
* Phi Minus: |Φ⁻⟩
* Psi Plus: |Ψ⁺⟩
* Psi Minus: |Ψ⁻⟩

Hadamard, CNOT, Pauli-X, and Pauli-Z gates are used to construct the states. Statevectors and measurement histograms are used to verify their properties.

**Key concepts:** Quantum superposition, entanglement, quantum gates, statevector analysis, and measurement outcomes.

### Task 2: Personalized Quantum Circuit Using Roll-Number Encoding

A 12-qubit quantum circuit is constructed using the binary representation derived from the student's roll number.

**Roll number:** `2025BCY0004`

The last four digits are converted to the number 4 and added to the year:

`2025 + 4 = 2029`

The resulting 12-bit binary string is:

`011111101101`

The circuit uses X gates for initialization, Hadamard gates for superposition, CNOT gates for conditional qubit correlations, and a final X gate because the last digit of the roll number is even.

The circuit is examined using its diagram, statevector, and measurement histogram.

**Key concepts:** Binary encoding, quantum circuit construction, superposition, controlled operations, and quantum measurement.

### Task 3: Learning With Errors (LWE)

This exercise demonstrates the simplified LWE-style equation:

$$
B = (A \times s + e) \bmod q
$$

The secret value is derived from the last three digits of the roll number:

`s = 004 mod 97 = 4`

The program randomly selects a public value, a small error term, and a message bit. It prints the parameters and the calculation steps.

The exercise discusses how error terms obscure the relationship between public values and a secret, and why appropriately constructed LWE problems are important in post-quantum cryptography.

**Key concepts:** Modular arithmetic, secret values, error terms, and post-quantum cryptography.

**Note:** The LWE program is an educational illustration, not a production-ready encryption system. The message bit is selected separately and does not affect the displayed LWE equation.

## Technologies Used

* Python
* Google Colab
* Qiskit
* Qiskit Aer
* NumPy
* Matplotlib

## Repository Contents

* `ASSIGNMENT2_2025BCY0004.ipynb` — Jupyter notebook containi_

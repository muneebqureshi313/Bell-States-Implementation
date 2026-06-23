# Bell-States-Implementation

## Theory
In Quantum Mechanisc, entanglement is a phenomenon where two or more particles become deeply interconnected. Once entangled, the physical state of one particle instantly dictates the state of the other.
So, Now in Quantum Computing, there are single and multi qubits system. so when 2 qubits system shows that the qubits are maximally entanglement (maximally means the probability of both quantum states are equcal), then such states are called Bell States. 
Think of qubits as quantum coins. Normal coins land on heads (0) or tails (1). Qubits can exist as both at the same time until you look at them.

Here is what happens when you measure the four Bell states:


State 1 ($\Phi^+$): Both coins always land on the same side (both heads or both tails).


State 2 ($\Phi^-$): Both coins land on the same side, but they have a hidden phase difference.


State 3 ($\Psi^+$): The coins always land on opposite sides (one heads, one tails).


State 4 ($\Psi^-$): The coins always land on opposite sides with a hidden phase difference.



$$\lvert\Phi^+\rangle = \frac{|00\rangle + |11\rangle}{\sqrt{2}}$$

$$\lvert\Phi^-\rangle = \frac{|00\rangle - |11\rangle}{\sqrt{2}}$$

$$\lvert\Psi^+\rangle = \frac{|01\rangle + |10\rangle}{\sqrt{2}}$$

$$\lvert\Psi^-\rangle = \frac{|01\rangle - |10\rangle}{\sqrt{2}}$$



## Overview

This project demonstrates the creation and simulation of a Bell State using Qiskit. Bell States are among the most fundamental examples of quantum entanglement and play a crucial role in quantum information processing, quantum communication, and quantum cryptography.

The project implements a quantum circuit that generates the Bell State:

|Φ⁺⟩ = (|00⟩ + |11⟩)/√2

and visualizes the measurement outcomes obtained from a quantum simulator.

---

## Objectives

- Understand quantum entanglement.
- Generate all Bell State using quantum gates.
- Simulate the quantum circuit using Qiskit.
- Visualize measurement results.
- Verify the presence of entanglement through measurement statistics.

---

## Bell State Circuit

The Bell State is generated using two quantum gates:

1. Hadamard Gate (H) on the first qubit
2. Controlled-NOT Gate (CNOT) between the two qubits


After applying these operations, the resulting quantum state becomes:

|Φ⁺⟩ = (|00⟩ + |11⟩)/√2

---

## Project Structure

```text
Bell-States-Implementation/
│
├── notebooks/
│   └── Bell_State.ipynb
│
├── src/
│   └── bell_state.py
│
├── figures/
│   ├── circuit.png
│   └── histogram.png
│
├── README.md
├── requirements.txt
└── LICENSE
```

## Requirements

- Python 3.10+
- Qiskit
- Matplotlib
- NumPy

## Expected Results

The measurement outcomes should show approximately equal probabilities for:

```text
00 ≈ 50%
11 ≈ 50%
```

and near-zero probability for:

```text
01 ≈ 0%
10 ≈ 0%
```

This demonstrates the entangled nature of the Bell State.

---

## Applications of Bell States

Bell States are widely used in:

- Quantum Teleportation
- Superdense Coding
- Quantum Key Distribution (QKD)
- Quantum Networks
- Quantum Error Correction
- Entanglement-Based Quantum Computing

---

## Future Work

- Perform Bell Inequality Tests
- Execute the circuit on IBM Quantum Hardware

---

## References

1. Michael A. Nielsen and Isaac L. Chuang, Quantum Computation and Quantum Information.
2. Qiskit Documentation.
3. Bell, J. S. (1964). On the Einstein-Podolsky-Rosen Paradox.

---

## Author

**Muneeb Ur Rehman**

Physics Graduate, Pakistan Institute of Engineering and Applied Sciences (PIEAS)
Developement Fellow - Physics , Quantum communications Lab

Interests:
- Quantum Computing
- Quantum Algorithms
- Quantum Machine Learning
- Quantum Cryptography



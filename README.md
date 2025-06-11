# QuantumRings_Scalable-Shor-s-Algorithm-for-Semi-Prime-Factorization

## Overview:
QuantumRing is a quantum computing project developed for MIT IQUHACK 2025, focused on implementing a scalable version of Shor’s Algorithm to factor semi-prime numbers — a task fundamental to breaking classical encryption. The project successfully demonstrated factorization of integers up to 17-bit length, integrating optimized modular arithmetic, Inverse Quantum Fourier Transform (IQFT), and quantum parallelism for high computational fidelity.


## 🧰 Tech Stack: 
Qiskit – For building and simulating quantum circuits

Python – For algorithm control, modular exponentiation, and orchestration

Shor's Algorithm – Mathematical backbone of the quantum factoring process

Modular Arithmetic + Exponentiation by Squaring – Classical optimizations for quantum pre-processing



## System Architecture 
1. Classical Preprocessing → 2. Modular Exponentiation Circuit → 3. Quantum Fourier Transform → 4. Post-Measurement Classical Analysis

Classical Preprocessing: Uses exponentiation by squaring and modulus reduction to keep computations bounded before quantum execution.

Modular Exponentiation Circuit: Constructs circuits that compute 
𝑎
𝑥
m
o
d
 
 
𝑁
a 
x
 modN with controlled operations, translated into efficient quantum gates.

Inverse QFT (IQFT): Built using Hadamard and controlled-phase gates, this module transforms periodic states into readable measurement outcomes for factor extraction.

Quantum Parallelism: Leverages superposition to evaluate all possible exponents simultaneously, with qubit-efficient control logic optimizing gate usage.

Post-Processing: Classical code analyzes measurement results to extract the period and compute the non-trivial factors of 
𝑁
N.


# Quantum Phase Estimation for H2 Hamiltonian

Educational project implementing Quantum Phase Estimation (QPE) for a small hydrogen molecule Hamiltonian.

The goal is to demonstrate how phase estimation can be used to estimate an eigenvalue of a Hamiltonian after mapping the problem to a unitary operator.

## Stack

- Python
- NumPy
- SciPy
- Matplotlib
- Qiskit

## What is implemented

- construction of a simple 2-qubit H2 Hamiltonian;
- exact diagonalization for reference eigenvalues;
- Hamiltonian shift and scaling;
- unitary operator construction via matrix exponentiation;
- QPE circuit construction;
- simulation with Qiskit Aer;
- conversion of measured phase to energy estimate;
- visualization of the measurement distribution.

## Project structure

```text
qpe-h2-qiskit/
├── README.md
├── requirements.txt
├── qpe_h2.py
└── plots/
```

## How to run

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the experiment:

```bash
python qpe_h2.py
```

The script prints the exact ground-state energy, the estimated QPE phase and the reconstructed energy.
It also saves a histogram to `plots/qpe_distribution.png`.

## Notes

This is a compact educational implementation, not a chemistry-grade VQE/QPE pipeline.
The Hamiltonian is hard-coded for clarity.

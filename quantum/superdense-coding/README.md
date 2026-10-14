# Superdense Coding Simulator

Superdense coding sends **two classical bits by transmitting a single qubit**, using an entangled pair shared in advance. The sender applies one of four operations (I, X, Z or ZX) to her half of the pair, sends it, and the receiver decodes both bits with a CNOT and a Hadamard.

This notebook works through the protocol for **all four Bell states** (|Φ⁺⟩, |Φ⁻⟩, |Ψ⁺⟩, |Ψ⁻⟩), deriving the state at every stage and checking the decoded bits across repeated runs. It also extends the idea to two EPR pairs carrying four bits.

## Files

- [`superdense_coding.ipynb`](superdense_coding.ipynb) — derivations, circuits and simulation
- [`images/`](images) — circuit diagrams used in the notebook

## Run it

```bash
pip install qiskit qiskit-aer matplotlib jupyter
jupyter notebook superdense_coding.ipynb
```

**Stack:** Python, Qiskit

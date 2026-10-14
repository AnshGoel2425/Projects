# BB84 Quantum Key Distribution

A simulation of the BB84 protocol in Qiskit, including an eavesdropper.

- **Alice** prepares qubits in randomly chosen bases; **Bob** measures in his own random bases, and the two sift a shared key from the rounds where their bases matched.
- **Eve** runs an intercept-resend attack. She has to measure before forwarding, which disturbs the states whenever she guesses the wrong basis.
- Alice and Bob compare a sample of the key to estimate the **quantum bit error rate (QBER)**. Eve's interference pushes it above the threshold, so they detect her and discard the key. Security rests on physics, not on a computational assumption.

A physical demonstration was also built with an Arduino Uno, servo-driven polarising film and lasers, so the basis choices and their consequences can be watched on a bench.

## Files

- [`BB84_Project_Report.pdf`](BB84_Project_Report.pdf) — full report: theory, implementation, results

**Stack:** Python, Qiskit, Arduino

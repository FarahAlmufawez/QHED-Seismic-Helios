# Quantum Hadamard Edge Detection (QHED) for Seismic Images

Tests whether Quantum Hadamard Edge Detection can find geological boundaries in synthetic seismic images. Built in pytket as part of PHY5004 (Quantum Computing), La Trobe University.

**Status:** results are from **noiseless simulation** (pytket with Qiskit Aer). Code for Quantinuum Helios hardware is prepared but **has not been run**.

## Results (8×8 images, 4,096 shots per scan)

| Image | Edge-location accuracy (FOM) |
|---|---|
| Seismic reflectors | 0.95 |
| Seismic with fault | 0.91 |
| Single edge | 0.85 |
| Checkerboard (stress test) | 0.00 |

Each scan uses 5 qubits (13 gates, depth 8). The method works well on layered seismic patterns but fails on very dense edges.

## References
Yao et al. (2017), *Physical Review X* 7, 031041 · Wijaya et al. (2025), *IJIGSP* 17(5)

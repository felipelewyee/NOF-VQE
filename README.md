# NOF-VQE

> [!TIP]
> [![doi](https://img.shields.io/badge/DOI-10.1021/acs.jctc.4c01734-darkgreen)](https://doi.org/10.1021/acs.jctc.4c01734)
# <img src="https://github.com/felipelewyee/NOF-VQE/blob/main/NOF-VQE.png" height=300>

This repository contains straightforward examples of the **Natural Orbital Functional Variational Quantum Eigensolver (NOF-VQE)** that requires only measurements of the 1RDM, hence, the execution on the quantum computer scales as $N^2$. The examples computes the energy of $H_2$, and can be easily extended to other systems and ansatz.

In particular, the following notebooks compute the energy of the corresponding NOF, then, they minimize with respect to $E_\text{NOF}$
- PNOF4-VQE
- PNOF3-VQE
- BBAC3-VQE
- BBC2-VQE
- GU-VQE
- HF-VQE

The performance of the algorithms on a IBM Fez with a quantum processor **IBM Heron R2** (optimization level 3 and resilience level 1, 1000 shots, run on May 4th, 2025) is the following

# <img src="https://github.com/felipelewyee/NOF-VQE/blob/main/H2-IBM-Fez-1000.png" height=300>

For this system, PNOF4 provides the most accurate results, although the resuts might depends on the system.

As a rule of thumb, PNOF4-VQE and BBAC3-VQE (and somtimes PNOF3-VQE and BBC2-VQE) provides good results.

These notebooks are partially based on: https://pennylane.ai/qml/demos/tutorial_vqe

## Authors

- Ph.D. Juan Felipe Huan Lew-Yee (felipe.lew.yee@dipc.org)
  - Donostia International Physics Center (DIPC)
- Prof. Mario Piris (mario.piris@ehu.es)
  - Donostia International Physics Center (DIPC)
  - Euskal Herriko Unibertsitatea (UPV/EHU)
  - Basque Foundation for Science (Ikerbasque)

## Acknowldgments

- J. F. H. Lew-Yee acknowledges the **Donostia International Physics Center (DIPC)** and the **Ministerio de Ciencia, Innovación y Universidades (MCIN) program Severo Ochoa** and **Agencia Estatal de Investigación (AEI)** under reference AEI/CEX2018-000867-S for post-doctoral funding (Ref.: 2023/74.)

- M. Piris acknowledges **MCIN** and **AEI** funding from MCIN/AEI/10.13039/501100011033 (Ref.: PID2021-126714 NB-I00) and the **Eusko Jaurlaritza** (Ref.: IT1584-22).

- The authors acknowledge the technical and human support provided by the **DIPC Supercomputing Center**.

- This work has been possible thanks to the quantum resources and ecosystem provided through the **IBM-BasQ** alliance for the development of quantum technologies.

---
layout: post
title: "The Idea of the VQE"
date: 2020-05-01
image: /images/VQE.png
categories: Emory, Phys 380 Quantum Computing
author: "Taikan Nakada"
authors:
venue:
arxiv:
slides:
code: https://github.com/tnakada/physics/blob/master/VariationalQuantumEigensolver.ipynb
---

For quantum systems, the problem complexity increases exponentially as the Hilbert space grows, and analytical methods in solving Schrodinger's equation become intractable quickly. This fundamental challenge has been shown to be solvable using the quantum phase estimation algorithm but is merely a theoretical method until the development of the hardware catches up. The alternative solution proposed by Alberto Peruzzo, the Variational Quantum Eigensolver, is able to estimate the ground state energy of a molecule with the current quantum hardware and shallow quantum circuits by exploiting the variational principle.
Essentially, the Hamiltonian of a system is described by the Hermitian matrix and the ground state energy of that system is the smallest eigenvalue associated with the Hamiltonian. So an arbitrary ansatz wave function is selected as an initial guess approximating the smallest eigenvalue. Calculating its expectation value and iteratively updating the wave function creates an upper bound, and thus the ground state energy of a Hamiltonian can be obtained.

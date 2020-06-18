---
layout: post
title: "The Idea of the VQE"
date: 2020-05-01
---

The advent of quantum hardware brings the potential to efficiently tackle computational problems that are unfeasible on a classical computer. Notably, for quantum systems, the problem complexity increases exponentially as the Hilbert space grows, and analytical methods in solving Schrodinger's equation become intractable quickly. This fundamental challenge has been shown to be solvable using the quantum phase estimation algorithm. However, as quantum algorithms are being developed, they remain merely theoretical methods until the development of the hardware catches up. But even as companies like Google, IBM, Rigetti, and many other leading quantum researchers build up to a more coherent quantum infrastucture, solving the minimum eigenvalues of matrices is still a far reach with the QPE.

An alternative solution was proposed by Alberto Peruzzo, at the Centre for Quantum Photonics, and his collaborators. The proposed Variational Quantum Eigensolver is able to estimate the ground state energy of a molecule with the current quantum hardware and shallow quantum circuits.

The VQS exploits the variational principle: it's the basis for variational methods in quantum mechanics. It gives approximations of the ground state, and some excited states. The method involves choosing a "trial wavefunction", or an ansatz solution, depending on one or more parameters. Finding these parameter values for which the expectation value of the energy is the lowest possible is the objective. The wavefunction obtained by fixing the parameters is approximated to the ground state wavefunction, where the closeness can be characterized by, say, a Manhattan norm. The expectation value of the energy of the obtained statevector is an upper bound to the ground state energy.

For the case of VQS, the Hamiltonian of a system is described by the Hermitian matrix and the ground state energy of that system is the smallest eigenvalue associated with the Hamiltonian. So an arbitrary ansatz wave function is selected as an initial guess approximating the smallest eigenvalue. Calculating its expectation value and iteratively updating the wave function creates an upper bound, and thus the ground state energy of a Hamiltonian can be obtained.

By using a variational algorithm, the approach reduces the requirement for coherent evolution of the quantum state, making more efficient and practical use of quantum resources available today to solve the eigenvalue problem.

More about this [here.](https://github.com/tnakada/physics/blob/master/VariationalQuantumEigensolver.ipynb)

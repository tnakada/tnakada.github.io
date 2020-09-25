---
layout: post
title: "Testing Quantum/Classical Hybrid Neural Networks"
date: 2020-04-20
image: /images/qiskit.png
categories: "Emory, Phys 380 Quantum Computing"
author: "Taikan Nakada"
authors:
venue:
arxiv:
slides:
code:
---

[This paper](https://arxiv.org/abs/1911.02998) explored the possibility of leveraging quantum algorithms on quantum hardware to augment neural networks. The idea I was trying to explore is to have a parametric quantum circuit using Qiskit in the convolutional layer of a CNN implemented in PyTorch. The quantum circuit seems advantageous in the feature mapping since it's able to explore an exponentially large space for localized patterns.

---
layout: post
date:   2019-01-29 17:32:00 -0600
title: "Neural Ordinary Differential Equations"
subtitle: "Do they have anything to say?"
categories: physics simulation
comments: true
---

Neural Ordinary Differential Equations
======================================

Neural networks have been around for a long time. But the era of neural
network computing has only recently become a big deal as a result of
hardware which can perform the training process fast enough to be useful
in real problems. The general structure of a deep architecture (and RBMs,
restricted Boltzmann machines) is a sequence of layers consisting of nodes
or neurons which individually connect to every node in both adjacent layers
and to no other nodes in their own layers or any other non-adjacent layer.
If we were to write down a mathematical structure of such a thing, it would
look like the following.

$$
x^{k+1}_i = W^k_{ij} x^k_j + b_j
$$

This is the ordinary form of a single layer of neural network in the context
of deep learning. But there's a more interesting generalization of the neural
network layer which might just make things work more efficiently in the future.
This is the neural ordinary differential equation, or NODE {% cite Chen2018 --file refs %}

References
==========

{% bibliography --file refs --cited %}



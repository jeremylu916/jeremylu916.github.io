---
title: "MoPINNEnKF / iPINNER: Iterative Physics-Informed Neural Network with Ensemble Kalman Filter"
collection: publications
category: ai4s
permalink: /publication/2025-ipinner
excerpt: 'An iterative PINN–EnKF framework that couples physics-informed networks with ensemble Kalman filtering for robust parameter and state estimation under uncertainty.'
date: 2025-08-01
venue: 'Journal of Computational Physics'
paperurl: 'https://arxiv.org/abs/2506.00731'
citation: 'Lu, B., Mou, C., &amp; Lin, G. (2025). &quot;iPINNER: An iterative physics-informed neural network with ensemble Kalman filter.&quot; <i>Journal of Computational Physics</i>, 114592.'
---

**iPINNER** (a.k.a. MoPINNEnKF) embeds a physics-informed neural network inside an ensemble Kalman filter, alternating between PINN-based forward solves and EnKF-based Bayesian updates. The iterative loop yields calibrated uncertainty estimates and robust parameter recovery for noisy, partially-observed PDE systems where pure PINN training is ill-conditioned.

---
permalink: /
title: "Hi, I'm Binghang Lu 👋"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

I am a graduate researcher in the [School of Electrical and Computer Engineering](https://engineering.purdue.edu/ECE) at **Purdue University**, advised in close collaboration with the Department of Mathematics. My work sits at the intersection of **large language models**, **continual learning**, and **AI for Science (AI4S)** — building optimization and learning algorithms that let modern models keep learning new tasks, respect physical laws, and stay reliable under distribution shift.

I work on questions like: *how do we update an LLM with new knowledge without erasing what it already knows?* *How do we train neural surrogates that obey conservation laws and PDEs at scale?* *What optimizers make both of these problems tractable?*

---

## 🔬 Research Thrusts

### Large Language Models
I design **optimizer- and geometry-aware** methods for adapting large pretrained models. Recent work introduces *Muon-OGD*, a spectral orthogonal-gradient-projection variant of the Muon optimizer for continual learning of LLMs, and contributes to safety research on large reasoning models (*Chain of Risk*, adaptive multi-principle steering).

### Continual Learning (for LLMs)
I am interested in **forgetting-free adaptation** of large language models — methods that let a pretrained LLM absorb a stream of new tasks or domains while preserving prior capabilities. My approach combines spectral / orthogonal gradient projection with the matrix-aware preconditioning of modern LLM optimizers (e.g., Muon), aimed at sharper plasticity–stability trade-offs in the post-training regime.

### AI for Science (AI4S)
On the scientific machine learning side, I develop **physics-informed and operator-learning** frameworks for PDEs, including fractional and high-dimensional regimes. Representative work: *fPINN-DeepONet* (JCP 2025) for multi-term time-fractional diffusion–wave equations; *iPINNER* (JCP 2025) iterative inference via ensemble Kalman filtering; *AdamFLIP* for hard-constrained PINN training; *Muon with Spectral Guidance* for stiff scientific-ML objectives; *Morphy-Net* / *NSGA-PINN* multi-objective and evolutionary training; and *Neural-POD* for nonlinear functional model reduction.

---

## 📰 News

- **[May/2026]** New preprint: *Muon-OGD — Muon-based Spectral Orthogonal Gradient Projection for LLM Continual Learning* on arXiv.
- **[May/2026]** *Morphy-Net* accepted by *Computer Methods in Applied Mechanics and Engineering* (CMAME).
- **[May/2026]** New preprint: *AdamFLIP — Adaptive Momentum Feedback Linearization for Hard-Constrained PINN Training* on arXiv.
- **[Apr/2026]** New preprint: *Chain of Risk — Safety Failures in Large Reasoning Models* on arXiv.
- **[Feb/2026]** Two preprints released: *Muon with Spectral Guidance* and *Neural-POD*.
- **[Sep/2025]** Awarded IMSI (Institute for Mathematical and Statistical Innovation) travel award.
- **[Aug/2025]** Paper submitted to *IEEE Transactions on Evolutionary Computation*.
- **[Aug/2025]** *iPINNER* accepted by the *Journal of Computational Physics*.
- **[Jun/2025]** *fPINN-DeepONet* published in the *Journal of Computational Physics*.
- **[Dec/2024]** Awarded the Undergraduate Research Scholarship 2024–2025 (Top 5%), Purdue.
- **[Apr/2024]** Awarded the Spira Undergraduate Research Fellowship, College of Science, Purdue (1 / 6000).
- **[Mar/2024]** Office of Undergraduate Research Scholarship, Purdue (Top 5%).
- **[May/2023]** Thomas Arai Scholarship, Department of Mathematics, Purdue (Top 1%).
- **[Mar/2023]** *NSGA-PINN* published in *Algorithms*.

---

## 🧑‍🏫 Professional Service

Reviewer for:

- *IEEE Transactions on Neural Networks and Learning Systems* (TNNLS)
- *IEEE Data Science and Advanced Analytics* (DSAA)
- *SIAM Multiscale Modeling and Simulation* (MMS)
- *Journal of Computing and Information Science in Engineering*

---

## 📬 Contact

- 📧 `lu895 [at] purdue [dot] edu`
- 📍 610 Purdue Mall, West Lafayette, IN 47907, USA
- 🔗 [Google Scholar](https://scholar.google.com/citations?user=EFPK9yoAAAAJ&hl=en) · [GitHub](https://github.com/jeremylu916) · [ORCID](https://orcid.org/0009-0001-6001-6632) · [CV (PDF)](/files/Purdue.MSECE.Binghang.Lu.Resume.pdf)

I am always happy to talk about LLM post-training, continual learning theory, and physics-informed machine learning. If any of this resonates, feel free to reach out.

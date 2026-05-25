---
title: "Research"
permalink: /research/
author_profile: true
---

My research spans three closely interacting threads — **Large Language Models &amp; Safety**, **LLM Continual Learning**, and **AI for Science (AI4S)**. The common thread is *how to train large parametric models so that they remain stable, knowledge-preserving, and physically faithful when the world (or the task stream, or the PDE) changes underneath them*.

---

## 🧠 Large Language Models &amp; Safety

I study **post-training** of large language and reasoning models — in particular, how the *geometry* of the optimizer shapes what a model learns, forgets, and refuses.

- **Chain of Risk** *(arXiv 2026)* — characterizes how chain-of-thought reasoning compounds safety failures in large reasoning models; introduces *adaptive multi-principle steering* as a step-wise mitigation. [[paper]](https://arxiv.org/abs/2605.05678)

<figure>
  <img src="/images/chain-of-risk-fig.png" alt="Chain of Risk diagnosis-control loop diagram." style="max-width:100%;border:1px solid #e6e8eb;border-radius:6px;">
  <figcaption style="font-size:0.9em;color:#4a5159;margin-top:0.4em;"><strong>Chain of Risk.</strong> Stage-wise safety diagnosis of the reasoning trace and final answer feeds adaptive multi-principle steering, which activates only the safety directions relevant to the current hidden state.</figcaption>
</figure>

**Open questions I care about.** When does safety steering trade off against reasoning ability — and can we get both? How do unsafe intermediate steps interact with the spectral geometry of the model's representations?

---

## ♻️ LLM Continual Learning

I design optimizers and training schemes that let **pretrained LLMs keep learning** — absorbing new tasks, domains, and skills while preserving what they already know. My approach combines **spectral / orthogonal gradient projection** with the matrix-aware preconditioning of modern LLM optimizers.

- **Muon-OGD** *(arXiv 2026)* — Muon-based spectral orthogonal gradient projection. Updates are restricted to spectral subspaces orthogonal to prior-task representations, giving forgetting-resistant adaptation without sacrificing Muon's efficiency. [[paper]](https://arxiv.org/abs/2605.08949)

<figure>
  <img src="/images/muon-ogd-fig.png" alt="Muon-OGD overview: continual learning + projection geometry + spectral-norm Muon update." style="max-width:100%;border:1px solid #e6e8eb;border-radius:6px;">
  <figcaption style="font-size:0.9em;color:#4a5159;margin-top:0.4em;"><strong>Muon-OGD.</strong> A projection-based continual-learning objective (Frobenius geometry) is combined with the spectral-norm geometry of the Muon update, yielding a dual gradient update that protects the subspace spanned by previous-task representations.</figcaption>
</figure>

**Open questions I care about.** What is the right notion of "task subspace" for an LLM whose parameters are tied to language? Can spectral projections be made cheap enough to run at every step of post-training? How do we certify forgetting bounds without storing replay buffers?

---

## 🧪 AI for Science (AI4S)

On the scientific side, I build **physics-informed and operator-learning** methods for PDEs — including the *nonlocal*, *high-dimensional*, and *stiff* regimes where classical solvers struggle — together with the optimization machinery needed to train them.

- **fPINN-DeepONet** *(JCP 2025)* — operator learning for multi-term time-fractional mixed diffusion–wave equations. [[paper]](https://doi.org/10.1016/j.jcp.2025.114184)
- **iPINNER / MoPINNEnKF** *(JCP 2025)* — iterative PINN training coupled with ensemble Kalman filtering for calibrated parameter and state estimation. [[paper]](https://arxiv.org/abs/2506.00731)
- **AdamFLIP** *(arXiv 2026)* — adaptive feedback-linearization optimizer enforcing hard constraints in PINN training. [[paper]](https://arxiv.org/abs/2605.08408)

<figure>
  <img src="/images/adamflip-fig.png" alt="AdamFLIP algorithm: feedback-linearization-corrected Adam update for hard-constrained PINN training." style="max-width:100%;border:1px solid #e6e8eb;border-radius:6px;">
  <figcaption style="font-size:0.9em;color:#4a5159;margin-top:0.4em;"><strong>AdamFLIP.</strong> A closed-form feedback-linearization multiplier projects the raw gradient onto the constraint tangent before standard Adam momentum and adaptive-step bookkeeping — enforcing the hard constraint <code>h(θ) = 0</code> step-by-step rather than via a soft penalty.</figcaption>
</figure>
- **Muon with Spectral Guidance** *(arXiv 2026)* — Muon augmented with spectrum-aware step sizes for stiff, multi-scale scientific-ML objectives. [[paper]](https://arxiv.org/abs/2602.16167)
- **Neural-POD** *(arXiv 2026)* — plug-and-play neural-operator framework for infinite-dimensional functional nonlinear proper orthogonal decomposition. [[paper]](https://arxiv.org/abs/2602.15632)
- **Morphy-Net** *(CMAME 2026, accepted)* — evolutionary multi-objective search with replica exchange for training physics-informed neural operators. [[paper]](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=6253351)
- **NSGA-PINN** *(Algorithms 2023)* — multi-objective NSGA-II training for PINNs; mitigates loss-balancing pathologies. [[paper]](https://doi.org/10.3390/a16040194)

**Open questions I care about.** Can a single foundation operator model transfer across PDE families? How do we get rigorous a-posteriori error estimates for neural surrogates? What is the right inductive bias for fractional / nonlocal operators?

---

## Co-authors

- **[Guang Lin](https://www.math.purdue.edu/~lin491/)** — Associate Dean for Research; Moses Cobb Stevens Professor of Mathematics and Mechanical Engineering, **Purdue University**
- **[Na Li](https://nali.seas.harvard.edu/)** — Winokur Family Professor of Electrical Engineering and Applied Mathematics, **Harvard University**
- **Changhong Mou** — Assistant Professor, Department of Mathematics &amp; Statistics, **Utah State University**
- **Zhaopeng Hao** — School of Mathematics, **Southeast University**, China
- **Runyu (Cathy) Zhang** — **MIT**
- **Xiaomin Li** — **Harvard University**

---

📄 A full list of papers, with categories aligned to the thrusts above, is on the [Publications page](/publications/). My most up-to-date record is on [Google Scholar](https://scholar.google.com/citations?user=EFPK9yoAAAAJ&amp;hl=en).

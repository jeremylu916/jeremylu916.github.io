---
title: "Chain of Risk: Safety Failures in Large Reasoning Models and Mitigation via Adaptive Multi-Principle Steering"
collection: publications
category: llm
permalink: /publication/2026-chain-of-risk
excerpt: 'Characterizes how chain-of-thought reasoning compounds safety failures in large reasoning models and proposes adaptive multi-principle steering as a mitigation.'
date: 2026-04-01
venue: 'arXiv preprint'
paperurl: 'https://arxiv.org/abs/2605.05678'
citation: 'Li, X., Hou, J., Deng, Z., Zhang, Z., Li, T., Lu, B., Hu, B., Zhao, Y., &amp; Hao, Y. (2026). &quot;Chain of Risk: Safety Failures in Large Reasoning Models and Mitigation via Adaptive Multi-Principle Steering.&quot; <i>arXiv:2605.05678</i>.'
---

This work studies *chain-of-risk* — the observation that errors and unsafe intermediate steps accumulate along the reasoning trace of large reasoning models, often producing more harmful outputs than direct-answer baselines. We propose **adaptive multi-principle steering**, which dynamically rebalances safety constraints across reasoning steps to suppress these compounding failures without sacrificing task performance.

<figure>
  <img src="/images/chain-of-risk-fig.png" alt="Two-row diagram of the Chain of Risk diagnosis–control loop: stage-wise safety diagnosis of CoT and final answer, followed by adaptive multi-principle steering that activates only relevant safety directions in the hidden state." style="max-width:100%;border:1px solid #e6e8eb;border-radius:6px;">
  <figcaption style="font-size:0.92em;color:#4a5159;margin-top:0.5em;"><strong>Figure 1.</strong> Overview of the proposed diagnosis-control loop. Stage-wise diagnosis evaluates reasoning traces and final answers under the same twenty-principle rubric, revealing <em>unsafe</em>, <em>leak</em>, and <em>escape</em> failures. Adaptive multi-principle steering then reuses the principle-level labels to construct safety directions and applies only the directions activated by the current hidden state.</figcaption>
</figure>

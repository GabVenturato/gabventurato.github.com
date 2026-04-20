---
layout: page
title: NeSy-MM
description: Relational neurosymbolic Markov models
img:
importance: 1
category: work
---

Our most powerful AI agents rely almost exclusively on neural networks, which cannot easily be told to obey certain rules or incorporate background knowledge. **Relational Neurosymbolic Markov Models (NeSy-MMs)** combine the learning abilities of neural networks with the guarantees of symbolic reasoning, applied to sequential decision-making under uncertainty.

NeSy-MMs integrate neurosymbolic AI with Markov models by using **probabilistic models over relations** as their core representation. Unlike standard hidden Markov models that use unstructured latent variables, NeSy-MMs decompose symbolic relations over time, similar to how planning algorithms work, while learning unknown dynamics with neural networks.

This gives NeSy-MMs three key abilities that other models lack:

1. **Consistent generation.** NeSy-MMs generate sequences that respect given constraints (e.g., navigation rules), while deep Markov models and visual transformers trained on the same data fail to do so.
2. **Out-of-distribution generalisation.** Trained on small grids with one enemy, NeSy-MMs generalise to larger grids, more enemies, and longer time horizons, unlike transformer baselines.
3. **Test-time interventions.** New constraints can be added at test time without retraining (e.g., forbidding the agent from entering part of the room).

<div class="row mt-5">
    <div class="col-sm mt-3 mt-md-0 text-center">
        <p><strong>Deep Markov Model</strong></p>
        <!-- TODO: Replace with actual GIF (Figure 3 left — blurry/superposition agent) -->
        <img class="rounded z-depth-1" style="width: 80%" src="/assets/img/nesy-mm/generation_dmm.gif" alt="Deep Markov Model generation">
    </div>
    <div class="col-sm mt-3 mt-md-0 text-center">
        <p><strong>NeSy-MM (Ours)</strong></p>
        <!-- TODO: Replace with actual GIF (Figure 3 middle — crisp and consistent) -->
        <img class="rounded z-depth-1" style="width: 80%" src="/assets/img/nesy-mm/generation_nesymm.gif" alt="NeSy-MM generation">
    </div>
    <div class="col-sm mt-3 mt-md-0 text-center">
        <p><strong>Visual Transformer</strong></p>
        <!-- TODO: Replace with actual GIF (Figure 3 right — crisp but wrong dynamics) -->
        <img class="rounded z-depth-1" style="width: 80%" src="/assets/img/nesy-mm/generation_transformer.gif" alt="Visual Transformer generation">
    </div>
</div>

<h2 class="mt-5">resources</h2>

- **Paper**: [arXiv](https://arxiv.org/pdf/2412.13023)
- **Code**: [ML-KULeuven/nesy-mm](https://github.com/ML-KULeuven/nesy-mm)
- **Blog post**: [AIHub](https://aihub.org/2026/02/19/relational-neurosymbolic-markov-models/)

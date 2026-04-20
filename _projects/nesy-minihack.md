---
layout: page
title: NeSy MiniHack
description: Neurosymbolic RL with Probabilistic Logic Shields
img:
importance: 2
category: work
---

Reinforcement learning agents can learn impressive policies, but they often exhibit unsafe behaviour during both training and deployment.
In this project, we integrate neurosymbolic AI with reinforcement learning by using **probabilistic logic programs as shields** to guide the agent towards safe behaviour in [MiniHack](https://github.com/facebookresearch/minihack), a challenging procedurally-generated roguelike environment based on NetHack.

The probabilistic logic shield, written in [ProbLog](https://dtai.cs.kuleuven.be/problog/), encodes domain knowledge about dangerous situations (e.g., lava, monsters) and intervenes on the agent's action selection to prevent unsafe actions.
This allows the agent to **learn faster** and **die significantly less** during training compared to an unshielded baseline.

This project won the **Best Technical Demonstration Award** at AAAI 2025.

<div class="row mt-5">
    <div class="col-sm mt-3 mt-md-0 text-center">
        <p><strong>With Shield (Safe)</strong></p>
        <img class="rounded z-depth-1" style="width: 60%" src="/assets/img/nesy-minihack/safe_death_count.gif" alt="Safe agent behaviour with death count">
    </div>
    <div class="col-sm mt-3 mt-md-0 text-center">
        <p><strong>Without Shield (Unsafe)</strong></p>
        <img class="rounded z-depth-1" style="width: 60%" src="/assets/img/nesy-minihack/unsafe_death_count.gif" alt="Unsafe agent behaviour with death count">
    </div>
</div>

<h2 class="mt-5">resources</h2>

- **Code**: [ML-KULeuven/nesy-minihack](https://github.com/ML-KULeuven/nesy-minihack)
- **Video**: [YouTube demo](https://youtu.be/3uLVxwlcSQc)
- **Project page**: [dtai.cs.kuleuven.be](https://dtai.cs.kuleuven.be/projects/nesy/minihack.html)

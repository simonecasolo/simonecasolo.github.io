---
layout: page
title: Bayesian Amortized Inference for Industrial Processes
description: Simulation-based Bayesian inference for fast uncertainty-aware parameters estimation in industrial process models.
img: assets/img/SBI_scheme.png
importance: 2
category: work
related_publications: false
---

This project explores Simulation Based Inference (SBI) a **Bayesian amortized inference** method for industrial process systems, using simulation-based inference to learn reusable probabilistic estimators from model-generated data. The goal is to support fast, uncertainty-aware inference for process monitoring, calibration, and decision support when direct likelihood evaluation is difficult or expensive. The workflow combines prior sampling, process simulation, neural density estimation, and posterior inference so that repeated inference tasks can be handled efficiently after training.

We applied this framework to heat exchangers subject to fouling and leakages [arXiv](http://arxiv.org/abs/2604.20735), and then to complex full-plant scale controlled systems (in press).

<div class="row justify-content-sm-center mt-3">
  <div class="col-sm-10">
    {% include figure.liquid path="assets/img/SBI_scheme.png" title="Simulation-based Bayesian inference workflow for industrial processes" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

[Open the original scheme PDF](/assets/img/SBI_scheme.pdf).

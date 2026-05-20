---
layout: post
title: "Publication of floatCSEP: An Application to Deploy and Conduct Reproducible Prospective Earthquake Forecasting Experiments"
date: 2026-04-08 00:00:00 -0000
categories: news publication
---

A new paper introducing floatCSEP — a Python application that standardizes and orchestrates the workflow of earthquake forecasting experiments — by Pablo Iturrieta, William H. Savran, Marcus Herrmann, José A. Bayona, Matthew C. Gerstenberger, Kenny Graham, Philip J. Maechling, Warner Marzocchi, Leila Mizrahi, Danijel Schorlemmer, Francesco Serafini, Fabio Silva, and Maximilian J. Werner.

Building on CSEP principles, floatCSEP tackles a long-standing challenge in the field: the original CSEP Testing Centers relied on centralized, rigid infrastructures that tightly coupled data management to local hardware, limiting reusability, scalability, and community engagement. floatCSEP fills this gap by introducing the concept of the “Floating Experiment,” where software and data artifacts are decoupled from specific physical infrastructure and encapsulated as self-contained, reproducible packages that can run on any machine with sufficient computational resources.

The application manages the complete experiment lifecycle — from model integration and catalog handling to forecast generation, evaluation, visualization, and reporting. It supports both time-invariant and time-dependent experiments and integrates external models through containerized Docker environments. Beyond supporting new official CSEP experiments, floatCSEP enables independent researchers to create new retrospective or prospective studies, benchmark novel models against established ones, and contribute to the continuous evaluation of operational earthquake forecasting systems. Together with pyCSEP, open-source forecasting models, and long-term open-science repositories, floatCSEP helps lay the foundation for robust, collaborative benchmarks in earthquake forecasting research.

[Read the article][paper-link]

[Explore the GitHub repository][github-repo]

[paper-link]: https://doi.org/10.21105/joss.09408
[github-repo]: https://github.com/cseptesting/floatcsep
---
layout: post
title: "Publication of EarthquakeNPP: A Benchmark for Earthquake Forecasting with Neural Point Processes"
date: 2026-03-24 00:00:00 -0000
categories: news publication
---

A new paper published in Transaction of Machine Learning Research (TMLR) – EarthquakeNPP: A benchmark for Earthquake Forecasting with Neural Point Processes by Sam Stockman, Daniel John Lawson, and Maximilian J. Werner.

This article takes a critical look at the intersection of machine learning and seismology. For decades, earthquake forecasting has been dominated by classical statistical models like the Epidemic-Type Aftershock Sequence model, which explicitly capture how earthquakes trigger subsequent events. While Neural Point Processes (NPPs) have recently emerged as a flexible alternative, their evaluation has been limited by outdated and flawed benchmarks, some even suffering from data leakage and incomplete datasets.

To address this, the authors introduce EarthquakeNPP, a new benchmarking framework built on curated earthquake catalogs from California spanning 1971–2021. Crucially, the platform aligns machine learning evaluation practices with those used in seismology, incorporating both likelihood-based and generative metrics. This creates a more realistic and rigorous testing ground, enabling fair comparisons between NPPs and established models. The benchmark also includes the ETAS model as a baseline, ensuring that new approaches are judged against the current standard.

[Read the article: EarthquakeNPP: A benchmark for Earthquake Forecasting with Neural Point Processes][paper-link]

[Explore the GitHub repository][github-repo]

[paper-link]: https://openreview.net/pdf?id=dIcNAg6ZuZ
[github-repo]: https://github.com/ss15859/EarthquakeNPP
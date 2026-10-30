---
layout: page
title: ETAS and ETASV1.1 Models
permalink: /etas-models/
---

These versions of the Epidemic-Type Aftershock Sequence (ETAS) model are described in details in [Zhuang (2011](https://link.springer.com/article/10.5047/eps.2010.12.010). Both models consider a spatially varying background rate (constant in time), and a space triggering function that depends on the magnitude of the parent event, so that larger earthquakes produce aftershocks in a larger area.

Both rely on the following conditional intensity's formulation:

$latex \lambda(t, x, y, m \vert \mathcal H_t) = \pi(m) \left( \mu(x,y) + \sum_{(t_h, x_h, y_h, m_h) \in \mathcal H_t} k(m_h) g(t - t_h) f(x-x_h, y-y_h, m_h) \right)$

The parameters $latex mu, alpha, K, c, p, a, b$ of the ETAS model were calibrated with more than 4,700 earthquakes with magnitude greater or equal to 3.95 and less or equal to 6.0, reported by the ANSS catalog from January 1, 1898 to January 1, 1985. This parameters were used to produce daily (from 00:00:01 to 23:59:59) grid-based forecasts for events with magnitude above 3.95 occurring in California.

# Downloads

[ETAS 1-day forecasts from 1 August 2007 to 30 August 2018 (5.82GB)](https://g-3a9041.a78b8.36fe.data.globus.org/csep/csep1/files/ETAS_1day.hdf5)
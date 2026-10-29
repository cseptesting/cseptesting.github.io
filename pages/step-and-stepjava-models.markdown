---
layout: page
title: STEP and STEPJAVA Models
permalink: /step-and-stepjava-models/
---

These models are two instances of the Short-term Earthquake Predictability\cite{gerstenberger2005real} (STEP) model Similarly to ETAS, the STEP model also is composed of a background and aftershock (or cluster) component but there are two crucial differences.

Firstly, the STEP model assumes cluster-specific parameters for the magnitude and space-time distributions of aftershocks, and model parameters for each cluster are adjusted as new earthquakes accrue to it. 

Secondly, the background and aftershock components are not combined by summing them but by taking the maximum. The model by Frankel et al. (1997)\cite{frankel1996national}, which then underpinned the US national seismic hazard model, is used as background model, while the model by Reasenberg and Jones (1989)\cite{reasenberg1989earthquake} is used for the aftershock component.

The difference between STEP and STEPJAVA is that the STEP model was implemented in MatLab while STEPJAVA in JavaScript. This is because the MatLab version was deprecated, and the Java version was installed as replacement. Both models are calibrated on M=4.0 seismicity recorded from January 1, 1993 to November 1, 2006 from the ANSS catalogue.
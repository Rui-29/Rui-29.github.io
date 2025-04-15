---
layout: post
title: Demand Response-Based Battery Energy Storage Systems
subtitle: Design and Operation Optimization
cover-img: /assets/img/BESS.png
thumbnail-img: /assets/img/thumbnail_BESS.jpg
share-img: /assets/img/path.jpg
tags: [Demand Response, Battery Energy Storage Systems, Transformer, Journal]
author: Rui Li, Qingshi Tu, Haibo Feng, and Zhengbo Zou
---
Our [new paper](https://doi.org/10.1016/j.enbuild.2025.115738) has been accepted for publication in [Energy & Buildings](https://www.sciencedirect.com/journal/energy-and-buildings)!  

### Overview

This study presents an integrated framework that connects medium-term electricity demand forecasting with the design and operation optimization of battery energy storage systems (BESS) under demand response (DR) programs.

**Key motivations:**
- Most existing DR studies focus either on DR or BESS optimization, rarely integrating both in a realistic, data-driven way.
- Short-term forecasting dominates current work, limiting extended planning horizons for electricity procurement and system control.

### Method

- Applied the Informer model for medium-term demand forecasting (up to 30 days) using real electricity usage data from 72 buildings.
- Developed a Mixed-Integer Nonlinear Programming (MINLP) model to optimize BESS type, size, and hourly control under time-of-use pricing and carbon intensity constraints.
- Used real-world urban-level data from ASHRAE 90.1-2010 climate zone 5 (Vancouver, Canada).

![Overall_architecture](https://Rui-29.github.io/assets/img/thumbnail_BESS.jpg){: .mx-auto.d-block :}  

### Results

- Informer outperformed Bi-LSTM and vanilla Transformer models across all forecasting horizons, with up to 27% reduction in MSE.
- The 30-day model significantly outperformed iterative 1-day forecasting for long-range prediction.
- Optimization identified lithium-ion batteries as the most cost-effective and carbon-efficient BESS option.

**For the three winter months analyzed:**
- Electricity cost savings: **C$311,000**
- CO₂-equivalent emission reduction: **471 tonnes**

---

### Notes

The framework is designed to be scalable to urban-scale implementation and can support extended planning for DR programs, predictive maintenance, and energy procurement. Future work could incorporate additional system integration (e.g., HVAC, PV) and more complex control strategies (e.g., RL-based control).  
Stay tuned for more updates on leveraging technology to drive sustainability and innovation in the built environment!  
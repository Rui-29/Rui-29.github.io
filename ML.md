---
layout: page
title: MACHINE LEARNING
subtitle: 
---
This page is for collecting tech-resources related to **ML and its applications**.  

**Papers/Seminars** that I think worth a reading/listening are also listed.

### Tech-resources
**Jun 2020** | [GNN using Pytorch Geometric | Stanford University](https://youtu.be/-UjytpbqX4A?si=UMotffD0bpDXo4fy) together with [official tutorial](https://pytorch.org/tutorials/beginner/basics/buildmodel_tutorial.html).  
**Notes**:  
* The overall Pytorch workflow is to class a network, define parameters and forward functions. Remember to add *self.* Before parameter, otherwise it won't be added to parameter lists.  
* Training metric (loss) need to be differentiable, but evaluation metric no need, sklearn have a lot evaluation metrics already, no need to hand write.  
* The precision is the ratio tp / (tp + fp), recall tp / (tp + fn), f1 score search online, all of these are 1 best 0 worst.  

**Comments**: powerful lightweight yet high fidelity simulation engine, better to utilize its efficiency in integrative control (e.g., serve as RL env). Better to combine with 3D modeling tools and more user-friendly interface to accelerate modeling speed (actually OpenStudio + SketchUp plugins is exactly for this).  

### Papers/Seminars
**Jul 2021** | [IBPSA-Python Programming for Energy Modelers](https://www.youtube.com/live/lDN_nybJq20?si=cAvhqDLQWy8ZZdAv) by [Clayton Miller](https://scholar.google.ch/citations?user=akL857IAAAAJ&hl=en).  
    **Notes**: python is great in enhancing the ability from data processing to time-series forecasting, till the sophisticated control.
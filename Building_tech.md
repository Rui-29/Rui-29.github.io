---
layout: page
title: BUILDING TECHNOLOGY
subtitle: ENERGY MODELING and PYTHON
---
This page is for collecting tech-resources related to **building modeling** and **object oriented programming (OOP)-modeling integration**.  

**Papers/Seminars** that I think worth a reading/listening are also listed.

### Tech-resources
**Mar 2024** | [EnergyPlus  Tutorial](https://youtu.be/j1foofH0eRw?si=w0iuGnrGr_jQKXRX)  
    **Notes**: 
    - Open EP-lanuch.exe, Inputs to EnergyPlus are input data files (IDF) and weather file (epw). Weather file can be downloaded from [climate_onebuilding](https://climate.onebuilding.org/). "CTRL+L" can shrink IDF class list to existing ones.  
    - Geometry model can be drawn directly, but really troublesome. Thermal zones are first defined, following constructions and materials. Internal gains mainly include occupant, equipment and lighting, can edit schedule of them by adding new objs, then link to designated zones.  
    - Infiltration is not intentional, air renovation and HVAC is intentional. Ideal loads are not consuming electricity but district thermal energy.  
    **Comments**: powerful lightweight simulation engine, better to utilize its efficiency in integrative control (e.g., serve as RL env). has to combine with 3D modeling tools and more user-friendly interface to accelerate modeling speed.

### Papers/Seminars
**Jul 2021** | [IBPSA-Python Programming for Energy Modelers](https://www.youtube.com/live/lDN_nybJq20?si=cAvhqDLQWy8ZZdAv) by [Clayton Miller](https://scholar.google.ch/citations?user=akL857IAAAAJ&hl=en).  
    **Notes**: python is great in enhancing the ability from data processing to time-series forecasting, till the sophisticated control.
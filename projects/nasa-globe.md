---
layout: default
title: NASA GLOBE
---

# NASA GLOBE
NASA GLOBE (Global Learning and Observations to Benefit the Environment), launched by Al Gore in the 1990s, is a global earth-monitoring citizen science and education program. Over the course of three decades, participants have contributed hundreds of millions of observations through manual in-situ measurements and weather stations. Variables include air and surface temperature (the focus of the figures shown here study), mosquito habitats, soil moisture, and water transparency. 

Characteristic of citizen science, GLOBE’s data stream is irregular and noisy, creating challenges to analysis. Investigating these data provides insight into how citizen science can advance environmental understanding and play a role in monitoring a changing world.

The figures below are part of my investigation into GLOBE air and surface temperature data. To assess the spatiotemporal availability of GLOBE temperature data, I grouped observations into cells of equal area then used a custom metric for data quality, Qcell, to score each of the cells. In general, Qcell, which ranges from 0–1 (worst–best) rewards data availability and penalizes inconsistent sampling. 

Cells with high Qcell scores were chosen for further analysis along with sites inside those cells with high data outputs. In addition to cells and sites, I analyzed data at the global and country scale. Using these four scales of analysis, I used Structured Interpolation Gaussian Processes (SKI-GP) to model GLOBE temperature time series, imputed model outputs into missing GLOBE values, then ran STL decompositions to compare to an STL-decomposed signal from ERA5-Land, a trusted reanalysis model.

### - [NASA GLOBE Data System Analysis](portfolio/nasa-globe)
A research + engineering project to evaluate data quality, build scalable pipelines, and propose a design framework for improving citizen-science data systems.
- Feb 2025 - Present
- CUNY Advanced Science Research Center
- **Publication:** in progress...check back soon

### - [Albatross Flight Performance](portfolio/albatross-flight-performance)
My Masters thesis work on the effects of winds and waves on albatross flight performance.
- Aug 2022 - Present
- NASA
- **Publication:** [Differential impacts of wind and waves on albatross flight performance in two ocean basins](https://link.springer.com/article/10.1186/s40462-025-00614-w)

### - [Urban Heat Mitigation](portfolio/urban-heat-mitigation)
My work with NASA DEVELOP. Quantifying and mapping urban heat mitigation in Chatham County, Georgia
- Jan - Apr 2025
- NASA
- **Publication:** [Chatham County Health & Air Quality: Mapping Urban Heat to Identify Priority Mitigation Areas in Chatham County, Georgia](https://ntrs.nasa.gov/citations/20250005541)

### - [Marine Ecosystem Indicators](portfolio/marine-ecosystem-indicators)
A quantitative analysis of the health of the New York Bight in conjuction with the NY State Department of Environmental Conservation.
- Sep - Dec 2024
- Stony Brook University
- **Report**: [New York Bight Indicator Report 2024](https://static1.squarespace.com/static/68b223ce11aaa7708d75452f/t/68b79fd6fa9a262ebbe9b485/1756864470688/New+York+Bight+Indicator+Report+2024.pdf)

### - [Avian Parasitology](portfolio/avian-parasitology)
Tracking the community composition of malarial parasites infection common yellowthroat birds
- Sep 2018 - May 2021
- Skidmore College
- **Thesis**: [Temporal dynamics of malarial parasites infecting common yellowthroats (Geothlypis trichas)](https://static1.squarespace.com/static/68b223ce11aaa7708d75452f/t/68c0d6570d70650370cab06d/1757468247915/Maywar2021.pdf)

<br>

<--- [Projects](.) <br>
<--- [Homepage](..)
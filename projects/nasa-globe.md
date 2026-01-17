---
layout: default
title: NASA GLOBE
---

# NASA GLOBE

NASA GLOBE (Global Learning and Observations to Benefit the Environment), launched by Al Gore, is a global earth-monitoring citizen science and education program. 
Since 1995, participants have contributed hundreds of millions of observations through manual in-situ measurements and automated sensors. 
Variables recorded by this program include air and surface temperature, mosquito habitats, soil moisture, and water transparency. 

Characteristic of citizen science, GLOBE’s data stream is irregular and noisy, creating challenges for analysis. 
Investigating these data provides insight into how citizen science can advance environmental understanding and play a role in monitoring a changing world.
I assessed GLOBE data along two major axis: data availability, the volume of measurements across both time and space, 
and data validity, the accuracy and cogency of measurements.

A publication is in progress...check back here for updates.

<br>

## Data availability

I created a methodology to assess the availability of data from various GLOBE protocols.
The figure below displays the output of such an assessment for air temperature measurements taken at solar noon.
The highlighted region of the map, and the highlighted point within the region, are areas with high data output which I assess in further detail.

{% include figure.html
   src="/assets/figures/ATN_map.png"
   caption="$ρ_{(R,Q)}$ scores of air temperature measurements at noon."
%}

I quantified the spatiotemporal distribution of data from various protocols using a custom metric for data regularity and quantity, $ρ_{(R,Q)}$.

$$
\rho_{(R,Q)}
= \frac{n/D}{1+RCV_{Q}(\Delta T)}
$$

where n is the number of days with an observation in a given cell, D is the total number of days covered by the entire dataset, 
and $RCV_{Q}(Δt)$ is the $RCV_{Q}$ of the duration (in days) between dates with at least one observation.

$$
RCV_{Q} = 0.75 x \frac{IQR}{m}
$$

where m is the median and IQR is the interquartile range. RCVQ, coined by <a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC9196089/" target="_blank" rel="noopener noreferrer">Arachchige et al. (2020)</a>,
is an alternative to the coefficient of variation which measures dispersion while providing resistance to outliers. 
Ranging from 0 to 1, $ρ_{(R,Q)}$ rewards high volumes of data (quantity) and penalizes inconsistent sampling (irregularity).

<br>

## Data validity

To assess data validity, data were compared to a trusted, alternative source of data to determine areas of agreement and disagreement. 
ERA5-Land (<a href="https://rmets.onlinelibrary.wiley.com/doi/10.1002/qj.3803" target="_blank" rel="noopener noreferrer">Hersbach et al. 2020</a>) 
was used to provide the trusted alternative for air temperature and surface temperature measurements.

{% include figure.html
   src="/assets/figures/ATN_STN_ERA5.png"
   caption="Seasonally de-trended air temperature timeseries at the full, cell, and site scale."
%}

Temperature timeseries were aggregated worldwide (<u>full</u> scale), and within a designated <u>cell</u> and <u>site</u> (both highlighted in the map).
GLOBE data at the three spatial scales were seasonally de-trended using STL decomposition and compared to the data from the trused alternative.

<br>

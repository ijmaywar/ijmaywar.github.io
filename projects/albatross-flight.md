---
layout: default
title: Albatross Flight Performance
---

# Albatross Flight Performance

Albatrosses embark on multi-day foraging trips in the open ocean, using winds and waves to conserve energy expenditure by fueling soaring flight. 
Fitted with an accelerometer (tri-axial acceleration sensor) and a GPS, we can analyze albatross flight performance relative to local wind and wave conditions. 

I developed data and signal processing methods to analyze tens of thousands of sensor data hours, plus environmental data. 
Using these data, I conducted a comparative study of the flight performance of five albatross species across two ocean basins, the subject of my master's thesis 
and a resulting <a href="https://doi.org/10.1186/s40462-025-00614-w" target="_blank" rel="noopener noreferrer">publication</a>.
The framework of these analyses are being used by colleagues to investigate the flight performance of Giant Petrels.

My work suggests that there is a divergence in environmental energy extraction for soaring across albatross species in the Southern Ocean and North Pacific.
The Southern Ocean species appears to rely more on winds whereas North Pacific species relied more on swells.
This divergence in behavior is likely the result of differences in the regional winds and swells between the two ocean basins.

<br>

<p align="center">
  <video width="550" autoplay loop muted playsinline preload="metadata">
    <source src="{{ '/assets/figures/bird_track_v10.mp4' | relative_url }}" type="video/mp4">
    Your browser does not support the video tag.
  </video>
  
  <span class="figure-caption">
    A black-footed albatross foraging off the coast of Midway Atoll in the North Pacific (north of Hawaii).
    Wind field and wind speed displayed simultaneously with GPS track.
  </span>
</p>

<br>

<div style="display: flex; align-items: center; gap: 1rem;">

  <!-- Left image -->
  <img src="{{ '/assets/images/IAPC7.jpg' | relative_url }}"
       alt="iapc7"
       width="300">

  <!-- Right column -->
  <div style="display: flex; flex-direction: column; gap: 2rem;">

    <!-- Top (rectangular) image -->
    <img src="{{ '/assets/images/IAPC7_crowd.jpg' | relative_url }}"
         alt="IAPC7 poster"
         width="320">

    <!-- Text -->
    <div>
      I had the opportunity to present early findings of this work at the
      7th International Albatross and Petrel Conference (IAPC7) held in
      Ensenada, Mexico in May 2024.
    </div>

  </div>

</div>

<br>

{% include figure.html
   src="/assets/images/Molly229.JPG"
   caption="A black-browed albatross mounted with sensors (photo credits to Rachael Orben)."
%}

<br>

{% include figure.html
   src="/assets/figures/GAM_V_2.png"
   caption="The outputs of a GAM predicting the flap rate of foraging albatrosses using wind speed and wave height predictors."
%}

<br>

---
layout: page
title: Understanding Geothermally Induced Seismicity
description: Exploring the vibrational effects of geothermal energy on urban structures
img: assets/img/P5.jpg
importance: 1
category: work
related_publications: true
---
<div class="project-introduction">
    <p>
        This research is a key component of the collaborative <a href="https://geothermie-allianz.de/en/home/" target="_blank">Geothermie-Allianz Bayern</a> initiative, aimed at harnessing deep geothermal energy in Bavaria, Germany.
    <p>
        The Bavarian Molasse Basin provides ideal conditions for geothermal energy, but geothermal operations as shown in Figure 1, particularly during subsurface water injection, can induce micro-seismic events that cause building vibrations. Although these vibrations are usually harmless, they have led to public concern due to their annoyance and, in rare cases, panic from stronger events. This project seeks to better understand these impacts to enhance public support and mitigate risks.
    </p>

<div class="row">
    <div class="col-sm mt-3 mt-md-0 text-center">
        {% include figure.liquid loading="eager" path="assets/img/P5plant.png" title="schematic sketch GPP" class="img-fluid" width="30%" %}
    </div>
</div>
<div class="caption text-center">
    Figure 1. Definition sketch explaining the energy production process of a typical geothermal power plant.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0 text-center">
        {% include figure.liquid loading="eager" path="assets/img/P5citizens.png" title="citizens council meeting in Puccheim, Germany" class="img-fluid" width="80%" %}
    </div>
</div>
<div class="caption text-center">
    Figure 2. Meeting of the citizens' initiative against geothermal energy in Puccheim, Germany. Citizens voted against geothermal explorations in their town unless provided with a safe and uncomplicated damage management plan.
</div>

    <p> 
        The project deals with the analysis of groud motion data as well as the vibrational analysis of the urban structures. A recent study {% cite taddei2024development %} in this direction examines small earthquakes caused by geothermal power plants in Southern Germany and develops new equations to predict ground motion during these events. The research uses data from a power plant in Insheim, Germany and combines it with simulated data for the Munich area. The findings highlight the need for region-specific ground motion prediction equations. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0 text-center">
        {% include figure.liquid loading="eager" path="assets/img/P5map.png" title="GPP and seismic recording stations" class="img-fluid" width="70%" %}
    </div>
</div>
<div class="caption text-center">
    Figure 2. Map illustrating the latitudes and longitudes of the GPP and the recording stations for events (left) Unterhaching on 2013-04-16 at 21:51:42 UTC, recorded at UH1, UH2, UH3; (right) Poing on 2016-12-20 at 03:30:21 UTC, recorded at POI01, POI02, POI03. The GPP in Unterhaching is situated south of Munich, while the GPP in Poing lies to the east of Munich.
</div>        
       
        Another study by {% cite kumawat2024impact %} also tests the impact of the events on low-rise building, showing that while minor earthquakes meet serviceability and comfort standards, slightly stronger ones do not. These insights help improve risk assessments and safety planning for geothermal energy projects. The methodology used in this study combines two modeling techniques, finite element and lumped parameter models, to assess how buildings respond to vibrations caused by geothermal earthquakes. The building taxonomy considered in this approach focuses on how factors like building geometry, structural stiffness, material properties, damping, and soil type affect the model's performance. These factors were chosen based on past studies analyzing how residential buildings respond to vibrations from railways. This approach offers a new way to understand how physical variations impact building behavior during small seismic events.

<div class="d-flex flex-column align-items-center">
    <div class="w-100 text-center mt-3 mt-md-0" style="max-width: 80%;">
        {% include figure.liquid loading="eager" path="assets/img/P5UHrms.png" title="Unterhaching: frequency domain analysis of vibration" class="img-fluid" %}
    </div>
    <div class="w-100 text-center mt-3 mt-md-0" style="max-width: 80%;">
        {% include figure.liquid loading="eager" path="assets/img/P5POIrms.png" title="Poing: frequency domain analysis of vibration" class="img-fluid" %}
    </div>
</div>
<div class="caption text-center mt-2">
    Figure 1. Mean (indicated by the red line) and standard deviation of velocity amplitudes for a hybrid finite-element and lumped-parameter (FEM-LPM) building unit model with varying floor sizes on homogeneous soil. The top row presents top-floor slab center level velocities in the (top-left) x, (top-center) y, and (top-right) z directions, while the bottom row displays velocities at the top-floor slab center in the (bottom-left) x, (bottom-center) y, and (bottom-right) z directions. These results correspond to seismic data recorded at station UH1 during the Unterhaching seismic event.
</div>

<p>
    For more detailed information and additional results, please refer to the studies: {% cite taddei2024development %}, {% cite kumawat2024impact %}. All codes associated with this study are available in the GitHub repository <a href="https://github.com/Aditi-Kumawat/TaxoSim" target="_blank">TaxoSim</a>.  
</p>



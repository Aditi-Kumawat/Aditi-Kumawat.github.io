---
layout: page
title: Railway Track Modeling
description: Analytical model for ballasted railway track system
img: assets/img/P1.jpg
importance: 3
category: work
related_publications: true
---

Ballasted railway track systems are the most widely used railroad structures due to their low construction and maintenance costs. However, with the increasing speeds and loads of modern rail systems, assessing their performance under dynamic loads is crucial. Traditional track design methods often rely on static stress analysis, which falls short in accurately predicting the dynamic response of rail tracks, especially under the influence of moving trains.

This project focuses on developing an innovative frequency-dependent analytical model that accounts for the flexibility of the sleeper beam and the shear effects of ballast and subballast layers. The proposed model is designed to offer a more precise representation of the rail track's dynamic behavior while maintaining computational efficiency, making it highly applicable for practical engineering use. A few key aspects of the study are listed below. 
<ul>
    <li>The ballasted railway track structure is typically divided into two subsystems: (a) track superstructure and (b) track substructure. The superstructure includes components such as rail beams, rail pads, sleepers, and fastening systems, while the substructure consists of ballast, sub-ballast, and subgrade, as illustrated in Figure 1.

    <div class="row d-flex align-items-end">
        <div class="col-sm mt-3 mt-md-0">
            {% include figure.liquid loading="eager" path="assets/img/P1track2.png" title="Longitudinal-section of railway track" class="img-fluid" %}
        </div>
        <div class="col-sm mt-3 mt-md-0">
            {% include figure.liquid loading="eager" path="assets/img/P1track1.png" title="Cross-section of railway track" class="img-fluid" %}
        </div>
    </div>
    <div class="caption">
        Figure 1. Longitudinal-section (left) and cross-section (right) of the ballasted railway track system. The superstructure and substructure, along with various rail components, are highlighted [source: <a href="https://core.ac.uk/reader/195631460" target="_blank">link</a>].
    </div>
    </li>


    <li>The model integrates the effects of all critical substructural components through a frequency-dependent substructural stiffness approach. A simplified representation of the model is depicted in Figure 2.

    <div class="row d-flex align-items-end">
        <div class="col-sm mt-3 mt-md-0">
            {% include figure.liquid loading="eager" path="assets/img/P1model2.png" title="Track component idealization" class="img-fluid" %}
        </div>
        <div class="col-sm mt-3 mt-md-0">
            {% include figure.liquid loading="eager" path="assets/img/P1model1.png" title="Equivalent stiffness" class="img-fluid" %}
        </div>
    </div>
    <div class="caption">
        Figure 2. A schematic showing the idealization of the cross-section (left) and longitudinal-section (right) of the railway track.
    </div>
    </li>


    <li>To validate the model, time-domain track deflections are evaluated for various train velocities using track and ground parameters specific to high-speed railway lines on both stiff and soft soil sites. An example of this validation is shown in Figure 3, using data from an experimental study on rail deflection monitoring conducted in <a href="https://www.sciencedirect.com/science/article/abs/pii/S0267726116302251" target="_blank">Portugal</a> .
    

    <div class="row d-flex align-items-end">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/P1vald2.png" title="Axle loads and train geometry" class="img-fluid" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/P1vald1.png" title="Validation with experimental data" class="img-fluid" %}
    </div>
    </div>
    <div class="caption">
    Figure 3. Axle loads and train geometry (left), and comparison of the track deflection profiles from the proposed model with the experimental data.
    </div>
    </li>

    <li>Spectral analysis of rail beam deflections indicates that the dominant frequency content of deflection amplitudes is strongly influenced by wheel-load velocity. Time-domain analysis further reveals a critical velocity at which rail beam vibration amplitudes become significantly large. At this velocity, the rail track system vibrates at the isolation frequency associated with the sleeper-substructure system. The results of the spectral analysis are presented in Figure 4.

    <div class="row">
        <div class="col-sm mt-3 mt-md-0 text-center">
            {% include figure.liquid loading="eager" path="assets/img/P1isof.png" title="Spectral analysis of deflection results" class="img-fluid" width="50%" %}
        </div>
    </div>
    <div class="caption text-center">
        Figure 4. Spectral analysis highlighting the critical velocity and isolation frequency.
    </div>
    </li>
</ul>

For more detailed information and additional results on rail deflection across various soil conditions, please refer to the studies {% cite kumawat2019frequency %} and {% cite kumawat2021thesis %}. All codes associated with this study are available in the GitHub repository <a href="https://github.com/Aditi-Kumawat/FreqTrack" target="_blank">FreqTrack</a>.


---
layout: page
title: Track-Defect Analysis
description: Impact of rail/track irregularities on rail system safety
img: assets/img/P2rsqtthumb.jpg
importance: 2
category: work
related_publications: true
---

<p>
    This project is centered around the development of an innovative iterative technique designed to evaluate time-dependent loads on track structures, specifically addressing the challenges posed by various track defects. The interaction between a moving train and rail defects, such as rail-head corrugation or mud spots, can lead to unstable vibrations and rapid track degradation (see examples in <strong>Figure 1</strong> and <strong>Figure 2</strong>). These defects cause sudden variations in track stiffness and geometry, resulting in additional dynamic stresses that can compromise the structural health of the track.
</p>
<p>
    While existing methods can address some aspects of vehicle-track interaction, they often fall short in fully capturing the complex, coupled dynamics involved when multiple track defects are present. This project aims to bridge that gap by developing a more comprehensive and general technique to assess the potential damage to track structures, in order to ensure a more reliable rail transport.
</p>

<div class="row justify-content-center align-items-center">
    <div class="col-sm-4 d-flex justify-content-center">
        {% include figure.liquid loading="eager" path="assets/img/P2.jpg" title="rail head corrugation" class="img-fluid" style="max-width: 80%;" %}
    </div>
    <div class="col-sm-4">
        <div class="d-flex justify-content-center">
            {% include figure.liquid loading="eager" path="assets/img/P2rsqt.jpg" title="rail squat" class="img-fluid mb-3" %}
        </div>
        <div class="d-flex justify-content-center">
            {% include figure.liquid loading="eager" path="assets/img/P2wflt.jpg" title="wheel flat" class="img-fluid" %}
        </div>
    </div>
</div>
<div class="caption text-center mt-3">
    Figure 1. The rail and wheel head defects such as rail head <a href="https://www.jstage.jst.go.jp/article/jmtl/3/1/3_1_154/_article" target="_blank">corrugation</a> (left), <a href="https://mp.nl/en/solution/sound-measurements-board-train-detecting-rail-defects" target="_blank">rail squat</a> (top-right), and the wheel flat <a href="https://en.wikipedia.org/wiki/Flat_spot" target="_blank">wheel flat</a> (bottom-right) may cause unwanted stress on the track under dynamic loading and may also result in wheel-rail contact loss.
</div>

<div class="row d-flex align-items-end">
    <div class="col-md-6 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/P2prtrackgeom.jpg" title="Poor track geometry" class="img-fluid w-100" %}
    </div>
    <div class="col-md-6 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/P2mud.jpg" title="Mud-pumping" class="img-fluid w-100" %}
    </div>
</div>
<div class="caption">
    Figure 2. Track irregularities caused by <a href="https://railgallery.wongm.com/atsb.gov.au" target="_blank">poor track geometry</a> (left) and <a href="https://railgallery.wongm.com/" target="_blank">mud-pumping</a> (right).
</div>

  
<p>
    A new iterative approach is developed to analyze the coupled equation of motion of the vehicle-track system. This approach takes into account:
</p>

<ul>
    <li>The possibility of contact loss between the wheel and rail.</li>
    <li>Variation in track stiffness.</li>
    <li>The effect of track defects, such as rail-head corrugation, on track deflection.</li>
</ul>

<p>
    An example track model and vehicle idealization is shown in <strong>Figure 3</strong>. The track model used for the analysis can account for variations in track stiffness and geometry {% cite kumawat2022influence %}, while the vehicle model can account for loss of contact {% cite kumawat2022iterative %}.
</p>

<div class="row d-flex align-items-end">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/P2trckmod.png" title="track model" class="img-fluid" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/P2veh.png" title="vehicle idealization" class="img-fluid" %}
    </div>
</div>
<div class="caption">
    Figure 3. Basic idealization of track model (left) and vehicle (right).
</div>

<p>
    <strong>Figure 4</strong> illustrates the steps of the proposed iterative scheme via a flowchart. The proposed iterative scheme is applied along with the <a href="https://aditi-kumawat.github.io/projects/3_project/" target="_blank">track's Green's function</a> to obtain the time-domain response of a rail beam. Observations include:
</p>

<ul>
    <li>Loss of contact occurs when the wheel encounters rail-head corrugation.</li>
    <li>This contact loss results in high impact loads on the rail beam, leading to a significant increase in rail beam deflections (by up to 85% for undamped cases and 57% for damped cases).</li>
    <li>The method is described in full detail in the {% cite kumawat2022iterative %}.</li>
</ul>

<div class="row">
    <div class="col-sm mt-3 mt-md-0 text-center">
        {% include figure.liquid loading="eager" path="assets/img/P2flow.png" title="Iterative approach" class="img-fluid" width="80%" %}
    </div>
</div>
<div class="caption text-center">
    Figure 4. Flow chart showing the steps of the iterative approach used for analyzing the track model traversed by a multi-degree-of-freedom system.
</div>

<p>
    An important next step in this research involves validating the models using experimental data on rail deflections. During my academic stay at the University of Stuttgart, my team initiated an experimental study aimed at:
</p>

<ul>
    <li>Collecting acceleration data from rail beams along an 8-kilometer section (see <strong>Figure 5</strong>)of railway track near Stuttgart, Germany.</li>
    <li>Analyzing the data to identify rail defects and compare the observed rail beam deflections with those predicted by the model under identical track conditions.</li>
</ul>

<p>
    Unfortunately, the data collection process was interrupted due to the COVID-19 lockdown in 2020.
</p>

<div class="row">
    <div class="col-sm mt-3 mt-md-0 text-center">
        {% include figure.liquid loading="eager" path="assets/img/P2expmap.png" title="Map Neuffen" class="img-fluid" width="90%" %}
    </div>
</div>
<div class="caption text-center">
    Figure 5. Track Length: 8 km (Neuffen, Baden Württemberg, Germany).
</div>

<div class="row justify-content-center align-items-center">
    <div class="col-sm-4 d-flex justify-content-center">
        {% include figure.liquid loading="eager" path="assets/img/P2exp3.jpg" title="data collection station" class="img-fluid" style="max-width: 90%;" %}
    </div>
    <div class="col-sm-4">
        <div class="d-flex justify-content-center">
            {% include figure.liquid loading="eager" path="assets/img/P2exp1.jpg" title="wagon used for testing" class="img-fluid mb-3" %}
        </div>
        <div class="d-flex justify-content-center">
            {% include figure.liquid loading="eager" path="assets/img/P2exp2.jpg" title="sensor installed on axle box" class="img-fluid" %}
        </div>
    </div>
</div>
<div class="caption text-center mt-3">
    Figure 6. (left) Measurement facility inside the wagon, (top-right) Train wagon used for the experimental study, (bottom-right) accelerometer installed on axle box.
</div>

<p>
    For more detailed information and additional results on rail deflection across various track defects and wheel-rail contact conditions, please refer to the studies: {% cite kumawat2022iterative %}, {% cite kumawat2022influence %}, and {% cite kumawat2021thesis %}.
</p>
 


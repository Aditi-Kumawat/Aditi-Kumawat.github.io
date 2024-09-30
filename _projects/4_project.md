---
layout: page
title: Wave-propagation Analysis
description: Synthetic ground motion generation for induced events
img: assets/img/P4.jpg
importance: 4
category: work
related_publications: true
---
<div class="project-introduction">
    <p>
        As part of a broader initiative to harness the potential of <a href="https://geothermie-allianz.de/en/home/" target="_blank">geothermal energy in Bavaria</a>, this project focuses on addressing the challenges associated with its safe extraction. Geothermal energy is increasingly recognized as a sustainable and renewable resource. However, its extraction has been linked to minor earthquakes, raising concerns within both scientific circles and local communities about infrastructure safety.
    </p>

    <p> 
        Although these seismic events are typically few in number and relatively minor, they still pose potential risks to buildings and other structures. Research into the effects of these geothermally induced earthquakes is hampered by the limited availability of ground motion data. This scarcity makes it difficult to fully understand the impact of such events on the built environment.
    </p>

    <p>
        While there are advanced tools available for simulating seismic wave propagation in complex 3D soil environments, these methods often require significant computational resources, making them less accessible and efficient for widespread use. Given the challenges posed by limited data and the computational demands of existing techniques, there is a clear need for a more simplified and rapid approach to generating synthetic ground motion data.
    </p>

    <p>
        This project aims to fill that gap by developing a streamlined method for creating synthetic ground motions using a semi-analytical approach. Building on previous research, our methodology (illustrated in <strong>Figure 1</strong>) focuses on analyzing layered soil profiles to simulate the effects of seismic events associated with geothermal power plants. 
    </p>

</div>

<div class="row">
        <div class="col-sm mt-3 mt-md-0 text-center">
            {% include figure.liquid loading="eager" path="assets/img/P4flow.png" title="Evaluation Approach" class="img-fluid" width="1000%" %}
        </div>
    </div>
<div class="caption text-center">
    Figure 1. Flow chart showing the steps of the evaluation of the groud motion using the proposed approach. 
 </div>

<p>
    This project examines a case study of a geothermal facility located near Munich, Germany. Notably, in 2016, this site witnessed two seismic occurrences, each with a local magnitude of approximately 𝑀𝐿≈2.0. <strong>Figure 2</strong> offers a map pinpointing the site of the associated geothermal power plant. Additionally, the figure shows the three distinct recording stations: POI01, POI02, and POI03. These stations were situated at distances of 1.55 km, 5.6 km, and 3.3 km from the seismic events' epicenter, respectively.
</p>

<div class="row">
    <div class="col-sm mt-3 mt-md-0 text-center">
        {% include figure.liquid loading="eager" path="assets/img/P4map.png" title="Poing geothermal power-plant" class="img-fluid" width="40%" %}
    </div>
</div>
<div class="caption text-center">
    Figure 2. Map showing the geothermal power plant and the seismic data recording stations POI01, POI02, and POI03 located at distances of 1.55 km, 5.6 km, and 3.3 km from the epicenter.
</div>

<p>
    <strong>Figure 3</strong> presents the free-field velocities for the East-West (E-W), North-South (N-S), and vertical directions. Each figure displays the velocities evaluated at seven distinct locations, ranging from 𝑟=0.5 km to 𝑟=10 km from the epicenter. Each of the waveforms shown in Figures <strong>Figure 3</strong> is simulated for a frequency range of 0 – 10 Hz, chosen due to its significance for induced events. 
</p>

<p>
    Key observations include:
</p>
<ul>
    <li>A marked decrease in velocity values in each direction as the distance from the epicenter increases, primarily due to radiation damping.</li>
    <li>All simulated free-field vibrations remained below the 5 mm/s threshold, a benchmark set by DIN4150-3 for evaluating structural damages.</li>
    <li>From a computational standpoint:
        <ul>
            <li>Simulating frequency domain Green’s functions within the 0 to 10 Hz range took approximately 8 minutes.</li>
            <li>Evaluating time-domain waveform outcomes for a designated 𝑟 value took roughly 60 seconds.</li>
        </ul>
    </li>
    <li>These computations were executed on a 2x Intel-Xeon-Gold 6136 3GHz/12C computer with dual 12 processors.</li>
    <li>The relatively fast runtime of the presented methodology underscores its applicability in engineering contexts.</li>
</ul>

<div class="row">
    <div class="col-sm mt-3 mt-md-0 text-center">
        {% include figure.liquid loading="eager" path="assets/img/P4gm.png" title="generated ground motions" class="img-fluid" width="100%" %}
    </div>
</div>
<div class="caption text-center">
    Figure 3. Simulated ground motions in the horizontal east-west (left), north-south (center), and vertical (right) sensor directions at various distances from the epicenter.
</div>

<p>
    By simplifying the process of generating ground motion data, this project contributes to safer geothermal energy extraction and better preparedness for any seismic risks. For more detailed information and additional results, please refer to the studies: {% cite Kumawat2024 %}. All codes associated with this study are available in the GitHub repository <a href="https://github.com/Aditi-Kumawat/WaveSim" target="_blank">WaveSim</a>.  
</p>



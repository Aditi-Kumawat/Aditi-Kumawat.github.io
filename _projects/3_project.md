---
layout: page
title: Green's Function for Continuous Structrue
description: Wavenumber based approach for Fourier analysis
img: assets/img/P3.jpg
importance: 1
category: work
related_publications: true
---
<div class="project-introduction">
    <p>
        Understanding the impact of time-dependent loads caused by track defects is crucial for railway track analysis. Typically, this analysis involves using various numerical and analytical models, many of which rely on Green's function (or the time-domain impulse response function of the rail beam) to determine the dynamic response of the railway track under such loads. Green's function is usually derived from the rail beam's frequency-domain response, known as track receptance, through an inverse Fourier transform. However, this method has some significant drawbacks:
    </p>
    <ul>
        <li>The need to evaluate the frequency-domain solution over a vast range of frequencies, which increases computational costs.</li>
        <li>The difficulty in accurately inverting the frequency-domain solution, often requiring complex numerical techniques.</li>
    </ul>
    <p>
        To address these challenges, we propose a novel and straightforward approach to evaluate Green's function for a conventional continuous, linear track model. This model consists of an infinite Euler-Bernoulli beam supported by a Pasternak-type viscoelastic foundation, offering computational efficiency that can be particularly useful for practicing engineers.
    </p>
    <p>
        Our approach involves first computing the rail beam's response in the time-wavenumber domain using the classical Duhamel integral technique. The Green's function is then obtained by converting this solution into the time-space domain. The process is outlined in the flowchart provided below (<strong>Figure 1</strong>).
    </p>
</div>

<div class="row">
        <div class="col-sm mt-3 mt-md-0 text-center">
            {% include figure.liquid loading="eager" path="assets/img/P3flow.png" title="Evaluation Approach" class="img-fluid" width="60%" %}
        </div>
    </div>
<div class="caption text-center">
    Figure 1. Flow chart showing the steps of the evaluation of the Green's Function using the wavenumber approach. 
 </div>

<p>
    <strong>Figure 2</strong> shows the normalized time-domain Green's function for the viscoelastic track model as a function of time and distance (with the impulse applied at <em>x=0</em> and <em>t=0</em>). The displacements are normalized against the maximum displacement of the rail beam observed within the considered range of time and distance. As distance increases, the time lag before a non-zero displacement is observed also increases, while the displacement magnitude decreases. This time delay is due to the finite phase velocity of flexural waves in the rail beam. Additionally, the deflection curve stretches out as the distance increases, a result of the dispersive nature of flexural wave velocity, where high-frequency waves travel faster than low-frequency waves.
</p>

<div class="row">
    <div class="col-sm mt-3 mt-md-0 text-center">
        {% include figure.liquid loading="eager" path="assets/img/P3gf.png" title="Green's function space-time domain" class="img-fluid" width="60%" %}
    </div>
</div>
<div class="caption text-center">
    Figure 2. Green's function for viscoelastic model at locations, <em>x</em>=(0, 40m).
</div>

<p>
    Unlike conventional methods, this Fourier inversion approach is both numerically stable and computationally efficient. <strong>Figure 3</strong> presents contour plots of the normalized Green's function of the viscoelastic track model. These are shown as a function of wavenumber-time (proposed approach) and frequency-distance (conventional approach), respectively. The yellow portions of the plots in <strong>Figure 3</strong> indicate the dominant wavenumbers and frequencies. In the proposed approach (Figure 3, left), the dominant wavenumber range is small across all considered time instances, and the Green's function decays rapidly with wavenumber, simplifying the transformation to the space-time domain.
</p>

<div class="row d-flex align-items-end">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/P3kvary.png" title="Green's function wavenumber-domain" class="img-fluid" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/P3omgvary.png" title="Green's function frequency-domain" class="img-fluid" %}
    </div>
</div>
<div class="caption">
    Figure 3. Contour plots showing the variation of normalized Green's function of the viscoelastic track model with (left) wavenumber-time and (right) frequency-distance.
</div>

<p>
    For more detailed information and additional results on the use of Green's function, please refer to the studies: {% cite kumawat2019wave %} and {% cite kumawat2021thesis %}.
</p>



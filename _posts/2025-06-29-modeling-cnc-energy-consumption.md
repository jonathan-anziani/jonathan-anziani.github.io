---
title: "G-Code Based Toolpath Simulation for Predicting CNC Energy 
Consumption"
tagline: " "
header:
  overlay_image: /assets/images/Power and specific energy relation.jpg
  actions:
categories:
  - Uncategorized
gallery:
  - url: /assets/images/toolpath generated.jpg
    image_path: /assets/images/toolpath generated.jpg
    alt: "toolpath generated"
gallery2:
  - url: /assets/images/before and after simulation.jpg
    image_path: /assets/images/before and after simulation.jpg
    alt: "before and after mesh"
gallery3:
  -  url: /assets/images/Power and specific energy relation.jpg
     image_path: /assets/images/Power and specific energy relation.jpg
     alt: "power and sec relation"
gallery4:
  -  url: /assets/images/Power and specific energy relation.jpg
     image_path: /assets/images/Power and specific energy relation.jpg
     alt: "Machined components in titanium"
gallery5:
  -  url: /assets/images/al all.png
     image_path: /assets/images/al all.png
     alt: "Aluminum Power Breakdown graphs"
gallery6:
  -  url: /assets/images/ti all.png
     image_path: /assets/images/ti all.png
     alt: "Titanium Power Breakdown graphs"
gallery7:
  -  url: /assets/images/cumulative energy.png
     image_path: /assets/images/cumulative energy.png
     alt: "Energy vs time graphs"
---

For my undergraduate thesis, I developed a G-code based program in MATLAB that simulates the material removal process and predicts the energy and power consumption required to CNC machine a part. The simulation was validated by machining a part in both aluminum and titanium, showing an energy prediction error of 2.11% and 3.48% respectively.

{% include gallery id="gallery4" class="full" %}

{% include gallery id="gallery5" class="full" %}

{% include gallery id="gallery6" class="full" %}

{% include gallery id="gallery7" class="full" %}

This program functions by first reconstructing the toolpath from the G-code.

{% include gallery id="gallery" class="full" %}

The simulation then runs a virtual endmill along the toolpath in a voxel mesh of the workpiece, replicating material removal.

{% include gallery id="gallery2" class="full" %}

The model predicts the power and specific energy consumption for a timestep by relating it to the simulated material removal rate and spindle speed using existing analytical models and machine-dependant power data. An example relation is shown below.

{% include gallery id="gallery3" class="full" %}

The full thesis with comparisons and sensitivity analyses can be found [here.](/assets/files/anziani-anzianij-bs-meche-2025-thesis.pdf)




---
title: "G-Code Based Toolpath Simulation for Predicting CNC Energy 
Consumption"
tagline: " "
header:
  overlay_image: /assets/images/Power and specific energy relation.jpg
  caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
  actions:
categories:
  - Uncategorized
tags:
  - image
last_modified_at: 2018-03-20T16:00:52-04:00
gallery:
  - url: /assets/images/toolpath generated.jpg
     image_path: /assets/images/toolpath generated.jpg
     alt:"toolpath generated"
gallery2:
  - url: /assets/images/before and after simulation.jpg
    image_path: /assets/images/before and after simulation.jpg
    alt: "before and after mesh"
gallery3:
  - url: /assets/images/Power and specific energy relation.jpg
    image_path: /assets/images/Power and specific energy relation.jpg
    alt: "power and sec relation"


    
---

For my undergraduate thesis, I developed a G-code based program in MATLAB that simulates the material removal process and predicts the energy and power consumption required to machine a part. When analyzing a constant material removal rate milling operation, the average power and specific energy consumption prediction accuracy were shown to be 96.83% and 97.02% respectively.

This program functions by first reconstructing the toolpath from the G-code.

{% include gallery id="gallery" class="full" %}

The simulation then runs a virtual endmill along the toolpath in a voxel mesh of the workpiece, replicating material removal.

{% include gallery id="gallery2" class="full" %}

The model predicts the power and specific energy consumption for a timestep by relating it to the simulated material removal rate and spindle speed using existing analytical models and machine-dependant power data. An example relation is shown below.

{% include gallery id="gallery3" class="full" %}

The full thesis with comparisons and sensitivity analyses can be found [here.](/assets/files/anziani-anzianij-bs-meche-2025-thesis.pdf)




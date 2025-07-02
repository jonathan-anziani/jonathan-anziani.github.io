---
title: "G-Code Based Toolpath Simulation for Predicting CNC Energy 
Consumption "
tagline: " "
header:
  overlay_image: /assets/images/Foot_Dorsiflexed_2985W.jpg
  caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
  actions:
categories:
  - Uncategorized
tags:
  - image
last_modified_at: 2018-03-20T16:00:52-04:00
---

For my undergraduate thesis, I developed a G-code based program in MATLAB that simulates the material removal process and predicts the energy and power consumption required to machine a part. When analyzing a constant material removal rate milling operation, the average power prediction accuracy was shown to be 96.83%.

This program functions by first reconstructing the toolpath from the G-code.

![mount]({{ "/assets/images/mm-header-overlay-black-filter.jpg" | relative_url }})

The simulation then runs a virtual endmill along the toolpath in a voxel mesh of the workpiece, replicating material removal.

![mount]({{ "/assets/images/mm-header-overlay-black-filter.jpg" | relative_url }})

The model predicts the power consumption for a timestep by relating it to the simulated material removal rate and spindle speed using existing analytical models and machine-dependant power data. An example relation is shown below.

![mount]({{ "/assets/images/mm-header-overlay-black-filter.jpg" | relative_url }})

The full thesis with comparisons and sensitivity analyses can be found [here.](/assets/images/mm-header-overlay-black-filter.jpg)




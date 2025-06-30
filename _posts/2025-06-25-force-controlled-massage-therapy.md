---
title: "Force-Controlled Massage Therapy"
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

For MIT's Medical Device Design class, I worked in a team of seven to design a force-controlled automated massaging device that measures muscle stiffness in real-time.
![device moving gif]({{ "/assets/images/massage moving.gif" | relative_url }})

The device consists of three key components: a scissor lift-inspired mechanism that applies force onto the limb, a load cell that measures the force applied, and a linear stage that moves the stage along the limb. By measuring the force on the limb and knowing the distance pressed into the muscle, real-time muscle stiffness can be measured. Future iterations of this project will implement closed-loop stiffness feedback control, replicating how a clinician can feel muscle stiffness during a massage.
![massage exploded view]({{ "/assets/images/Massage_Exploded_View.jpg" | relative_url }})

I was primarily responsible for the load analysis of the structure and the power transmission design. For the load analysis, I modeled the yeilding and buckling failure criterion using a spreadsheet to easily tabulate and communicate the calculations to teammates and project mentors. For the power transmission, I calculated the stepper motor torque and speed requirements needed to replicate the motion and force measured from a massage clinician. With these specifications, I chose sufficient stepper motors for the linear stage and scissor lift and desgned a mounting part to integrate the motors into the rest of the system while preventing a structural collapse when reaching holding torque.

![spreadsheet]({{ "/assets/images/mm-header-overlay-black-filter.jpg" | relative_url }})

More detailed design and testing for this device can be read here.




## Overlay filter

You can use it by specifying the opacity (between 0 and 1) of a black overlay like so:

![transparent black overlay]({{ "/assets/images/mm-header-overlay-black-filter.jpg" | relative_url }})


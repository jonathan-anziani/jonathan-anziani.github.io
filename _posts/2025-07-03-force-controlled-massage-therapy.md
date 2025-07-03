---
title: "Force-Controlled Massage Therapy"
tagline: " "
header:
  overlay_image: /assets/images/Massage.jpg
  actions:
categories:
  - Uncategorized
gallery:
  - url: /assets/images/massage moving.gif
    image_path: /assets/images/massage moving.gif
    alt: "device moving gif"
gallery2:
  - url: /assets/images/Massage_Exploded_View.jpg
    image_path: /assets/images/Massage_Exploded_View.jpg
    alt: "exploded"
  - url: /assets/images/Massage.jpg
    image_path: /assets/images/Massage.jpg
    alt: "close"
gallery3:
  - url: /assets/images/Sample Spreadsheet.jpg
    image_path: /assets/images/Sample Spreadsheet.jpg
    alt: "spreadsheet"
---

For MIT's Medical Device Design class, I worked in a team of seven to design a force-controlled automated massaging device that measures muscle stiffness in real-time.

{% include gallery id="gallery" class="full" %}

The device consists of three key components: a scissor lift-inspired mechanism that applies force onto the limb, a load cell that measures the force applied, and a linear stage that moves the stage along the limb. By measuring the force on the limb and knowing the distance pressed into the muscle, real-time muscle stiffness can be measured. Future iterations of this project will implement closed-loop stiffness feedback control, replicating how a clinician can feel muscle stiffness during a massage.

{% include gallery id="gallery2" class="full" %}

I was primarily responsible for the load analysis of the structure and the power transmission design. For the load analysis, I modeled the yeilding and buckling failure criterion using a spreadsheet to easily tabulate and communicate the calculations to teammates and project mentors. For the power transmission, I calculated the stepper motor torque and speed requirements needed to replicate the motion and force measured from a massage clinician. With these specifications, I chose sufficient stepper motors for the linear stage and scissor lift and desgned a mounting part to integrate the motors into the rest of the system while preventing a structural collapse when reaching holding torque. A sample of these calculations are shown below.

{% include gallery id="gallery3" class="full" %}





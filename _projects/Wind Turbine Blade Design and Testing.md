---
layout: project
title: Wind Turbine Blade Design and Testing
description: MAE 4272: Fluids and Heat Transfer Laboratory
image: /assets/images/radio-machine-cad.jpg
---

As part of MAE 4272, our team designed, fabricated, and experimentally tested a three-blade wind turbine intended to maximize power extraction at a specified operating RPM under realistic wind conditions. The design target was informed by a Weibull probability distribution of free-stream wind speeds, reflecting how wind energy systems operate in practice rather than at a single idealized velocity. In addition to aerodynamic performance, the blade was required to meet strict geometric, RPM, and structural stress constraints to ensure safe operation in a wind tunnel environment.

Our design combined aerodynamic modeling, structural analysis, and CAD-driven fabrication. We selected a NACA 7412 airfoil and implemented a variable chord and twist distribution along the blade span to balance torque generation and structural loading. Using blade element–style calculations, we modeled effective flow velocity, lift and drag forces, torque production, and bending stress as functions of radius. These calculations guided iterative decisions on pitch angle, chord length, and operating RPM to remain within stress limits while targeting maximum power output. The final blade geometry was generated in CAD using discrete spanwise sections and manufactured to interface with the provided turbine hub.

The completed blades were tested in a wind tunnel across a range of free-stream velocities by applying controlled torque loading and measuring rotational speed and power output. Power curves were generated for multiple wind speeds, allowing us to identify the true operating RPM that maximized power under the most probable wind conditions. Experimentally, the turbine achieved a peak power output of 0.04 W at an operating speed of approximately 590 RPM and remained structurally intact at wind speeds up to 12.2 m/s. While performance was lower than predicted, testing revealed that the discrepancy was largely due to blade twist orientation relative to the incoming flow, highlighting the importance of validating design assumptions experimentally.

I worked on the aerodynamic modeling and performance analysis portions of the project, including calculating lift, drag, torque, and bending stress distributions along the blade span. I also contributed to interpreting wind tunnel data, generating power curves, and comparing experimental results against model predictions to diagnose sources of performance loss.

![Chord and Pitch Functions for U = 4.4m/s, 1800 RPM]({{ "/assets/images/Functions.png" | relative_url }}){: .inline-image-r style="width: 200px"}

![Blade CAD, Left: Sketches and Guiding CurveCenter: View from Blade Tip, Right: View from Blade Hub]({{ "/assets/images/CAD.png" | relative_url }}){: .inline-image-r style="width: 200px"}

![Power Curves for Likely U Range from Weibull and Power Curves up to U = 12.2 m/s]({{ "/assets/images/Weiball.png" | relative_url }}){: .inline-image-r style="width: 200px"}

---
layout: project
title: MAE 4272 Wind Turbine Blade Design <!---->
description: Advanced CAD Project
technologies: [Autodesk Fusion]
image: /assets/images/windturbine.gif
permalink: /projects/2025-wind-turbine-blade-design/
---

For this project, we were tasked with designing and experimentally validating a small-scale horizontal-axis wind turbine blade in an open wind tunnel. Our primary objective was to maximize the weighted average power output across the given Weibull probability distribution of wind speed, with optimal performance targeted near our design rotation rate of 1600 RPM to maintain a factor of safety below the maximum 2000 RPM design constraint. We also needed to ensure our design complied with the torque brake’s rotation rate and torque limits, ensure the blades would not structurally fail, and the blades needed to be compatible with the Big Blue wind tunnel test infrastructure. 
To design our blade geometry, we used a combined aerodynamic and structural design optimization framework, developed using Blade Element Theory, stress analysis, and the probabilistic power. Our design process used a parametric optimization of blade pitch, chord, twist, and taper, where each design was evaluated across the given range of wind speeds. We quantified each design’s performance using the expected (probability-weighted) power output from the Weibull distribution, and ensured structural feasibility for each design using bending stress calculations. The final design satisfied all of our constraints in simulation, including maximum rotation rate, torque brake capacity, and material strength limits for the Accura 25 printed blades.

![Photo of Blade CAD]({{ "/assets/images/blade-image.png" | relative_url }}){: .inline-image-l}

We conducted experimental testing to generate power curves at constant wind speeds, using a torque brake to measure the wind turbine blades performance. We collected data by increasing the torque brake voltage until stall at each wind speed. Then we post-processed the data to construct power curves at constant wind turbine blade rotation rates. This approach enabled us to evaluate whether our design rotation rate was optimal under the wind speed distribution while also allowing us to collect data most efficiently with the Big Blue wind tunnel setup.
Though our blade met all safety, structural, and experimental constraints, its performance fell significantly short of our theoretical predictions. Our model predicted a weighted average power output of 1.73 W and a weighted average torque of 1.70 N·cm, whereas our experimental results yielded only 0.0305 W and 0.0568 N·cm, respectively.

![Results Photo]({{ "/assets/images/results-blade.png" | relative_url }}){: .inline-image-r style="width: 200px"}

 Our experimental results are more than an order of magnitude lower than what we predicted, which we believe was caused by a 90° root pitch orientation mistake when we created a CAD model from our design model’s geometry output. This severely degraded the blade’s aerodynamic efficiency. But despite the blade’s performance shortfalls, the blades operated safely and  allowed us to collect usable data. Overall, the project achieved its educational and experimental objectives, providing clear insights into both wind turbine blade design and the practical challenges of translating theory into hardware.


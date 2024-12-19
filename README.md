# Dye in Stream Monitoring: Environmental Analysis Strategy
## Background

The dye tracer monitoring system has controllable injection and measurement capabilities. When deployed in rivers, environmental monitoring operators can optimize measurement strategies for accuracy. Under the constraints of individual monitoring station optimization and the need for comprehensive river system modeling, given the limitations of equipment costs and sampling frequency restrictions, we can propose a new method based on the principles of advection-diffusion and photochemical decay patterns.

# My Work

In this project, we established a comprehensive mathematical model with the goal of optimizing downstream dye detection in river monitoring systems. The model incorporates the key physics of advection-diffusion transport, photochemical decay rates, measurement constraints, and environmental conditions. We developed both analytical and numerical solutions using Forward Euler methods with finite differences to realize accurate dye transport prediction and monitoring optimization.

In the USGS Monocacy River validation tests, the model successfully predicted dye concentration patterns under real-world conditions. The simulation demonstrated the effects of:
- Advective transport at 0.5 m/s flow velocity
- Diffusive spreading with coefficient 0.1 m²/s
- Photochemical decay rates up to 5×10⁻⁴ s⁻¹
- Detection thresholds of 10⁻⁵ g/m

In comparative analysis testing different numerical methods and model dimensions, our Forward Euler implementation showed clear advantages in computational efficiency and accuracy. The 2D model extension revealed that decay effects vary significantly with depth due to UV attenuation, providing more realistic predictions than simple 1D approaches.

Through validation against historical monitoring data, the model proved capable of:
- Predicting optimal sampling frequencies (10-15s intervals at 1km)
- Determining effective measurement station placement
- Estimating detection windows for various decay rates
- Accounting for depth-dependent photodegradation

Since the 1D model has limitations in capturing complex river geometries and flow patterns, we extended to a 2D framework incorporating depth-dependent decay. Further work could focus on 3D modeling using advanced numerical methods and including additional environmental factors. 


# File Description

## Core Implementation (Jupyter Notebook)
- `Dye in a Stream.ipynb`: Main simulation and analysis notebook
- Complete 1D and 2D model implementations
- Model validation with USGS data
- Visualization and analysis tools
- Parameter optimization studies


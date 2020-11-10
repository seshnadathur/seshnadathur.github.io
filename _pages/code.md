---
permalink: /code/
title: "Code"
excerpt: "Data and code"
author_profile: true
---

Much of my code is publicly available on [GitHub](https://github.com/seshnadathur), and is mostly written in Python or Python-wrapped C/C++.

Some particularly useful repositories:

[Revolver](https://github.com/seshnadathur/Revolver)
------
A tool for finding voids in a discrete set of tracer positions. Can be used for galaxies with sky coordinates 
```(RA, dec, z)``` in survey data, or for mock galaxies/halos/dark matter particles with Cartesian coordinates in 
simulation boxes. Includes step to recover approximate real-space positions from redshift-space input by applying 
Zel'dovich reconstruction using iterative FFT method (optional). Can also be used for BAO reconstruction.

[Victor](https://github.com/seshnadathur/victor)
-----
Python code for modelling the void-galaxy correlation function and exploring the likelihoods for cosmological fits to 
data.

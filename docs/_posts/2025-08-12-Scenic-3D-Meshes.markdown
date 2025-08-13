---
layout: post
title:  "Research Project: Extending Scenic to Generate Three-Dimensional Meshes of Road Networks"
date:   2025-08-12 13:09:12 -0700
categories: Scenic Meshes
---

CARLA Town05             |  Scenic Town05 (My Version)
:-------------------------:|:-------------------------:
![Carla Town05](/docs/assets/CARLA_Town05.png)  |  ![Scenic Town05](/docs/assets/Scenic_Town05.png)

## Links

Github Repository: [Github Repository][github-repo]

Research Paper: [Paper][paper]
 
Capstone Presentation: [Presentation][presentation]


## Intro

Scenic is a probabilistic programming language designed to create and evaluate scenarios for perception systems in autonomous vehicles and other cyber-physical platforms, such as robotics. It generates “scenes” composed of objects and agents, allowing users to repeatedly simulate diverse environments. By producing numerous variations, including rare or edge cases, Scenic supports machine learning workflows, helps identify potential failure modes, and enables rigorous testing and validation of perception-driven systems.

Previously, Scenic supported only two-dimensional polygonal map representations, preventing accurate modeling of three-dimensional road features such as ramps, bridges, hilly roads, and tunnels. To address this limitation, I have been working to extend Scenic’s codebase to parse three-dimensional elements and generate corresponding 3D meshes.

In this project, I have completed the following:
- Modify the calculations in the parser file to account for three dimensions
- Use three-dimensional meshes from the Trimesh library in place of polygons
- Modify the Road objects to include new geometries
- Create three-dimensional visualizations of the road map scenarios
- Support both 2D and 3D compatibility with command line options

This project was done as part of a Capstone Requirement as part of my Master's Program for Computer Science in Spring 2025. 

I am still improving on this project and have compiled a list of tasks/improvements that I am currently working on.
- Testing functionality with CARLA driving simulator
- Fixing orientation of objects
- Optimizing calculations of road network

TODO:
- Add Pictures
- Add Link to Github
- Add Link to Paper
- Add Link to Presentation

[github-repo]: https://github.com/BerkeleyLearnVerify/Scenic/tree/3d-driving
[paper]: https://drive.google.com/file/d/1heSntBwkX-YIAxuAPf8Bvj73L73NmwS3/view?usp=sharing
[presentation]: https://drive.google.com/file/d/1DkTVb16uYtd1eQdSoJ52yy_plOK3Svzt/view?usp=sharing
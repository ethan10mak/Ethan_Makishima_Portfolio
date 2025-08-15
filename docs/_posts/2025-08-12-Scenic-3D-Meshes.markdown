---
layout: post
title:  "Research Project: Extending Scenic to Generate Three-Dimensional Meshes of Road Networks"
date:   2025-08-12 13:09:12 -0700
categories: Scenic Meshes
---

CARLA Town05             |  Scenic Town05 (My Version)
:-------------------------:|:-------------------------:
![Carla Town05]({{site.baseurl}}/assets/Capstone/CARLA_Town05.png)  |  ![Scenic Town05]({{site.baseurl}}/assets/Capstone/Scenic_Town05.png)
**Left:** [CARLA's][carla] generation of the map from parsing the OpenDrive file.
**Right:** [Scenic's][scenic]/my generation of the map from parsing of the same OpenDrive file.

## About

[Scenic][scenic] is a probabilistic programming language designed to create and evaluate scenarios for perception systems in autonomous vehicles and other cyber-physical platforms, such as robotics. It generates “scenes” composed of objects and agents, allowing users to repeatedly simulate diverse environments. By producing numerous variations, including rare or edge cases, Scenic supports machine learning workflows, helps identify potential failure modes, and enables rigorous testing and validation of perception-driven systems.

Previously, Scenic supported only two-dimensional polygonal map representations, preventing accurate modeling of three-dimensional road features such as ramps, bridges, hilly roads, and tunnels. To address this limitation, I have been working to extend Scenic’s codebase to parse three-dimensional elements and generate corresponding 3D meshes.

In this project, I have done the following:
- Enhanced [OpenDrive][opendrive] file parser to seamlessly integrate elevation data, enabling more realistic road network representations.
- Upgraded parsing algorithms to handle full 3D spatial calculations, improving simulation accuracy.
- Integrated Trimesh 3D meshes in place of traditional polygons, boosting visualization fidelity.
- Extended Road object architecture to support advanced 3D geometries.
- Developed immersive 3D visualizations for complex road map scenarios, aiding debugging and presentation.
- Built dual-mode support for 2D and 3D simulation with flexible command-line configuration.
- This project was done as part of a Capstone Requirement as part of my Master's Program for Computer Science in Spring 2025. 

I am still improving on this project and have compiled a list of tasks/improvements that I am currently working on.
- Testing functionality with [CARLA][carla] driving simulator
- Fixing orientation of objects
- Optimizing calculations of road network

<!-- TODO: Add design process?-->

## Resources/Links:

Github Repository: [Github Repository][github-repo]
Research Paper: [Paper][paper]
Capstone Presentation: [Presentation][presentation]

Scenic's Homepage: [Scenic][scenic]
Scenic's Documentation: [Documentation][scenic_documentation]
Carla's Homepage: [CARLA][carla]
ASAM OpenDrive's Documentation: [ASAM OpenDrive][opendrive]

[github-repo]: https://github.com/BerkeleyLearnVerify/Scenic/tree/3d-driving
[paper]: https://drive.google.com/file/d/1heSntBwkX-YIAxuAPf8Bvj73L73NmwS3/view?usp=sharing
[presentation]: https://drive.google.com/file/d/1DkTVb16uYtd1eQdSoJ52yy_plOK3Svzt/view?usp=sharing
[scenic]: https://scenic-lang.org/
[scenic_documentation]: https://docs.scenic-lang.org/en/latest/
[carla]: https://carla.org/
[opendrive]: https://www.asam.net/standards/detail/opendrive/
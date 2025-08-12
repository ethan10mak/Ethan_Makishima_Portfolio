---
layout: post
title:  "Research Project: Extending Scenic to Generate Three-Dimensional Meshes of Road Networks"
date:   2025-08-12 13:09:12 -0700
categories: Scenic Meshes
---
Scenic is a probabilistic programming language designed to create and evaluate scenarios for perception systems in autonomous vehicles and other cyber-physical platforms, such as robotics. It generates “scenes” composed of objects and agents, allowing users to repeatedly simulate diverse environments. By producing numerous variations, including rare or edge cases, Scenic supports machine learning workflows, helps identify potential failure modes, and enables rigorous testing and validation of perception-driven systems.

Currently, Scenic supports only two-dimensional polygonal map representations, preventing accurate modeling of three-dimensional road features such as ramps, bridges, hilly roads, and tunnels. To address this limitation, I have been working to extend Scenic’s codebase to parse three-dimensional elements and generate corresponding 3D meshes.

In this project, I have completed the following:
- Modify the calculations in the parser file
- Build meshes instead of polygons
- Modify the Road objects to include new geometries
- Create three-dimensional visualizations of the road map scenarios

This project was done as part of a Capstone Requirement as part of my Master's Program for Computer Science in Spring 2025. 

I am still improving on this project and have compiled a list of tasks/improvements that I am currently working on.
- Testing functionality with CARLA driving simulator
- Fixing orientation of objects
- Optimizing calculations of road network
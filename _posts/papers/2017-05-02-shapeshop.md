---
layout: paper
categories: papers
permalink: papers/shapeshop
id: frontier
title: "Predicting Situations with Loop Closures in Frontier Based Robotic Exploration"
authors:
    - Etash Guha
    - Patricio Vela
venue: "National Conference of Undergraduate Research"
venue-shorthand: NCUR
location: Atlanta, GA, USA
year: 2019
icon: shapeshop.png
tagline: Understanding Deep Learning Representations via Interactive Experimentation
feature-title: "Robotic Exploration"
feature-description: "Robotic Exploration"
poster: /papers/NCURPOSTER.pdf
pdf: /papers/NCURPOSTER.pdf
collaboration: PNNL
type: poster
featured: true
selected: true
image: images/featured/ego_3d.png
feature-order: 3
---

The objective of this research project is to develop a method of predicting loop closures within Frontier Based Exploration, to improve the accuracy and time to which a robot can create a map of its surrounding area. Frontier Based Exploration (FBE) is when robots are deployed to map an unknown environment. It involves analyzing and moving to unknown “frontiers” of the explored region, using several factors to judge each frontier. These factors balance the exploitation of known information versus exploration of the unknown. One major means to reduce map uncertainty is through the generation of loop closures. However, many frontier based navigation algorithms forgo the use of loop closures as a factor due to the difficulty of modeling loop-closure. This work proposes implementing a method of using loop closures by analyzing the odometry drift, spatial surroundings, and robotic vision of simulated FBE scenarios to create a predictive model to be integrated with FBE. We will use ROS packages to code the movement algorithms for the robot and Rviz and Gazebo to simulate the movement, using C++ and Python. The simulated environment will be used to generate visual loop closures and provide the data needed for a data-driven model of loop-closure likelihood to then be incorporated as an FBE factor. We will then compare the new loop-closure informed FBE with a traditional FBE model. We will use accuracy and completeness to evaluate the map created by using and not using loop closures prediction. We hypothesize that this implementation will result in a frontier-based algorithm that creates a more complete map than would with standard techniques. These results will give information about several new possible avenues for predicting loop closures to optimize robotic exploration, an important field that improves areas such as driverless cars or rescue missions.  
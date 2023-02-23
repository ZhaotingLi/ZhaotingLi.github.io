---
layout: research_example
image: /img/contact-aware-control-demo.png
---


### CARE: Contact Aware and Reactive Estimator for Contact-Rich Motion Planning
Advisor: Prof. Dr. Stelian Coros, Computational Robotics Lab, ETH Zurich



Contact-rich tasks require the robot to make necessary contacts with the environment. 
One example is the stowing task at the Amazon factory, where elastic bands are mounted on the cabinet to prevent objects from falling out.
In this case, contacts with elastic bands are inevitable during package stowing.
For robot arms equipped with the torque-sensing capabilities, the contact detection algorithm can estimate the contact point location and contact force. 
Furthermore, the contact information can be utilized for estimating the model of the environment and for planning with safety constraints. 
The goal of this project is to explore ways to robustly detect external contacts, utilize contact information, and trajectory planning to enable smooth and safe contact-rich tasks.

## 1. Contact point detection

When the robot has physical contact with the environment, the observed external torque data in the joints can be utilized to estimate the contact locations and forces.
One typical method is the contact particle filter, which designs a particle filter to find the contact point on the robot's surface. 
However, due to the singularity of the robot and the noise of the external torque data, there can be multiple possible solutions for one external contact situation. 
To solve this problem, we propose a clustered contact particle filter, which can find the set of possible solutions and the corresponding possibilities. 

<iframe width="560" height="315" src="https://www.youtube.com/embed/VXqhTi8C144" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## 2. Contact-aware control

Usually, the robot arm only interacts with the environment with its end-effector, while trying to avoid the obstacles to keep safe. 
However, in cluttered environments, contacts with the surrounding objects are inevitable. 
To remain safe, nullspace control schemes can be adopted to keep the contact force to a desired value, while trying to track the reference trajectory.
However, the simple nullspace control scheme fails to consider the inequality constraints, which can lead to large jerks or large deviations from the reference trajectory.
To solve this problem, we propose an optimization-based framework, which can handle both soft and hard contacts. 

<iframe width="560" height="315" src="https://www.youtube.com/embed/gkBA3sUJjAI" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


## 3. Contact-aware planning

This section is still under research. 

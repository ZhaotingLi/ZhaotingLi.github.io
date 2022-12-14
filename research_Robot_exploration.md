---
layout: research_example
image: /img/robot_expo_comparision_result2.png
---


### Learning Robot Exploration Strategy with Deep Reinforcement Learning
* Advisor: Max Q.-H. Meng , IEEE Fellow and Professor in Department of Electrical and Electronic Engineering, SUSTech

Being able to explore unknown environments is a requirement for fully autonomous robots. Many learning-based methods have been proposed to learn an exploration strategy. In the frontier-based exploration, learning algorithms tend to learn the optimal or near-optimal frontier to explore. Most of these methods represent the environments as fixed size images and take these as inputs to neural networks. However, the size of environments is usually unknown, which makes these methods fail to generalize to real world scenarios. To address this issue, we present a **novel state representation** method based on 4D point-clouds-like information, including the locations, frontier, and distance information. We also design a neural network that can process these 4D point-clouds-like information and generate the estimated value for each frontier. Then this neural network is trained using the typical reinforcement learning framework. We test the performance of our proposed method by comparing it with other five methods and test its scalability on maps that are much larger than maps in the training set. The experiment results demonstrate that our proposed method needs shorter average traveling distances to explore whole environments and can be adopted in maps with arbitrarily sizes.



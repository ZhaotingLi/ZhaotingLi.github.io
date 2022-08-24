---
layout: research_example
image: /img/DLAD_overview.png
---


### Deep Learning for Autonomous Driving: muti-tasking learning and 3D object detection

In the course *Deep Learning for Autonomous Driving* at ETH Zurich, two projects are finishded including (1) multi-tasking learning for semantics segmentation and depth estimation (2) 3D object detection from Lidar Point clouds. Here are the details.

#### Multi-tasking learning for semantics segmentation and depth estimation

In this project, we explore the effectiveness of different Muti-Task Learning architectures for semantic segmentation and monocular depth estimation.
For better performance and to increase the resolution of the predicted results, the ASPP module is also implemented. We also proposed an **adaptive weight tuning method** which can adaptively adjust the weight of each task to prioritize difficult tasks first.

#### 3D object detection from Lidar Point clouds

3D object detection is crucial for autonomous driving, where the most frequently used 3D sensor are the LiDAR sensors. 
The typical commonly-used 2-stage framework is composed of two networks: the Region Proposal Network (RPN) and the proposal refining network.
In this report, we propose several methods to improve the network performance:
(1) Include the local coordinate and intensity information as features.
(2) Using Adam as optimizer instead of SGD.
(3) Adding IoU loss for the regression task.
(4) Changing the bounding box enlargement strategy for roi pooling step.



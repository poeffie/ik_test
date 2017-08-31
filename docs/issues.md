# Limit of KDL Solver
The ROS MoveIt! KDL solver is only suitable for use with >= 6DoF kinematic chains. This is an issue that normally would make IK on the PaBiLegs impossible, as this model only has 2DoF.

To overcome these limitations, MoveIt! allows to use another solver, the so called IKFast solver, which is capable of solving IK equations, no matter what the DoF of the kinematic chain. It even needs less time for the same problem as KDL. IKFast is developed by [OpenRave](http://openrave.org/docs/0.8.2/openravepy/ikfast/)

# Install Openrave
OpenRave for Ubuntu 16.04 Xenial can be downloaded as a robotic workstation by following this [tutorial](https://fsuarez6.github.io/blog/workstation-setup-xenial/). Unfortunately many compiling errors occured during all of my attempts. Using the workstation with a graphical visualization by OpenSceneGraph, as it is described in the tutorial may be not necessary for this project, as ROS MoveIt! offers an own solution...

# Create IKFast Plugin
...

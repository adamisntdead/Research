# Fido: A Universal Robot Control System using Reinforcement Learning with Limited Feedback

This document is a summary. For a more detailed look at our research, [here is a link to our paper](http://mntruell.com/pdf/Fido_Paper.pdf).

A robot control system that learns from humans **four times faster** than the current industry standard. Researched and built by [Josh Gruenstein](https://github.com/joshuagruenstein "@joshuagruenstein") and [Michael Truell](https://github.com/truell20 "@truell20").

## Abstract

A robot control system was developed that could be taught tasks through reinforcement learning. The system, nicknamed “Fido”, was designed to be universal regardless of inputs and outputs, robot kinematics, and processing capability.   In addition, Fido was built to learn with limited feedback, allowing humans to train Fido in a minimal amount of time. This was achieved through the training of artificial neural networks with a wire-fitted interpolator following the Q-learning reinforcement learning algorithm and an intelligent action selection policy that utilizes a probabilistic approach to exploration.  Functionality was first tested and evaluated in simulation.  Next, hardware implementations of differing kinematics, sensors, and central processors were constructed.  Fido successfully converged on all given tasks in simulation and in hardware within very few learning iterations while maintaining impressively low latency, demonstrating its potential as a comprehensive robot control system.

## Project Summary

Robotic intelligence can be simplified to a black box, with inputs such as sensor data and outputs such as motor control.  Most robotic software today operates as an "expert system," using preprogrammed logic to execute a set routine.  These implementations are sufficient for the specific purpose and platform that they are designed for but lack the ability to perform other tasks or work on other robots.

The purpose of this project was to develop a universal robot control system that does not require preprogrammed logic to accomplish specific tasks, can be adapted to any robot hardware, and can be trained in a short amount of time using positive and negative reinforcement.  The control system we developed (nicknamed Fido) is lightweight and resource-efficient, making it a practical solution for mobile robots.  This was achieved by employing an artificial neural network and a novel learning algorithm.  The algorithm takes a well-tested learning algorithm called Q-learning and modifies it to be better suited for robotic tasks.

Fido was tested on a computer simulated robot with a motor control system, a large sensor array, and some additional outputs.  The system performed well doing a variety of tasks, such as learning to drive to a radio beacon and following a line.  Two hardware implementations were also created for additional testing.  These implementations used low cost and low power embedded GNU/Linux systems to run the Fido software, and were successfully trained to perform complex tasks such as line following, learning a kiwi holonomic drive system, following a ball, and adapting to mechanical failures.

Further details can be found in the [research paper](http://mntruell.com/pdf/Fido_Paper.pdf) and [poster](http://mntruell.com/pdf/Fido_Poster.pdf).

## Awards

In 2016, Fido advanced to the finals of the New York City Science and Engineering Fair.  There it won the Intel Excellence in Computer Science award, placed first in the Computer Science category, and was selected to represent NYC at the Intel International Science and Engineering Fair (ISEF). At ISEF, Fido won the second place NASA award, a visit to CERN, and second place in its category (Robotics and Intelligent Machines).

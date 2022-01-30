# Continuous Control

## Project Goal

The goal is to train an agent to maintain the double-jointed arm at a moving target location as long as possible.

![In Project 2, Continuous Control](resources/reacher.gif)

## Environment Details

The environment is based on [Unity ML-agents](https://github.com/Unity-Technologies/ml-agents).

In this environment, a double-jointed arm can move to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of your agent is to maintain its position at the target location for as many time steps as possible.
The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

## Getting Started:

#### 1. Clone this Github repository:
```bash
git clone https://github.com/SagarRathod-TomTom/Continuous-Control-Deep-Refinforcement-Learning-Udacity-Nanodegree.git
```

#### 2. Setup Python:
Follow this [link](https://github.com/udacity/deep-reinforcement-learning#dependencies) to setup your environment for traning an agent on your local machine.

#### 3. Download the Unity Environment:

For this project, you will not need to install Unity - this is because we have already built the environment for you, and you can download it from one of the links below. You need only select the environment that matches your operating system:

* Version 1: One (1) Agent
    * Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux.zip)
    * Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher.app.zip)
    * Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86.zip)
    * Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86_64.zip)


* Version 2: Twenty (20) Agents
    * Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux.zip)
    * Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher.app.zip)
    * Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86.zip)
    * Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86_64.zip)

Then, place the file in the unity_environment/ folder after you clone this GitHub repository, and unzip (or decompress) the file.
(For Windows users) Check out this link if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

The second version is useful for algorithms like PPO, A3C, and D4PG that use multiple (non-interacting, parallel) copies of the same agent to distribute the task of gathering experience.


#### 3. Continuous Control Jupyter Notebook:

Executes the code cells in the provided [notebook](Continuous_Control.ipynb).


## Implementation Details:

This repository contains the implementation of DDPG to solve the second version of the environment of Twenty(20) Agents.
Checkout [Report.md](Report.md) for in-depth implementation details.
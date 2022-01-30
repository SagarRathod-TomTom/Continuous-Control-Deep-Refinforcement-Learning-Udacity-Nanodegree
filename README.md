# Navigation

## Project Goal

The goal is to train an agent to maintain the double-jointed arm at a moving target location as long as possible.

![In Project 2, Continuous Control](resources/reacher.gif)

## Environment Details

The environment is based on [Unity ML-agents](https://github.com/Unity-Technologies/ml-agents).

In this environment, a double-jointed arm can move to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of your agent is to maintain its position at the target location for as many time steps as possible.
The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

## Getting Started:

### Clone this Github repository:
```
git clone 
```

### Download the Unity Environment

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
(For AWS) If you'd like to train the agent on AWS (and have not enabled a virtual screen), then please use this link (version 1) or this link (version 2) to obtain the "headless" version of the environment. You will not be able to watch the agent without enabling a virtual screen, but you will be able to train the agent. (To watch the agent, you should follow the instructions to enable a virtual screen, and then download the environment for the Linux operating system above.)


## Note

The project environment is similar to, but not identical to the Banana Collector environment on the [Unity ML-Agents GitHub page](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#banana-collector).
For this project, you will not need to install Unity. You can download the environment from one of the links below. 
You need only select the environment that matches your operating system:

* Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
* Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
* Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
* Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)

Once you download the zip file, unzip or decompress it.

## Quick Start

### 1. Install:

#### Prerequisite:
Python 3.6+
    
1. Clone the repository.
```shell
git clone https://github.com/SagarRathod-TomTom/Navigation-Deep-Reinforcement-Learning-Nanodegree.git
```
2. Install dependencies.
```shell
cd Navigation-Deep-Reinforcement-Learning-Nanodegree
pip install -r requirements.txt
```

### 2. Usage:
```shell
python main.py --help
```
##### Parameters:
```shell
usage: main.py --unity_env_path UNITY_ENV_PATH [--batch_size BATCH_SIZE]
               [--gamma GAMMA] [--eps EPS] [--eps_end EPS_END]
               [--eps_decay EPS_DECAY] [--tau TAU] [--lr LR]
               [--update_every UPDATE_EVERY] [--disable-graphics]
               [--seed SEED] [--help] [--version]

Train DQN Agent to solve Banana Unity Environment.

optional arguments:
  --unity_env_path UNITY_ENV_PATH
                        (type:str default:None)
  --batch_size BATCH_SIZE
                        (type:int default:64)
  --gamma GAMMA         (type:float default:0.9)
  --eps EPS             (type:float default:1.0)
  --eps_end EPS_END     (type:float default:0.01)
  --eps_decay EPS_DECAY
                        (type:float default:0.995)
  --tau TAU             (type:float default:0.001)
  --lr LR               (type:float default:0.001)
  --update_every UPDATE_EVERY
                        (type:int default:4)
  --disable-graphics    Set graphics to False
  --seed SEED           (type:int default:42)
  --help                Print Help and Exit
  --version             show program's version number and exit
  
```

### 3. Train agent with default parameters.
```shell
python main.py --unity_env_path path/to/BananaEnv
```
The process terminates when the agent achieves the average score of 13 or more.


## Implementation Details:
Checkout [Report.md](Report.md) for in-depth implementation details.

# Unity Banana collector environment

### Introduction

We provide an implementation of DQN that solves the Unity Banana collector environment.

![Banana solved](Banana.gif)

The set-up is as follows: the agent is on a flat enclosed surface and can move forward, backward, left and right. Bananas spawn and the agent receives a reward of +1 for collecting a yellow banana and -1 for collecting a blue banana. At each timestep, the agent observes 37 dimensional vector information about the agent's velocity along with ray-based perception of objects around the agent's forward direction. At each timestep the agent outputs an action: it moves in one of the four directions.

### Solving the Environment
To solve the environment, the agent must get an average score of +13 over 100 consecutive episodes.

### Solution

We use the [deep Q network](https://www.cs.toronto.edu/~vmnih/docs/dqn.pdf) (DQN) reinforcement learning algorithm to solve the environment.

### Try it yourself!

0. Install anaconda from [here](https://www.anaconda.com/distribution/).

1. Install unity ml-agents using the [instructions](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Installation.md) here.

2. Download the Reacher environment from one of the links below.  You need only select the environment that matches your operating system:

- [Linux](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)

- [Mac OSX](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)

- [Windows (32-bit)](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)

- [Windows (64-bit)](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)


3. Download the Banana_DQN.ipynb notebook from this repository to train the agent. Follow these simple [these instructions](https://stackoverflow.com/questions/45622602/how-to-save-jupyter-notebooks-from-github).

4. Go to the relevant terminal and create a conda environment
```
conda create -n myenv python=3.6
```

5. Activate the environment and open jupyter notebooks
```
conda activate myenv
jupyter notebook
```

Then open up the Banana_DQN notebook and run it.

If you're not on a Mac make sure to change the filename of the environment in the notebook.

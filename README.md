[//]: # (Image References)

[image1]: reacher.png "Trained Agent"

# Project 2: Continuous Control

### Introduction

This project, you we train an agent that have to reache a sphere around it, 

![Trained Agent][image1]

A reward of +0.1 is provided with the agent touch the sphere, the goal of the agent is to maintain 30 points or more  in 100 episodes consecutives

The state space has 33 dimensions , the action spaces is 4 for each agent, and we have 20 agents

### Getting Started

The instruccion 1 is for Windows 10 Users with NVIDIA VideoCards, another S.O. please refer [this link](https://pytorch.org/get-started/locally/) and then  go to the number 2 Instruccion.


### Instructions

1.- NVIDIA CARDS : If you have a Nvidia VidCard you can use Pytorch and train your model faster, follow this intructions for Windows:
	
Install the latest nvidia driver [here](https://www.nvidia.com/es-la/geforce/drivers/)

Install Visual Studio 2019 16x (needed for CUDA) [here](https://visualstudio.microsoft.com/es/downloads/)

Install CUDA Kit [here, and note the version to be 11.0 ](https://docs.nvidia.com/cuda/cuda-installation-guide-microsoft-windows/index.html)

2.- Install AnaConda [here](https://www.anaconda.com/products/individual)

3.- Create a kernel "drlnd" on AnaConda and install pytorch, torchvision with cuda support, gym enviroment, mlagents and unityagents: 

	on your menu on windows , select "Anaconda3" - and then "Anaconda Prompt" it will open a new command window then 
     (For another S.O. please refer  (https://docs.anaconda.com/anaconda/install/verify-install/) ):

	conda create --name drlnd python=3.6

	conda activate drlnd

	conda install -c anaconda ipykernel
	
	python -m ipykernel install --user --name drlnd --display-name "drlnd"

	pip install mlagents

	pip install unityagents --user

	pip install torchvision===0.8.2 -f https://download.pytorch.org/whl/torch_stable.html


4.- Download the github project (git clone https://github.com/pelsan/Continuous-Control.git) and open Continuous_Control.ipynb on Jupyter


5.- Download the environment from one of the links below.  You need only select the environment that matches your operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86_64.zip)
    
    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

    (_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux_NoVis.zip) to obtain the environment.

6-. Place the file in the DRLND GitHub repository, in the `Continuous-Control/` folder, and unzip (or decompress) the file. 


5.- Select drlnd Kernel:

	On Jupyter Menu select "Kernel" - "Change Kernel" - "drlnd"

6.- Run the Notebook `Continuous_Control.ipynb` 

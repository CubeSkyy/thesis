# Critical Review of Reinforcement Learning Based Adaptive Traffic Signal Control

Final versions of my Master's Thesis for my Computer Science degree.

Following are the abstract and contributions, taken from the full thesis.

## Abstract
Adaptive traffic signal control is a performance-critical task in intelligent transportation systems: Through the use of advanced sensors, controllers can respond to actual traffic conditions at intersections and produce policies capable of mitigating bottlenecks and preventing gridlocks. 

Reinforcement learning-based multi-agent systems (MARL) provide a natural framework to address the task. In MARL, each agent controls one intersection and can coordinate with its neighbors to attain an optimal network- wide policy. However, it remains a daunting task to compare approaches as there are many possible compositions. This thesis makes a critical comparison across different traffic controllers found in the literature.

We show that using non-linear approximators, coordination mechanisms and increasing the observability at each intersection are key performance drivers

## Contributions

The major contributions of the current work are to create a stable environment and defined problem
formulation to compare different traffic control strategies.

Specifically, this work aims to:

* Prepare the simulator that will be used to train and evaluate the traffic controllers and create a set of realistic scenarios for them to be tested on. In particular, a 1x3 arterial network and a 3x2 grid network.
* Create an effective Markov Decision Problem (MDP) formulation that allows for a meaningful comparison between the different traffic control methods.
* Develop baseline traffic controllers that will be used to compare with the other reinforcement learning-based controllers, in particular: a random controller, a fixed-time controller, a Webster controller and a Max-pressure controller.
* Develop reinforcement learning-based traffic controllers, in particular: an Actor-Critic (ACAT) model that uses tile coding [9], a Deep Q-Network (DQN) model [12] and three different implementations of the MARLIN algorithm [8], based on Fictitious Play.
* Analyse how do different methods of discretization, coordination and observability affect the base- line and reinforcement learning-based traffic controllers, using a set of evaluations metrics to access the performance of each controller in each of these 3 axis.

# LOG-Nav: Efficient Layout-Aware Object-Goal Navigation with Hierarchical Planning

<p align=“center”> 
<img src=".\figures\teaser.png" width="600"> 
</p>

We introduce **LOG-Navi**, an **Efficient Layout-Aware Object-Goal Navigation** approach designed for **complex multi-room indoor environments**.

By planning hierarchically leveraging a global topology map with layout information and detailed scene representation memory, LOG-Navi achieves both efficient and effective navigation. The process is managed by an LLM-powered agent, ensuring seamless operation from exploration to navigation, without the need for human interaction, complex rewards, or costly training. 

Our experimental results on the HM3D benchmark demonstrate a **16.7\% point improvement in navigation success rate** and **12\% improvement in success rate weighted by path length** compared to SOTA methods. Furthermore, we validate the robustness of our approach through real-world robotic deployment, showcasing its capability in practical scenarios.

## Real-world Experiments

Navigation examples

<img src=".\figures\1.gif" width="480"> 
<img src=".\figures\2.gif" width="480"> 
<img src=".\figures\3.gif" width="480"> 

Obstacle avoidance examples

<img src=".\figures\4.gif" width="480"> 

## Simulated Experiments in HM3D
scene 17DRP5sb8fy

<img src=".\figures\sim_1.gif" width="480"> 

scene 2t7WUuJeko7

<img src=".\figures\sim_2.gif" width="480"> 

scene HxpKQynjfin

<img src=".\figures\sim_3.gif" width="480"> 

RPmzsHmrrY

<img src=".\figures\sim_4.gif" width="480"> 

## Pipeline

The LLM agent takes user instructions as input and manages the optional action choices according to the prompts and data flow. Optional actions include exploring and recording the scene, constructing scene memory representation, planning, and executing navigation. Obstacles and error recognition together with iterative attempts are available.

The main components design is two-fold: **hierarchical planning** based on topo-layout and dense scene memory, **LLM-powered agent** that conducts the process from exploration to exploitation.

<img src=".\figures\method.png"> 

## Primary experiment results

<img src=".\figures\exp_1.png">

<img src=".\figures\exp_1.png">

## Embodiment construction

<img src=".\figures\robotic.png" width="480">

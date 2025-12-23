---
title: "MEng Thesis: Deep Reinforcement Learning Agents"
excerpt: "Explored the training of classical and deep reinforcement learning agents on neuromorphic hardware with biologically plausible algorithms."
header:
  image: /assets/images/A749923C-99EA-44DD-ABE7-88A0EFB8A492_1_201_a.jpeg
  teaser: /assets/images/gamer-6022003_1920_cropped.png
  caption: "Photo credit: [Pixabay](https://pixabay.com)"
permalink: /projects/meng-reinforcement-learning/
# core_discipline: ["AI", "Neuromorphic", "Reinforcement Learning"]
# meta_skill: ["Algorithm Design"]
project_type: "Academic"
toc: true
toc_sticky: true
toc_label: "On This Page"
toc_icon: "fa fa-stream"
author_profile: true
read_time: true
---

<div class="notice--info" markdown="1">
For my first deep learning research project, I explored the training of classical and deep reinforcement learning agents on neuromorphic hardware with biologically plausible algorithms.
</div>

## Situation

Reinforcement learning (RL) has surpassed human performance in complex decision-making AI tasks ([AlphaGo](https://deepmind.google/research/alphago/), [AlphaZero](https://deepmind.google/research/alphazero-and-muzero/), [AlphaFold](https://deepmind.google/science/alphafold/)). However, the standard machine learning training algorithm, backpropagation, is not biologically plausible, making it incompatible [neuromorphic computing](https://www.ibm.com/think/topics/neuromorphic-computing).

## Task

For my Master's, I was tasked with exploring the use of [Direct Feedback Alignment (DFA)](https://arxiv.org/abs/1609.01596) for training classical and deep reinforcement learning agents, comparing their performance to standard backpropagation-trained agents.

<img src="/assets/images/meng1.png" alt="direct-feedback-alignment" class="align-center" style="border-radius: 1%;">

## Action

I structured my research in three phases:

1. Established classical RL algorithms (Q-learning, SARSA) baselines on custom-built games such as Gridworld and Cliff Walker.
2. Engineer lightweight deep RL agents using both backpropagation and DFA, training them on classic control problems from OpenAI Gym such as CartPole, MountainCar, and Acrobot.
3. Expand the deep RL agents to use convolutional neural networks (CNNs) as function approximators, training them on complex Atari game environments from OpenAI Gym, such as Breakout and Seaquest

<img src="/assets/images/meng2.png" alt="deep-reinforcement-learning" class="align-center" style="border-radius: 1%;">

## Result

My work demonstrated that neuromorphic direct feedback alignment training performs similarly to backpropagation across all problems tested.

## Scars

As a self-taught programmer with a background in aeromechanical engineering,
this was my first (very) deep dive into AI research. I made many and learned as many lessons. However, the two key takeaways were:
1. Define the jobs to be done early, and reevaluate them often. This lesson came about
after spending weeks blocked, not knowing how to proceed with an ambiguous task in 
an unfamiliar domain, only to realize, with the help of my supervisor, that small,
incremental steps are better than giant leaps.
2. Test everything, as bugs can crop up in the most unexpected places. I learned
this the hard way after spending days training my final deep RL agents, only
to find that I was not saving the replay memory buffer, leading to the agents
learning almost nothing.

## Interdisciplinary Integration

The project gave me exposure to several topics:
* Neuromorphic computing and associated biologically plausible training algorithms.
* Deep learning architectures such as ANNs and CNNs.
* Reinforcement learning algorithms and environments.

## Technologies & Skills Used

* TensorFlow
* OpenAI Gym
* Reinforcement Learning (Q-Learning, SARSA)
* Direct Feedback Alignment (DFA)
* Data Analysis

## Publications & Resources

* [arXiv Publication](https://arxiv.org/abs/1905.04127)
* [GitHub Repository](https://github.com/AndreiRoibu/DeepReinforcementLearning)
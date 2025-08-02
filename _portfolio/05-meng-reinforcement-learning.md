---
title: "MEng Thesis: Deep Reinforcement Learning Agents"
excerpt: "Validated the feasibility of training deep reinforcement learning agents with biologically plausible algorithms, benchmarking their performance."
header:
  image: /assets/images/A749923C-99EA-44DD-ABE7-88A0EFB8A492_1_201_a.jpeg
  teaser: /assets/images/gamer-6022003_1920_cropped.png
  caption: "Photo credit: [Pixabay](https://pixabay.com)"
permalink: /projects/meng-reinforcement-learning/
core_discipline: ["AI", "Neuromorphic", "Reinforcement Learning"]
meta_skill: ["Algorithm Design"]
project_type: "Academic"
toc: true
toc_sticky: true
toc_label: "On This Page"
toc_icon: "fa fa-stream"
author_profile: true
read_time: true
---

<div class="notice--info" markdown="1">
For my first deep research project in AI, I pioneered an investigation into neuromorphic deep reinforcement learning, demonstrating the feasibility of **biologically plausible agents**.
</div>

## Situation

Reinforcement learning (RL) has achieved superhuman performance in complex decision-making AI tasks (AlphaGo, AlphaZero, AlphaFold). However, the standard training algorithm, backpropagation, is not biologically plausible, making it incompatible with the next generation of brain-inspired **neuromorphic hardware**.

## Task

The core objective of my Master's thesis was to validate the feasibility of a biologically plausible training algorithm, **Direct Feedback Alignment (DFA)**, for training deep reinforcement learning agents. The goal was to develop and benchmark agents trained with DFA against those trained with standard backpropagation to assess the viability of DFA training for future neuromorphic systems.

<img src="/assets/images/meng1.png" alt="direct-feedback-alignment" class="align-center" style="border-radius: 1%;">

## Action

I structured my research in three phases:

1.  **Established Baselines:** I first implemented and benchmarked classical RL algorithms (Q-learning, SARSA) on custom-built game environments to establish performance baselines.
2.  **Developed AI Agents:** I then developed two parallel cohorts of deep RL agents. I trained one set of agents with standard backpropagation and the other with the experimental DFA algorithm, using deep neural networks (DNNs, CNNs) as function approximators.
3.  **Conducted Comparative Analysis:** I rigorously tested both agent cohorts across classic control problems and complex Atari game environments from the OpenAI Gym, directly comparing their learning efficiency and final performance.

<img src="/assets/images/meng2.png" alt="deep-reinforcement-learning" class="align-center" style="border-radius: 1%;">

## Interdisciplinary Integration

This project was my first deep synthesis of multiple advanced computing domains, requiring me to integrate concepts from:

* **Neuromorphic Computing:** Leveraging insights into brain-like computation to explore biologically plausible training methods beyond backpropagation.
* **Deep Learning:** Engineering and training dense (DNN) and convolutional neural networks (CNNs) to process raw sensory data from game environments.
* **Reinforcement Learning:** Applying core RL principles like Q-learning and SARSA to enable agent decision-making and learning over time.

## Result

My research successfully demonstrated the potential of this novel approach:

* **Validated the feasibility** of using Direct Feedback Alignment to train complex deep reinforcement learning agents.
* **Demonstrated that biologically plausible agents** could achieve performance comparable to conventional methods on challenging tasks.
* **Contributed the complete analysis and source code** to the open research community via an arXiv publication and a public GitHub repository.

## Technologies & Skills Used

**Technical**
* **AI Frameworks:** Python, TensorFlow, OpenAI Gym, NumPy, Pandas, Matplotlib
* **Algorithms:** Reinforcement Learning, Deep Learning, Direct Feedback Alignment (DFA)
* **Methodologies:** Comparative Algorithm Analysis, Benchmarking, Feasibility Studies

**Research & Communication**
* Academic Research & Scientific Writing
* Open Source Contribution (arXiv, GitHub)

## Publications & Resources

* [arXiv Publication](https://arxiv.org/abs/1905.04127)
* [GitHub Repository](https://github.com/AndreiRoibu/DeepReinforcementLearning)
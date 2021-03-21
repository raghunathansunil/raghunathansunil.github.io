---
layout: post
title: Evolution Strategies an Alternative to Reinforcement Learning - DQN   
date: '2021-03-16T14:31:00+00:00'
tags:   AI ML RL DQN ES
---

Evolution Strategy presents a good alternative to RL DQN for games like Atari and Human Exoskeleton systems. All this without needing a SGD algorithms, which is arguably not the way how humans intelligence works.  All popular AI/ML is primarily dependent on backpropogation algorithms for optimizations.  A refreshing new method is a worthy alternative.

The ability to combine RL unsupervised learning algorithm that evolves through environment interaction is already proven in many game uses cases: Blackgammon, Go, Atari, etc. The extension of the same in flying unmanned helicopters is well demonstrated. The extension of the same in several mission critical use cases such as driving is yet to be explored, due to following limitations:
]
1. complexity in exploding states, and actions
2. Non-stationary nature of the real-world scenarios
3. Challenges in effectively defining the rewards and penalty models consistently for a continuous and non-terminating scenarios.

Alternate models like Evolution strategy may hold the promise for future.


<b>References of Scholarly articles<b><br>
1. <a href="https://arxiv.org/abs/1703.03864"> ES Alternative to RL </a>
2. <a href="https://science.sciencemag.org/content/356/6344/1280"> Human Exoskeleton case </a>

<b>Basic Algorithm and Intuition References<b><br>
<a href=https://openai.com/blog/evolution-strategies/> ES Vs RL debate. </a>


---
layout: post
title: AI Reinforcement Learning - Modelling Real world  
date: '2021-02-26T14:31:00+00:00'
tags: AI RL 
---

Reinforcement Learning models is a choice to consider for real-world reward maximization requirements. It closely mimics real-world agents (like humans) to continuously improve planning and learning cycle through simulated and real experiences. 

Applying this model, will require modelling the real-world scenarios as as markov process of states, policy or rules of behaviour,  agent actions, goals/rewards for actions, probability of state transitions and the reward discounts. 

The value at a givens state and actions are given by a value functions. The reinforcement learning algorithms are setup to optimize the policy and the value functions to achieve rewards maximization goal provided there is a good understanding of the environment dynamics, computation resources and markov property of states. 

<table> 
<th> Reinforcement Algorithms - Tabular models Given Conditions </th>
    <tr> 
        <td> Algorithm </td>
        <td> Perfect envt. Model</td>
        <td> Computation Resources </td>
        <td> Markov process? </td>
    </tr>
    <tr> 
        <td> Dynamic Programming </td>
        <td> Yes - Distribution Model used for Planning </td>
        <td> High </td>
        <td> Strong </td>
    </tr>
    <tr> 
        <td> Monte Carlo </td>
        <td> No. Model free and relies on sampling for Learning </td>
        <td> Medium </td>
        <td> Yes. Complete episodes with Termination </td>
    </tr>
    <tr> 
        <td> Temporal Difference  </td>
        <td> No. Model free - sampling, but markov for learning. </td>
        <td> Medium </td>
        <td> Yes. can have incomplete sequence. Both episodic & continuing tasks. </td>
    </tr>
</table>

The learning algorithm characteristics are determined by backups, bootstrapping, policy iteration: evaluation and improvements, and exploration.
<table> 
<th> Reinforcement Algorithm Models</th>
    <tr> 
        <td> Algorithm </td>
        <td> Backup </td>
        <td> Bootstrapping </td>
        <td> Policy Evaluation </td>
        <td> Policy Improvement </td>
        <td> Exploration/Control </td>
        <td> Convergence condition </td>
    </tr>
    <tr> 
        <td> Dynamic Programming </td>
        <td> Full </td>
        <td> Yes </td>
        <td> Greedy with threshold for Value function improvements </td>
        <td> Select Policy for action that maximizes action state function for all action </td>
        <td> NA as it is exhaustive</td>
        <td> Maximum Actions </td>
    </tr>
    <tr> 
        <td> Monte Carlo </td>
        <td> Simulated Sampling </td>
        <td> None. Actual experience values </td>
        <td> Episode level:Epsilon-Soft policy selection and averaging of Value action function </td>
        <td> Episode level: Select Epsilon Greedy value action function (on-Policy) </td>
        <td> On Policy: Exploring Starts/Episilon Greedy and Off Policy: behavioud Policy based</td>
        <td> Robin-Monroe sequence where sum of steps is infinity, but its square is bounded.</td>
    </tr>
    <tr> 
        <td> Temporal Difference  </td>
        <td> Simulated Sampling </td>
        <td> T+1 boottrap </td>
        <td> Time Step: Predicted value at T+1 for the Value action function. Updated value function updated for episilon greedy </td>
        <td> Time Step: Select Epsilon-Greedy or max target policy with minimizing delta loss for Epsilon Greedy value action function</td>
        <td> On Policy: Sarsa and Off Policy: Q-Learning & Expected Sarsa</td>
        <td> Robin-Monroe sequence where sum of steps is infinity, but its square is bounded.</td>
    </tr>
</table>

For all the above model the Bellman optimality conditions and the dicounted value functions are at the core of the learning algorithms. 
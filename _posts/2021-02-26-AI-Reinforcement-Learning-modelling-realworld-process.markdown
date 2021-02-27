---
layout: post
title: AI Reinforcement Learning - Modelling Real world  
date: '2021-02-26T14:31:00+00:00'
tags: AI RL 
---

Reinforcement Learning models is a choice to consider for real-world reward maximization requirements. Applying this model, will require modelling the real-world scenarios as as markov process of states, policy or rules of behaviour,  agent actions, goals/rewards for actions, probability of state transitions and the reward discounts. 

The value at a givens state and actions are given by a value functions. The reinforcement learning algorithms are setup to optimize the policy and the value functions to achieve rewards maximization goal provided there is a good understanding of the environment dynamics, computation resources and markov property of states. 

<table> 
<th> Reinforcement Algorithms Given Conditions </th>
    <tr> 
        <td> Algorithm </td>
        <td> Perfect envt. Model</td>
        <td> Computation Resources </td>
        <td> Markov process? </td>
    </tr>
    <tr> 
        <td> Dynamic Programming </td>
        <td> Yes </td>
        <td> High </td>
        <td> Strong </td>
    </tr>
    <tr> 
        <td> Monte Carlo </td>
        <td> No. Model free </td>
        <td> Medium </td>
        <td> Yes. Complete episodes with Termination </td>
    </tr>
    <tr> 
        <td> Temporal Difference  </td>
        <td> No. Model free, but markov. </td>
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
        <td> Exploration </td>
        <td> Value function Improvement </td>
        <td> Convergence condition </td>
    </tr>
    <tr> 
        <td> Dynamic Programming </td>
        <td> Full </td>
        <td> Yes </td>
        <td> Greedy with threshold </td>
        <td> Convergence of Value state function improvements </td>
        <td> NA as it is exhaustive</td>
        <td> Greedy method for Value state function </td>
        <td> Maximum Actions </td>
    </tr>
    <tr> 
        <td> Monte Carlo </td>
        <td> Simulated Sampling </td>
        <td> None. Actual experience values </td>
        <td> Episode level:Epsilon-Soft policy selection and averaging </td>
        <td> Episode level: Averaging </td>
        <td> On Policy: Exploring Starts/Episilon Greedy and Off Policy: behavioud Policy based</td>
        <td> Sampling to derive value action function</td>
        <td> Robin-Monroe sequence where sum of steps is infinity, but its square is bounded.</td>
    <tr>
    <tr> 
        <td> Temporal Difference  </td>
        <td> Simulated Sampling </td>
        <td> T+1 boottrap </td>
        <td> Time Step: Predicted value at T+1  </td>
        <td> Time Step: Epsilon-Greedy or max target policy with minimizing delta loss </td>
        <td> On Policy: Sarsa and Off Policy: Q-Learning & Expected Sarsa</td>
        <td> Greedy with step size reduction and reducing Gamma for Value action function</td>
        <td> Robin-Monroe sequence where sum of steps is infinity, but its square is bounded.</td>
    </tr>
</table>

For all the above model the Bellman optimality conditions and the dicounted value functions are at the core of the learning algorithms. 
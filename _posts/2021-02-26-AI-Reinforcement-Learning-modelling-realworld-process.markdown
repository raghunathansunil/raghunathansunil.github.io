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
        <td> No </td>
        <td> Medium </td>
        <td> Low/Medium </td>
    </tr>
    <tr> 
        <td> Temporal Difference  </td>
        <td> No </td>
        <td> Medium </td>
        <td> Low/Medium </td>
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
        <td> Value Improvement </td>
        <td> Exploration </td>
    </tr>
    <tr> 
        <td> Dynamic Programming </td>
        <td> Full </td>
        <td> Yes </td>
        <td> Greedy with threshold </td>
        <td> Convergence of improvements </td>
        <td> Greedy </td>
        <td> NA as it is exhaustive</td>
    </tr>
    <tr> 
        <td> Monte Carlo </td>
        <td> Simulated Sampling </td>
        <td> None. Actual experience values </td>
        <td> Epsilon-Soft policy selection and averaging </td>
        <td> Averaging </td>
        <td> Sampling </td>
        <td> On Policy: Exploring Starts/Episilon Greedy and Off Policy: behavioud Policy based</td>
    <tr>
    <tr> 
        <td> Temporal Difference  </td>
        <td> Simulated Sampling </td>
        <td> T+1 boottrap </td>
        <td> Predicted value at T+1  </td>
        <td> Epsilon-Greedy or max target policy with minimizing delta loss </td>
        <td> Greedy with step size reduction and reducing Gamma</td>
        <td> On Policy: Sarsa and Off Policy: Q-Learning & Expected Sarsa</td>

    </tr>
</table>

For all the above model the Bellman optimality conditions and the dicounted value functions are at the core of the learning algorithms. 
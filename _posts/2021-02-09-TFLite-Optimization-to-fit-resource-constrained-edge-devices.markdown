---
layout: post
title: TFLite Optimization to fit resource constrained edge devices 
date: '2021-02-09T14:31:00+00:00'
tags: AI DL ML Tensorflow TFlite
---

TFLite brings in power of deploying AI/ML on resource constrained edge devices that lack memory, computing horsepower, storage and lacks floating point processing capabilities. All this with a small tradeoff on accuracy.

- Pre-Training and Post conversion quantization
- Size and Latency based optimizations

This is democratization of AI/ML deployments on edge contrary to thinking about cloud platforms. 

Google TF helps with the intuition and tricks to build edge model with their toolkits. But the real business case requiring a market-fit, architecture and design from ground-up will require many steps:

1. Collection, feature engineering, augmentation and data-pipeline - Google make it sound simple with curated TFdatasets
2. Pre-traininga model with ot without Transfer learning  --> Google make it sound simple leveraging its HUB with pretrained MobileNet models
3. The optimization choice: Pruning, Quantization, Size and Latency choices to pick from
4. Trade-off choices on accuracy versus loss for a test data and real-life prediction
5. Tracking of drifts and rinse-repeat of steps 1-4 periodically.

Most often one is stuck with steps 1-2. But, for those already got the  fundamentals of AI/ML algos, TF Lite intuition and learnt building edge toy models, the following papers provides a dee-dive into how and why's of edge AI/ML.


Edge AI/ML papers:<br>
<a href="https://arxiv.org/pdf/1801.04381.pdf"> MobileNetV2 </a> <br>
<a href="https://arxiv.org/abs/1712.05877"> Quantization basics </a> <br>


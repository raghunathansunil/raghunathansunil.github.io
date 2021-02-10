---
layout: post
title: AI Explainability - Speech Recognition Fundamentals 
date: '2021-02-09T14:31:00+00:00'
tags: AI DL ML Tensorflow TFlite
---

The open source of Speech recognition made possible with AI-ML algos with feature engineering science and techniques that emerged more than 25 yrs back. 

A marked move from DSP hardware and proprietary software for speec recognition has come a long way in last 25 years. (For those who remember Dragon Speech recognition software in mid 90's). The adoption has exponetially increased with AI/ML and open source. 

The underlying science has not changed fundamentally on sampling of sound at 16Khz (time vs amplitude in 25ms frames sliding in 10 ms), converting to frequency model with FFT (Frequency, Amplitude), vizualizing the spectogram patterns that uniquely identifies this, and conversion to Mel Filter banks to cluster high-frequency signals (MLCC - Mel Frequency Cepstral coefficients. 29 MFCC per frame) has not changed. 

But, the open source libraries that implement these makes all the difference to scale it significantly and explore newer frontiers in speech recognition: intonation, diction, Accent, emotion,...



References:<br>
<a href="https://github.com/mborgerding/kissfft"> KISS FFT </a> <br>
<a href="https://github.com/jameslyons/python_speech_features"> MLCC Python code </a> <br>
<a href="https://librosa.org/doc/latest/index.html"> Librosa Library for MLCC </a> <br>

Science: <br>
<a href="https://www.youtube.com/watch?v=spUNpyF58BY"> Fourier Transforms </a> <br>
<a href="http://practicalcryptography.com/miscellaneous/machine-learning/guide-mel-frequency-cepstral-coefficients-mfccs/"> Mel Frequency scales </a> <br>
<a href="https://jonathan-hui.medium.com/speech-recognition-feature-extraction-mfcc-plp-5455f5a69dd9"> MLCC </a> <br>
<a href="https://jonathan-hui.medium.com/speech-recognition-phonetics-d761ea1710c0">> Speech Recognition in humans mimicked </a><br>

Books
X. Huang, A. Acero, and H. Hon. Spoken Language Processing: A guide to theory, algorithm, and system development. Prentice Hall, 2001.



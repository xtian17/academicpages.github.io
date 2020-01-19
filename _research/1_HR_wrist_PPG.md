---
title: "Motion artifacts removal from photoplethysmogram(PPG) signal for robust heart rate (HR) tracking"
collection: research
permalink: /research/1_HR_wrist_PPG.md
excerpt: ''
date: 
venue: ''
paperurl: ''
citation: ''
---

## Introduction

Photoplethysmography(PPG) has attracted great interest these years with the fast development of wearable devices and semiconductors. PPG is obtained by pulse oximeter embedded in wearable devices, which emits light from light emission diode(LED) to the skin along with the underlying vessels and records the transmitted or reflected light intensity by photodetectors. Since the light intensity received by detectors is correlated with the blood volume in the vessel which fluctuates with the cardiac cycle, PPG has its widespread applications in extracting cardiac information, including heart rate(HR), blood oxygen saturation, respiration rate and more.
However, motion artifact(MA) created during physical fitness exercise is the one of the most problematic issues in applying PPG. MA contaminated PPG signal is distorted and even rendered to extract no useful HR signal for health analysis.

## Method

In this project, NLMS and RLS adaptive filters are implemented for motion artifacts removal from PPG signal in parallel and series modes. The steps and frameworks are basically referring to the two highly cited works. As for the HR tracking part, in contrast to the previous systems where the proposed HR tracking method depends on a set of heuristic rules, thresholds and searching ranges to be tuned, here we propose the peak selection problem as a most probable path selection task inspired by Viterbi algorithm. The HR tracking method using the idea of finding the most likely path is designated for higher performance of HR estimation accuracy. Also, adaptive searching range based on SNR is included in the tracking algorithm.

## Experimental Result

### Dataset 1:
The database used for this project is public available and has been widely cited since Signal Processing Cup 2015. In this dataset, two-channel PPG signal, three-axis acceleration signal and one-channel ECG signal with 5-min duration are simultaneously recorded from 12 healthy male subjects aged from 18 to 35. Those subjects were running starting from 0.5 minutes to the end of the whole duration with speed of 8-15km/h. For each subject, the PPG signal is recorded from wrist by two pulse oximeters with green LEDs(wavelength: 515nm). Their distance (from center to center) is 2 cm. The acceleration signal is also recorded simultaneously from wrist by a three-axis accelerometer. Both the pulse oximeter and the accelerometer are embedded in a wristband, which is comfortably worn. The ECG signal is recorded simultaneously from the chest using wet ECG sensors. All signals are sampled at 125 Hz.

### Dataset 2: MAST dataset

![](https://xtian17.github.io/images/HR_wrist_PPG/dataset2.png)

### Metrics
To evaluate the performance of the proposed system and to compare with the state-of-art, average absolute error(AAE) is used.


### Results
Here is an example of HR tracking result after MA removal for the input PPG siganl.
![](https://xtian17.github.io/images/HR_wrist_PPG/HR_wrist_PPG.png)







---
title: "Motion artifacts removal from photoplethysmogram(PPG) signal for robust heart rate (HR) tracking"
collection: research
permalink: /research/2018-06-01-HR-wrist-PPG
excerpt: 'In this project, adaptive filters techniques combined with a robust tracking algorithm are implemented for accurate HR estimation from wrist type PPG.'
date: 2018-06-01
location: "Collge Park, MD"
---

## Introduction

Photoplethysmography(PPG) has attracted great interest these years with the fast development of wearable devices and semiconductors. PPG is obtained by pulse oximeter embedded in wearable devices, which emits light from light emission diode(LED) to the skin along with the underlying vessels and records the transmitted or reflected light intensity by photodetectors. Since the light intensity received by detectors is correlated with the blood volume in the vessel which fluctuates with the cardiac cycle, PPG has its widespread applications in extracting cardiac information, including heart rate(HR), blood oxygen saturation, respiration rate and more. However, motion artifact(MA) created during physical fitness exercise is the one of the most problematic issues in applying PPG. MA contaminated PPG signal is distorted and even rendered to extract no useful HR signal for health analysis. In this project, adaptive filters techniques combined with a robust tracking algorithm are implemented for accurate HR estimation from wrist type PPG. 

## Results
Here is an example of HR tracking result after MA removal for the input PPG siganl.
![](https://xtian17.github.io/images/HR_wrist_PPG/HR_wrist_PPG.png)



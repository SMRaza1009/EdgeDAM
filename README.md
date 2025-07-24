
<!-- Title + authors -->
# EdgeDAM: Real-time Distractor-Aware Object Tracking for Mobile Devices

 <!-- <p align="center"> -->
<!-- [Syed Muhammad Raza](https://www.linkedin.com/in/smraza1009/)* · [Syed Murtaza Hussain Abidi](https://www.linkedin.com/in/murtazahussain0/) · [Muhammad Ibrahim](https://www.linkedin.com/in/muhammad-ibrahim-<!-- 83643b1a2/?original_referer=https%3A%2F%2Fwww%2Egoogle%2Ecom%2F&originalSubdomain=au) · [Ajmal Mian](https://ajmalsaeed.net/) 
<!-- </p> -->

<div align="center">

[Syed Muhammad Raza](https://www.linkedin.com/in/smraza1009/)* ·  [Syed Murtaza Hussain Abidi](https://www.linkedin.com/in/murtazahussain0/) ·  [Muhammad Ibrahim](https://www.linkedin.com/in/muhammad-ibrahim-83643b1a2/) ·  [Ajmal Mian](https://ajmalsaeed.net/)
</div>

---

## Overview

 EdgeDAM integrates a fast YOLOv11s detection backbone, a CSRT tracker, and an enhanced Distractor-Aware Memory (DAM) module specifically optimized for detection-driven occlusion handling.
 EdgeDAM achieves state-of-the-art results running at **25 FPS** on **iPhone 14 Pro Max** and **iPhone 15 Pro Max** 


<!-- Embedding a figure -->
<p align="center">
 <img src="fig1.pdf" width="600px" alt="AccuracyVsFPS">
 <br><em>Figure 1. Comparison of EdgeDAM with SOTA, and EdgeDAM is **1.8x faster** then recent methods.</em>
</p>

---

## Abstarct

Robust visual object tracking (VOT) under occlusion remains a fundamental challenge, particularly on mobile devices. Existing memory-based approaches effectively handle occlusion, but suffer from computational inefficiency due to the reliance on segmentation architectures that require significant processing power and memory. In this paper, we propose \textbf{EdgeDAM}, a lightweight and mobile-friendly framework for single-object tracking. EdgeDAM integrates a fast YOLOv11s detection backbone, a CSRT tracker, and an enhanced Distractor-Aware Memory (DAM) module specifically optimized for detection-driven occlusion handling. Unlike traditional segmentation-based memory methods, our DAM module employs IoU-guided filtering, area-consistent validation, confidence-aware distractor queuing, and dual-memory separation. These innovations significantly improve the target recovery and temporal stability without additional inference overhead. Extensive experiments demonstrate that EdgeDAM achieves state-of-the-art results, including 88.2% accuracy on the DiDi dataset, 84.9\% EAO on VOT2020, and 79.0\% EAO on VOT2022. It also obtains competitive performance on LaSOT (89.5% AUC), LaSOText (64.1% AUC), and GOT-10k (83.1% AO), running at 25 FPS on iPhone 14 Pro Max and iPhone 15 Pro Max. To the best of our knowledge, EdgeDAM is the first detection-centric memory-aware tracking method tailored for real-time occlusion recovery on edge devices. 

---

## Overall System Architecture

<!-- Embedding a figure -->
<p align="center">
 <img src="overall_architecture.png" width="600px" alt="System architecture">
 <br><em>Figure 2. EdgeDAM overall system architecture composed of detection backbon of YOLO11s with CSRT tracker, DAM memory bank.</em>
</p>







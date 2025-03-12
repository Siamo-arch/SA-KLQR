---
layout: default
title: Adaptive Koopman-Based Force Control for Deformable Tool Manipulation
description: Project page for our research on adaptive force control in robotic swabbing using Koopman-based modeling and centroid-aware regulation.
---

<header>
  <h1>Adaptive Koopman-Based Force Control for Deformable Tool Manipulation</h1>
  <p><em>Project webpage for our research on robotic force control in deformable tool manipulation.</em></p>
</header>

## Overview
This study presents an adaptive **Koopman-based force control framework** for **deformable tool manipulation (DTM)**, focusing on applications in **robotic environmental swabbing**. The approach leverages Koopman operator theory for **real-time force regulation**, enhanced with centroid-based monitoring for improved force distribution. 

This work contributes to **precision force control**, ensuring stable and uniform contact pressure while accounting for tool compliance. The methodology is tested in real-world swabbing tasks, demonstrating superior force adaptation compared to traditional PID and sliding mode controllers.

## Key Contributions
- **Koopman-based adaptive force control** for handling deformable tools.
- **Centroid-aware force distribution monitoring**, ensuring balanced force application.
- **Comparison with PID and SMC controllers**, showing improved stability and tracking accuracy.
- **Real-world validation** on robotic swabbing tasks.

## Results
Our method demonstrates:
- **Improved force tracking performance** (lower RMSE and MAE).
- **Superior stability in both low and high-frequency force variations**.
- **More uniform force application**, reducing tool deformation risks.
- **Efficient real-time adaptation** compared to baseline controllers.

### **Figures**
| Force Tracking Performance | Absolute Force Error | Centroid Force Distribution |
|---------------------------|----------------------|----------------------------|
| ![Force Tracking](./Figures/sins.png) | ![Absolute Error](./Figures/sin-er.png) | ![Centroid Analysis](./Figures/heatmap.png) |

## Future Work
This framework lays the foundation for **fully learning-based** control methods, such as **imitation learning**, by providing a robust force regulation system. Future studies will focus on further **reducing sensor dependencies**, exploring **learning-based actuator tracking**, and benchmarking human vs. robotic swabbing performance.

## Publication
_This page is currently anonymized for double-blind review. The final version, including author details, code, and dataset, will be available upon acceptance._

## Code & Data
_Source code and dataset will be released after publication._

---

<footer>
  <p>&copy; 2024 Research Group. This project is under review. Final details will be shared upon acceptance.</p>
</footer>

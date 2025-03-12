---
layout: default
title: "Adaptive Koopman-Based Force Control for Robotic Swabbing"
description: "Project page for our study on force control in robotic swabbing, integrating Koopman operator theory and fuzzy force regulation for accurate deformable tool manipulation."
author: "Anonymous (Double-Blind Review)"
---

# Adaptive Koopman-Based Force Control for Robotic Swabbing 🦾🔬

## Overview
This research introduces an **adaptive Koopman-based force control framework** for **deformable tool manipulation (DTM)** in robotic swabbing applications. The framework integrates **Koopman operator theory** with a **centroid-based fuzzy force regulation algorithm**, ensuring precise and adaptive force application across **non-rigid, deformable surfaces**.

### Key Contributions:
✅ **Koopman-Based Force Control**: Real-time adaptive force regulation using an **optimized Koopman lifting function**.<br>
✅ **Centroid-Based Force Tracking**: Ensuring **even force distribution** and **reduced tool deformation**.<br>
✅ **State-Dependent Koopman Switching**: Enhancing force stability through **real-time operator selection**.<br>
✅ **Performance Benchmarking**: Comparing with **PID and SMC controllers**, demonstrating superior tracking accuracy.

---

## 🔬 Research Motivation

**Environmental swabbing in meat processing plants** requires robots to **apply controlled force while ensuring uniform coverage**. Unlike rigid robotic tools, **deformable swabs change properties** during interaction, requiring **adaptive control strategies**.

While robotic **nasopharyngeal swabbing** has been explored for COVID-19 testing, **industrial swabbing presents additional challenges**:
- **Variable Surface Textures** 🛠️: Rough, slippery, and uneven surfaces impact force stability.
- **Tool Deformation** 🔄: The swab **absorbs moisture**, changing its **mechanical properties**.
- **Friction Variability** 🏭: Industrial residues like **grease and blood** affect swab motion.

Our approach **overcomes these limitations** by leveraging **Koopman operator-based modeling** and **centroid error-based force tracking**.

---

## 🔹 Koopman-Based Force Control

The **Koopman operator** enables **globally linearized dynamics** for a **nonlinear swabbing system**. Instead of approximating direct nonlinear dynamics, the system evolves through an **observables space**, where linear control techniques (e.g., LQR) can be applied.

### **State-Dependent Koopman Switching**
A **single Koopman operator** cannot accurately capture the full force dynamics due to:
- **Changing arm inertia**
- **Variable contact force**
- **Real-time tool deformation**

💡 **Solution:** Instead of using a single operator, we implement **state-dependent Koopman switching**, selecting the most relevant Koopman operator in real time.

<div align="center">
    <img src="/assets/images/koopman-switching.png" alt="Koopman Switching Mechanism" width="80%">
    <p><em>Figure 1: State-dependent Koopman switching ensures real-time adaptability in force control.</em></p>
</div>

---

## 🎯 Centroid-Based Fuzzy Force Regulation

To ensure **uniform force distribution**, a **centroid error fuzzy regulation algorithm** is introduced. This method:
- Monitors **real-time force centroid drift** 🛠️
- Adjusts the **robot's rolling angle** 🔄
- Prevents **excessive swab deformation** 🚨

**Equation: Centroid Error Computation**
\[
D = \sqrt{(C_x - C_x^*)^2 + (C_y - C_y^*)^2}
\]
where **\( C_x^*, C_y^* \)** represent the **ideal centroid location**.

### 🔹 **Effect on Force Distribution**
Without the centroid-based regulation, **force application is inconsistent**, leading to **unstable rolling angles** and **incomplete surface coverage**. 

<div align="center">
    <img src="/assets/images/centroid-error.png" alt="Centroid-Based Force Distribution" width="80%">
    <p><em>Figure 2: Force distribution heatmap. (Left) Without regulation: force inconsistencies. (Right) With regulation: uniform application.</em></p>
</div>

---

## 🏆 Experimental Results

### **Comparison of Controllers for Sine and Triangle Waves**
To benchmark performance, **sinusoidal** and **triangular force trajectories** were used. **Performance metrics** (MaxAE, RMSE) were compared for **low- and high-frequency tracking**.

<div align="center">
    <img src="/assets/images/tracking-results.png" alt="Tracking Performance" width="80%">
    <p><em>Figure 3: Force tracking results for sinusoidal and triangular reference trajectories.</em></p>
</div>

📊 **Table 1: Force Tracking Performance Comparison**
| Controller  | Sine (Low Freq) | Sine (High Freq) | Triangle (Low Freq) | Triangle (High Freq) |
|------------|----------------|------------------|------------------|------------------|
| **SA-KLQR** | ✅ Best | ✅ Best | ✅ Best | ✅ Best |
| **PID**     | ❌ Phase lag | ❌ High error | ❌ Lag at transitions | ❌ Overshoot |
| **SMC**     | ⚠️ Oscillations | ⚠️ Instability | ⚠️ Chattering | ⚠️ High variance |

---

## 🚀 Practical Impact

🔹 **Robotic Swabbing for Food Safety** 🏭
- **Improves biosecurity** in food processing environments.
- Reduces **human labor dependency** for swabbing.

🔹 **Deformable Tool Manipulation (DTM) Framework** 🤖
- Extends to **surgical robots**, **soft grippers**, and **agriculture robotics**.

🔹 **Bridging Model-Based and Learning-Based Control** 📡
- **Accurate actuator data** enables **behavior cloning** for fully data-driven learning.

---

## 📜 Citation

If you find this work useful, please consider citing:


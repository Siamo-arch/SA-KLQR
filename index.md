---
layout: splash
title: "Data-Driven Contact-Aware Control Method for Real-Time Deformable Tool Manipulation: A Case Study in the Environmental Swabbing
"
description: "33."
header:
  overlay_image: /assets/cover.jpg
  overlay_filter: 0.2
  caption: "🔬 Authors and lab name are anonymized for double-blind review."
  actions:
    - label: "📄 Read the Paper (submitted)"
      url: "#"
      icon: "fas fa-file-pdf"
    - label: "🖥️ GitHub Repository"
      url: "#"
      icon: "fab fa-github"
    - label: "📹 Watch Demo"
      url: "#"
      icon: "fas fa-video"
---

# 🚀 S

## 🔬 Overview  
This project introduces **State-Adaptive Koopman LQR (SA-KLQR)**, a novel data-driven control framework for real-time **deformable tool manipulation (DTM)**. Our case study focuses on environmental swabbing in food safety, where maintaining precise contact force and coverage consistency is crucial.

> *"Precision in force control is critical for robotic swabbing to ensure effective microbial collection and surface coverage."*

### **✨ Key Contributions**
✔ **Koopman-Based Linearization** → Models complex force dynamics in DTM.  
✔ **SA-KLQR Control Framework** → Combines Koopman operators with optimal LQR control.  
✔ **Centroid-Based Fuzzy Regulation** → Balances force distribution & minimizes tool misalignment.  
✔ **Robotic Swabbing Case Study** → Evaluates system performance in industrial hygiene settings.  

---

## 📊 Performance Evaluation

### **📌 Force Tracking Comparison**  
The table below compares **SA-KLQR vs. other controllers** for robotic swabbing.

| **Controller**   | **RMSE (N)** | **MAE (N)** | **Force Error (%)** |
|-----------------|------------|------------|-----------------|
| 🔵 **SA-KLQR**   | **0.006**  | **0.002**  | **3%** ✅ |
| 🟢 **PID**       | 0.12       | 0.08       | 10% ❌ |
| 🔴 **SMC**       | 0.09       | 0.07       | 7% ❌ |

📊 **Detailed experimental results are available in the [paper](#).**

---

## 🏆 Why SA-KLQR?  
Unlike traditional controllers, **SA-KLQR** adapts to **deformable tool dynamics**, ensuring:  
✅ **Minimal tracking error** → More **precise** force control.  
✅ **Stable tool compliance** → Avoids **unnecessary deformations**.  
✅ **Higher coverage efficiency** → Improves **surface consistency** in swabbing.  

---

## 📄 Read the Paper  
📄 **[Read Full Paper](#)** *(Link to be added upon publication)*  

## 🖥️ Code & Dataset  
- **GitHub Repository** → [SA-KLQR Codebase](#) *(To be published soon)*  
- **Benchmark Dataset** → Available soon.  

## 🎥 Video Demonstration  
Watch SA-KLQR in action:  
📽️ **[Watch Here](#)** *(To be added)*  

---

## 🌍 Stay Connected  
Stay updated with the latest advancements:  
- **GitHub** → [SA-KLQR Repository](#)  
- **Twitter** → [@YourLab](#)  
- **Website** → [YourLab.com](#)  

🚀 *This page is continuously updated. More content coming soon!*

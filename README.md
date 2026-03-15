# 🚗 Sensorless MFO Detection via Physics-Informed Tabular GenAI

[![License: Open Source](https://img.shields.io/badge/License-Open_Source-blue.svg)](#)
[![AI Field: Generative AI](https://img.shields.io/badge/Field-Generative_AI-orange.svg)](#)
[![Industry: EV Charging](https://img.shields.io/badge/Industry-EV_Charging-green.svg)](#)

This project addresses the critical data scarcity bottleneck in **Metallic Foreign Object (MFO)** detection for **Wireless Power Transfer (WPT)** systems. By bridging power electronics with state-of-the-art **Generative AI**, we eliminate the need for costly physical sensor hardware.

---

## 1. Background and Concept
Ensuring operational safety in EV charging relies on reliable MFO detection. Conventional methods depend on physical hardware (thermal/magnetic sensors), which increases the Bill of Materials (BOM) and introduces calibration vulnerabilities.

**Our Innovation:**
* **Sensorless Paradigm:** Monitoring real-time efficiency variations to infer MFO interference.
* **The Problem:** Collecting empirical data for every physical interference and spatial misalignment is practically impossible due to prohibitive costs.
* **The Solution:** A physics-informed tabular data synthesis framework that generates high-fidelity electromagnetic interference patterns, transforming a hardware constraint into a scalable algorithmic solution.

---

## 2. Features and Functionality
The project operates as a rigorous backend algorithmic pipeline focused on machine learning efficacy:

* **High-Fidelity Tabular Data Synthesis:** Automatically synthesizes complex, multidimensional data rows representing spatial classes, load conditions ($RL$), and efficiency metrics ($\eta$).
* **Algorithmic Benchmarking Protocol:** Systematically evaluates six cutting-edge tabular generative models.
* **Enhanced Downstream Inference:** Integrates synthesized datasets into classification architectures to validate improvements in detection accuracy.
* **Hardware-Agnostic Scaling:** A purely algorithmic enhancement deployable across various WPT topologies without physical retrofitting.

---

## 3. Development Tools and Techniques

### Generative AI Architectures
We implement, fine-tune (via **Optuna**), and benchmark six specialized Tabular GenAI models:
1.  **TVAE** (Tabular Variational Autoencoder) 
2.  **CTGAN** (Conditional Tabular GAN)
3.  **TabDDPM** (Tabular Denoising Diffusion Probabilistic Model) 
4.  **MDN** (Mixture Density Network) 
5.  **CopulaGAN** 
6.  **WGAN-GP** (Wasserstein GAN with Gradient Penalty) 

### Evaluation Metrics
| Phase | Focus | Methodology |
| :--- | :--- | :--- |
| **Phase 1** | **Statistical Similarity** | Evaluated against empirical baselines using the **Kolmogorov-Smirnov (KS) test** to ensure models respect physical electromagnetic variations. |
| **Phase 2** | **ML Efficacy** | Training ensemble classifiers (**CatBoost, LightGBM, XGBoost**) on augmented data, quantified by **Accuracy** and **Macro F1-score**. |

---

## 👥 4. Target User and Environment
* **Target Users (B2B):** Tier-1 automotive electronics suppliers, EV charging infrastructure developers, and industrial automation firms.
* **Deployment Environment:** Designed as a backend training pipeline for cloud-based or edge-computing WPT controllers (MCUs) operating at 85 kHz or 100 kHz.

---

## 5. Industry Application & Impact
* **Commercial Value:** Complete elimination of physical sensor arrays (thermal/magnetic), directly reducing manufacturing costs[cite: 3].
* **Safety & Trust:** Maximizes charging safety, prevents hardware degradation/fire hazards, and accelerates consumer trust in autonomous EV charging.

---

## References
* **Foundational Research:** Ho & Dat (2025). *Establishing a baseline mapping of real-time efficiency drops for sensorless detection*.

---
*Submitted for the Best AI Awards Project Description.* 
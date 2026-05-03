SRAM-based Hybrid AI Acceleration for Edge Inference ⚡

Overview

This project explores the design and evaluation of a hybrid SRAM-based Compute-in-Memory (CiM) AI accelerator for efficient edge inference. The work addresses the limitations of traditional von Neumann architectures by reducing data movement and enabling computation directly within memory.

The proposed architecture leverages charge-domain analog computing with C-2C capacitor ladders, combined with a hardware-software co-design methodology to achieve energy-efficient and scalable AI acceleration.

Motivation 🚀

Modern AI applications rely heavily on cloud-based computation, which introduces:

High latency
Privacy concerns
Dependence on connectivity

Shifting AI inference to edge devices requires low-power and efficient hardware, which is difficult to achieve using conventional architectures due to the von Neumann bottleneck.

This project investigates Compute-in-Memory (CiM) as a solution.

Key Contributions 🧠

Design of a charge-domain SRAM-based CiM architecture
Implementation of C-2C capacitor ladder for linear MAC operations
Analysis of hardware non-idealities in UMC 65nm technology
Investigation of inter-array communication losses in scalable systems
Development of a hardware-aware AI training framework

System Architecture ⚙️

Compute-in-Memory (CiM) Core
SRAM-based architecture for reliability and maturity
Charge-domain computation using capacitive coupling
Passive charge accumulation for energy efficiency
C-2C Capacitor Ladder
Enables binary-weighted multiply-accumulate (MAC) operations
Improves linearity and scalability
Array-Level Design
Scalable 8×8 / 16×16 CiM arrays
Passive interconnection for accumulation
Integrated DACs and ADCs
Research Focus 🔍

How to minimize power losses and maintain accuracy when scaling across multiple analog CiM arrays?

Focus areas:

Inter-array communication
Charge-domain signal propagation
Impact of parasitics and mismatch

Hardware Implementation 🧩

Technology
UMC 65nm CMOS process
Cadence Virtuoso
Challenges Addressed
Parasitic capacitance
Capacitor mismatch
Thermal noise (kT/C)
Signal degradation

AI Hardware-Software Co-Design 🤖

Workflow
Hardware Noise Profiling
Noise-Aware Training (PyTorch)
Model Validation

Ensures robustness to hardware non-idealities.

Tools & Technologies 🛠️

Cadence Virtuoso
PyTorch
MATLAB / Python
SPICE-based tools

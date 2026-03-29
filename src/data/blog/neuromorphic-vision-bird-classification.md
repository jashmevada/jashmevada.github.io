---
title: "Neuromorphic Vision Bird Classification using Spiking Neural Networks"
description: "End-to-end pipeline converting RGB videos into event-based DVS data using an IEBCS simulator, then classifying bird species with a Spiking Neural Network."
pubDatetime: 2026-01-01T00:00:00Z
tags: ["spiking-neural-networks", "neuromorphic", "pytorch", "computer-vision", "python"]
featured: true
---

## Overview

This personal research project explores **neuromorphic computing** applied to bird classification. Instead of using conventional frame-based video, the pipeline converts standard RGB video into event-based data — mimicking the output of a Dynamic Vision Sensor (DVS) — and feeds it into a Spiking Neural Network (SNN) classifier.

## Pipeline

1. **Video Input** — standard RGB bird footage
2. **Event Conversion** — RGB frames are processed through the IEBCS DVS simulator to generate asynchronous event streams
3. **SNN Training** — event data is fed into an SNN built with Norse (a PyTorch-based SNN library) for species classification

## Why Neuromorphic?

DVS cameras and SNNs are inherently temporal and energy-efficient. They encode motion and change rather than full frames, making them well-suited for fast-moving biological subjects like birds. This project tests whether event-based representations can achieve competitive accuracy on a naturalistic classification task.

## Tech Stack

- **Python** — core implementation
- **PyTorch** — deep learning backbone
- **Norse** — spiking neural network layers and dynamics
- **OpenCV** — video preprocessing
- **NumPy** — numerical operations
- **IEBCS** — event-based camera simulator

## Repository

[github.com/jashmevada/NeuroBCDA](https://github.com/jashmevada/NeuroBCDA)

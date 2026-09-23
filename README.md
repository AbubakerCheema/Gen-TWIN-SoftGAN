# Gen-TWIN Soft-GAN for RF Data Augmentation

A PyTorch implementation of a **Soft-Attention LSTM-based Generative Adversarial Network (Soft-GAN)** for synthetic RF IQ data generation and augmentation.

## Overview

This project learns the temporal and statistical characteristics of RF signals from **RadioML 2016.10a** and generates synthetic IQ sequences for data augmentation and digital-twin applications.

### Key Components

* RF IQ preprocessing and normalization
* LSTM-based Generator and Discriminator
* Soft-Attention mechanism in the Generator
* Spectral normalization
* Adversarial training
* Synthetic IQ sequence generation
* Training and convergence analysis

## Dataset

**RadioML 2016.10a**

* Complex I/Q samples
* Time-series RF representation
* Modulated wireless communication signals

## Model

The Soft-GAN consists of:

**Generator:** LSTM + Soft Attention → Synthetic IQ sequence

**Discriminator:** LSTM → Real/Fake classification

The attention mechanism enables the Generator to focus on informative temporal features when producing RF sequences.

## Evaluation

Generated samples are evaluated using:

* Generator/Discriminator loss
* I/Q mean and standard deviation
* Temporal signal statistics
* Real vs. synthetic IQ distribution

## Applications

* RF dataset augmentation
* Wireless signal modeling
* Digital Twin generation
* AI-enabled Open RAN research
* Synthetic RF data generation

## Technologies

Python · PyTorch · NumPy · Pandas · Matplotlib · Scikit-learn · Jupyter

## Reference

O. Basaran *et al.*, **"Gen-TWIN: Generative-AI-Enabled Digital Twin for Open Radio Access Networks,"** IEEE INFOCOM Workshops, 2025.

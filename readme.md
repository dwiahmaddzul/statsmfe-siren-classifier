# StatsMFE Siren Classifier

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Paper](https://img.shields.io/badge/Paper-ICIC%20Express%20Letters-green.svg)](#citation)

Efficient emergency vehicle audio classification using Statistical MFE features - achieving **8.2× faster feature extraction** than MFCC with ensemble learning.

## 🎯 Overview

This repository contains the implementation of a novel approach for emergency vehicle siren classification using **Statistical Mel-Filterbank Energy (MFE)** features. Our method provides a computationally efficient alternative to traditional MFCC-based approaches while maintaining competitive accuracy.

### Key Features

- ⚡ **8.2× faster** feature extraction compared to MFCC
- 💾 **4.85× memory reduction** (172 features vs 834 MFCC features)
- 🎯 **Competitive accuracy** using ensemble learning
- 🚀 **Optimized for edge deployment** (Jetson, Raspberry Pi, etc.)
- 🔊 Three-class classification: Ambulance, Firetruck, Traffic

## 📊 Performance Highlights

| Method | Features | Accuracy | Extraction Time | Memory |
|--------|----------|----------|----------------|--------|
| MFCC (Baseline) | 834 | 95.2% | 8.2s | 100% |
| **Statistical MFE (Ours)** | 172 | 94.8% | 1.0s | 20.6% |
| Raw MFE | 836 | 95.5% | 1.2s | 100.2% |

*Results based on 5-fold cross-validation on emergency vehicle siren dataset*

## 🏗️ Architecture

### Feature Extraction Pipeline
# Wavelet-Based Image Denoising and Analysis

This project implements a complete pipeline for reading PGM images, performing wavelet decomposition/reconstruction using the Haar filter, and applying various thresholding methods for image denoising. Additionally, the project compares the custom denoising approach with standard library methods such as BayesShrink, VisuShrink, median filter, and uniform filter.

## Features

- **Custom PGM Image Reader**: Supports both ASCII (P2) and binary (P5) PGM formats.
- **Discrete Wavelet Transform (DWT)**: Implements forward (FDWT) and inverse (IDWT) transforms using the Haar filter.
- **Wavelet Subband Visualization**: Decomposes images into LL, LH, HL, and HH subbands for inspection.
- **Image Denoising**: 
  - Applies preprocessing using a median filter.
  - Implements five thresholding methods (universal, VisuShrink, sure, bayes, normal) for denoising wavelet coefficients.
  - Compares the performance of custom denoising with standard methods.
- **Quality Metrics**: Computes Mean Squared Error (MSE) and Structural Similarity Index (SSIM) to evaluate denoising performance.
- **Extensible Code Base**: Contains testing and debugging sections for batch processing of images.

## Requirements

- **Python**: 3.10.4 (or later)
- **Libraries**:
  - NumPy
  - Matplotlib
  - SciPy
  - scikit-image
  - Pandas

Install the required packages via pip if not already installed:

```bash
pip install numpy matplotlib scipy scikit-image pandas

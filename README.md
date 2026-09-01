# DSP and Harmonic Composition Portfolio

This repository contains Python scripts showcasing core digital signal processing (DSP) concepts. It serves as a practical supplement to my academic transcripts and senior thesis.

## Core Implementations

### 1. Statistical Signal Detection (`iir_filter.ipynb`)
* **Objective:** Extracts a low-amplitude sine wave embedded in dense white noise.
* **Key Techniques:** Implements a Constant False-Alarm Rate (CFAR) threshold. It maps the noise spectrum to a Rayleigh distribution to calculate a statistical threshold for peak detection.
* **Filtering:** Applies a zero-phase 5th-order Butterworth bandpass filter to isolate the target frequency without distorting the phase.

### 2. Fourier Series Wave Synthesis (`square_wave_synthesis.ipynb`)
* **Objective:** Rebuilds a square wave step-by-step from its individual odd harmonics.
* **Key Techniques:** Plots the time-domain waveform alongside its frequency spectrum to verify that the spikes align with the theoretical 1/f envelope.
* **Mathematical Artifact:** Demonstrates the Gibbs phenomenon (the ringing and overshoot at sharp edges) caused by cutting off an infinite Fourier series at a finite number of harmonics.

## Environment Requirements
* Python 3.x
* NumPy, SciPy, Matplotlib, NoiseReduce
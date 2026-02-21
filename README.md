# Emotion Detection from Speech using Edge AI

This project detects human emotions from speech using deep learning and deploys a lightweight TensorFlow Lite model for IoT edge devices such as Raspberry Pi.

## Problem Statement

Speech emotion recognition systems typically rely on cloud processing, which introduces latency and privacy concerns. This project proposes an edge-based solution that performs emotion detection locally using an optimized deep learning model.

## Methodology

- Audio preprocessing using MFCC feature extraction  
- CNN-based emotion classification  
- Model optimization using TensorFlow Lite  
- Latency comparison between normal and edge inference

## Dataset

RAVDESS (Ryerson Audio-Visual Database of Emotional Speech and Song)
Speech subset used for training.

Dataset not included due to size:
https://zenodo.org/record/1188976

## Results

Test accuracy: **~59%**

Latency reduced from **~137 ms → ~7 ms** after TFLite optimization

Edge inference enables offline, privacy-preserving emotion detection

**System workflow is illustrated below:**
## Pipeline

Audio → MFCC → CNN Model → TensorFlow Lite → Edge Device → Emotion Output

## Repository Structure

notebooks → training and experimentation notebook

models → trained model information

tflite → optimized edge model

results → evaluation screenshots

This demonstrates feasibility of real-time emotion detection on edge devices.

dataset → dataset information

## Future Work

Real-time microphone emotion detection

CNN + LSTM hybrid architecture

Larger multi-speaker datasets

Mobile app deployment

Author: Bhumi Shah

BTech Computer Science-3rd year(Minor Project)

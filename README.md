# NEXA-AIR
AI-powered Android hand gesture tracking and recognition application built with Java, CameraX, MediaPipe Hand Landmarker, and real-time computer vision.



# ✋ NEXA AIR — AI Hand Gesture Tracking

<p align="center">
  <strong>Real-Time AI • Computer Vision • Android • Gesture Recognition</strong>
</p>

<p align="center">
  NEXA AIR transforms an Android smartphone camera into a real-time AI-powered hand tracking and gesture recognition system.
</p>

<p align="center">

![Platform](https://img.shields.io/badge/Platform-Android-green)
![Language](https://img.shields.io/badge/Language-Java-orange)
![UI](https://img.shields.io/badge/UI-XML-blue)
![Camera](https://img.shields.io/badge/Camera-CameraX-blue)
![Vision](https://img.shields.io/badge/Vision-MediaPipe-purple)
![Database](https://img.shields.io/badge/Storage-SharedPreferences-yellow)
![Status](https://img.shields.io/badge/Status-Active%20Development-success)
![Version](https://img.shields.io/badge/Version-v1.0-yellow)

</p>

---

## 🚀 Overview

**NEXA AIR** is an Android-based artificial intelligence and computer-vision application designed to detect, track, and recognize human hand gestures in real time using a smartphone camera.

The application combines **Android development, CameraX, MediaPipe Hand Landmarker, landmark-based gesture classification, custom real-time rendering, and performance monitoring** into a single computer-vision platform.

Instead of relying solely on traditional touch interaction, NEXA AIR explores how a smartphone camera can be used to understand hand positions and gestures.

The current version recognizes five primary gestures:

- 🖐️ Open Palm
- ✊ Fist
- ☝️ Point
- 👍 Thumbs Up
- ✌️ Peace

The project has been designed with a modular processing pipeline so that the recognition system can be expanded with additional gestures and interaction capabilities in future versions.

> **Current scope:** NEXA AIR is currently an Android hand-tracking and gesture-recognition application. Advanced PC control, mouse control, gaming controls, and wireless communication are planned future capabilities and are not part of the current implementation.

---

## 🎯 Project Objective

The primary objective of NEXA AIR is to explore practical applications of **AI-powered computer vision on Android devices**.

The application demonstrates how a smartphone can:

- Detect a user's hand
- Track 21 hand landmarks
- Analyze hand landmark relationships
- Recognize predefined gestures
- Calculate gesture confidence
- Visualize hand tracking in real time
- Monitor FPS and processing latency
- Provide immediate tracking feedback

NEXA AIR serves as the foundation for a larger gesture-based human-computer interaction platform.

---

# 🧠 Computer Vision Pipeline

NEXA AIR uses a modular processing pipeline:

```text
CameraX
   ↓
CameraManager
   ↓
Camera Frames
   ↓
HandLandmarkerHelper
   ↓
MediaPipe Hand Landmarker
   ↓
21 Hand Landmarks
   ↓
GestureClassifier
   ↓
GestureResult
   ↓
GestureTrackingActivity
   ↓
HandOverlayView + UI

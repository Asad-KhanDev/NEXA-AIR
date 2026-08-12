<div align="center">

# 🟢 NEXA AIR

### AI-Powered Real-Time Hand Gesture Tracking for Android

<p>
  <strong>Computer Vision • Hand Tracking • Gesture Recognition • Real-Time Visualization</strong>
</p>

<p>
  An Android computer-vision application that transforms a smartphone camera
  into a real-time hand tracking and gesture recognition system.
</p>

<br>

<img src="https://img.shields.io/badge/Platform-Android-3DDC84?style=for-the-badge&logo=android&logoColor=white"/>
<img src="https://img.shields.io/badge/Language-Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white"/>
<img src="https://img.shields.io/badge/UI-XML-1572B6?style=for-the-badge&logo=xml&logoColor=white"/>
<img src="https://img.shields.io/badge/Camera-CameraX-4285F4?style=for-the-badge&logo=google&logoColor=white"/>
<img src="https://img.shields.io/badge/Computer%20Vision-MediaPipe-8E75B2?style=for-the-badge&logo=google&logoColor=white"/>

<br><br>

<img src="https://img.shields.io/badge/Hand%20Tracking-21%20Landmarks-38F27F?style=for-the-badge"/>
<img src="https://img.shields.io/badge/Gestures-5%20Recognized-38F27F?style=for-the-badge"/>
<img src="https://img.shields.io/badge/Real--Time-Tracking-00C853?style=for-the-badge"/>
<img src="https://img.shields.io/badge/ViewBinding-Enabled-4CAF50?style=for-the-badge"/>
<img src="https://img.shields.io/badge/Storage-SharedPreferences-FF9800?style=for-the-badge"/>

<br><br>

<img src="https://img.shields.io/badge/Custom%20Overlay-HandOverlayView-00BCD4?style=for-the-badge"/>
<img src="https://img.shields.io/badge/FPS-Monitoring-2196F3?style=for-the-badge"/>
<img src="https://img.shields.io/badge/Latency-Monitoring-2196F3?style=for-the-badge"/>
<img src="https://img.shields.io/badge/Confidence-Scoring-9C27B0?style=for-the-badge"/>
<img src="https://img.shields.io/badge/Status-Active%20Development-success?style=for-the-badge"/>

<br><br>

</div>

---

# 🚀 Project Overview

**NEXA AIR** is an Android-based artificial intelligence and computer-vision application designed to detect, track, and recognize human hand gestures in real time using a smartphone camera.

The application combines **CameraX**, **MediaPipe Hand Landmarker**, custom landmark-based gesture classification, and a custom Android visualization layer to transform a smartphone into a real-time hand-tracking system.

NEXA AIR currently recognizes five fundamental gestures:

- ✋ Open Palm
- ✊ Fist
- ☝️ Point
- 👍 Thumbs Up
- ✌️ Peace

The system also provides `UNCERTAIN` and `NONE` recognition states when a supported gesture cannot be confidently determined.

> **NEXA AIR combines Android development, artificial intelligence, computer vision, camera processing, gesture recognition, real-time visualization, and modular application architecture into a single mobile application.**

---

# 🎯 Project Purpose

NEXA AIR was created to explore practical applications of **AI-powered computer vision on Android devices**.

Instead of relying only on traditional touch-based interaction, the project uses the smartphone camera to understand the structure and configuration of a user's hand.

The current system can:

- Detect a user's hand
- Track 21 hand landmarks
- Analyze landmark relationships
- Recognize predefined gestures
- Calculate gesture confidence
- Visualize the tracked hand
- Monitor FPS
- Measure processing latency
- Display real-time tracking status
- Allow users to customize tracking behavior

The architecture is intentionally modular so that the computer-vision pipeline can be extended with additional gestures and interaction systems in future versions.

---

# 🧠 Computer Vision Pipeline

NEXA AIR uses a modular processing pipeline:

```text
┌──────────────────┐
│     CameraX      │
│  Camera Frames   │
└────────┬─────────┘
         ↓
┌──────────────────┐
│  CameraManager   │
│ Camera Lifecycle │
└────────┬─────────┘
         ↓
┌──────────────────────┐
│ HandLandmarkerHelper │
│    MediaPipe AI      │
└────────┬─────────────┘
         ↓
┌──────────────────────┐
│   21 Hand Landmarks  │
└────────┬─────────────┘
         ↓
┌──────────────────────┐
│  GestureClassifier   │
│ Landmark Analysis    │
└────────┬─────────────┘
         ↓
┌──────────────────────┐
│    GestureResult     │
│ Gesture + Confidence │
└────────┬─────────────┘
         ↓
┌────────────────────────────┐
│ GestureTrackingActivity    │
│       + HandOverlayView     │
└────────────────────────────┘

# NEXA AIR

### AI Hand Gesture Tracking & Computer Vision Application

> A real-time Android computer-vision application that transforms a smartphone camera into an intelligent hand-tracking and gesture-recognition platform using CameraX and MediaPipe Hand Landmarker.

![Platform](https://img.shields.io/badge/Platform-Android-green)
![Language](https://img.shields.io/badge/Language-Java-orange)
![UI](https://img.shields.io/badge/UI-XML-blue)
![Camera](https://img.shields.io/badge/Camera-CameraX-blue)
![Computer Vision](https://img.shields.io/badge/Computer%20Vision-MediaPipe-purple)
![Hand Tracking](https://img.shields.io/badge/Hand%20Tracking-21%20Landmarks-brightgreen)
![Gestures](https://img.shields.io/badge/Gestures-5-success)
![ViewBinding](https://img.shields.io/badge/ViewBinding-Enabled-informational)
![Storage](https://img.shields.io/badge/Storage-SharedPreferences-yellow)
![Activities](https://img.shields.io/badge/Activities-6-blueviolet)
![Status](https://img.shields.io/badge/Status-Active%20Development-success)
![Version](https://img.shields.io/badge/Version-v1.0-yellow)

---

# 📖 About NEXA AIR

NEXA AIR is a professional Android **AI and computer-vision application** designed to detect, track, and recognize human hand gestures in real time using a smartphone camera.

The application combines **CameraX**, **MediaPipe Hand Landmarker**, custom gesture-classification logic, real-time performance monitoring, and a custom hand-tracking overlay to create an interactive computer-vision experience directly on Android.

NEXA AIR currently recognizes five fundamental hand gestures:

- Open Palm
- Fist
- Point
- Thumbs Up
- Peace

The project has been designed with a modular architecture so that the existing hand-tracking foundation can later be expanded into a larger gesture-based human-computer interaction platform.

---

# 🧠 Project Concept

Traditional mobile applications primarily depend on touch input, physical buttons, or other conventional interaction methods.

NEXA AIR explores a different approach by using the smartphone camera as a **computer-vision input device**.

The application continuously processes camera frames, detects the user's hand, extracts its 21 landmark points, analyzes the landmark configuration, classifies the gesture, and provides visual feedback through the application interface.

The overall concept is:

```text
Smartphone Camera
       ↓
   CameraX
       ↓
 Camera Frame
       ↓
MediaPipe Hand Landmarker
       ↓
  21 Hand Landmarks
       ↓
 GestureClassifier
       ↓
   GestureResult
       ↓
 Tracking UI
       ↓
HandOverlayView + Live Metrics

# 🖐️ NEXA AIR

### AI Hand Gesture Tracking & Computer Vision Application

> An Android-based AI computer-vision application that uses CameraX and MediaPipe Hand Landmarker to detect, track, and recognize hand gestures in real time.

![Platform](https://img.shields.io/badge/Platform-Android-green)
![Language](https://img.shields.io/badge/Language-Java-orange)
![UI](https://img.shields.io/badge/UI-XML-blue)
![Camera](https://img.shields.io/badge/Camera-CameraX-4285F4)
![Computer Vision](https://img.shields.io/badge/Computer%20Vision-MediaPipe-8E75B2)
![Hand Tracking](https://img.shields.io/badge/Hand%20Tracking-21%20Landmarks-00A67E)
![Gestures](https://img.shields.io/badge/Gestures-5%20Recognized-success)
![ViewBinding](https://img.shields.io/badge/ViewBinding-Enabled-informational)
![Storage](https://img.shields.io/badge/Storage-SharedPreferences-orange)
![Status](https://img.shields.io/badge/Status-In%20Active%20Development-success)
![Version](https://img.shields.io/badge/Version-v1.0-yellow)

---

# 📖 About NEXA AIR

NEXA AIR is a premium Android artificial intelligence and computer-vision application designed to detect, track, and recognize human hand gestures in real time using a smartphone camera.

The application combines **Java, XML, CameraX, MediaPipe Hand Landmarker, landmark-based gesture classification, custom hand visualization, and real-time performance monitoring** to transform an Android smartphone into an intelligent hand-tracking system.

The current version recognizes five primary hand gestures:

- 🖐️ Open Palm
- ✊ Fist
- ☝️ Point
- 👍 Thumbs Up
- ✌️ Peace

The recognition system also supports `UNCERTAIN` and `NONE` states when a supported gesture cannot be confidently determined.

NEXA AIR provides real-time gesture confidence, FPS, processing latency, tracking status, hand landmarks, calibration, tracking controls, and a custom visual overlay that allows users to see the computer-vision process while it is running.

The project is built with a modular architecture so that additional gestures and advanced gesture-based interaction capabilities can be introduced in future versions.

---

# ✨ Features

## 🖐️ AI Hand Tracking

- Real-time hand detection
- 21-point hand landmark detection
- Continuous camera-frame processing
- Real-time landmark updates
- Hand tracking visualization
- Tracking status feedback
- Camera preview integration

## ✋ Gesture Recognition

NEXA AIR currently recognizes five primary gestures:

- 🖐️ Open Palm
- ✊ Fist
- ☝️ Point
- 👍 Thumbs Up
- ✌️ Peace

### Recognition States

- `UNCERTAIN` — used when a hand is detected but the landmark configuration cannot be confidently classified.
- `NONE` — used when no supported gesture or valid recognition state is detected.

## 📊 Real-Time Tracking Metrics

The Gesture Tracking screen provides:

- Detected gesture
- Gesture confidence percentage
- FPS monitoring
- Processing latency
- Tracking status
- Tracking sensitivity information
- Live hand landmark visualization

## 🎯 Camera & Hand Calibration

The calibration system helps users prepare the tracking environment through:

- Hand positioning verification
- Hand visibility checks
- Lighting condition checks
- Tracking readiness
- Camera availability
- Visual calibration guidance

## ⚙️ Tracking Controls

Users can customize the tracking experience through:

- Landmark visibility
- Hand mask visibility
- Confidence display
- FPS display
- Camera mirroring
- Tracking sensitivity

## 📚 Gesture Library

The Gesture Library provides information about all five supported gestures through dedicated gesture cards, icons, descriptions, and visual presentation.

## 💾 Persistent Settings

Tracking preferences are stored locally using **SharedPreferences** through the application's `Prefs` utility.

This allows user configuration to remain available between application launches.

---

# 🎨 Premium User Interface

NEXA AIR follows a professional dark AI/computer-vision design language built around its green visual identity.

## 🎨 Visual Design

- 🌑 Dark futuristic interface
- 🟢 NEXA AIR green visual identity
- ✨ Glowing tracking elements
- 🟢 Green hand skeleton visualization
- 🔘 Glowing landmark points
- 🖐️ Translucent hand mask
- 📦 Rounded professional cards
- 🎛️ Modern controls
- 📊 Real-time status indicators
- 🎬 Smooth UI animations
- 📱 Responsive Android layouts
- 🧭 Clear information hierarchy

### Core Colors

```text
Background
#070B0F

Primary Green
#38F27F

Dark Green
#1DB954

Light Green
#79FFA9

White
#FFFFFF

Secondary Text
#B0B6BE

```

# 🏗 Architecture

Here we gooo

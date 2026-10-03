# 🏝️ HTMLHomeScreen — Dynamic Island for iOS 15

[![iOS Version](https://img.shields.io/badge/iOS-15.0%20--%2015.7.x-000000?style=for-the-badge&logo=apple&logoColor=white)](https://apple.com)
[![Architecture](https://img.shields.io/badge/Arch-arm64%20(Rootless)-FF2D55?style=for-the-badge&logo=iphone&logoColor=white)](https://dopamine.jailbreak.me)
[![License](https://img.shields.io/badge/License-MIT-007AFF?style=for-the-badge)](LICENSE)
[![Build Status](https://img.shields.io/badge/Status-v2.9.0%20Stable-34C759?style=for-the-badge)]()

**HTMLHomeScreen** is an interactive, native-style Dynamic Island tweak built specifically for rootless iOS 15 jailbreaks (Dopamine, Palera1n). It transforms the static notch or top status bar into a living, responsive UI element complete with live audio controls, active call interfaces, system alerts, privacy indicators, and deep per-element geometry customization.

---

## ✨ Features at a Glance

* **🎵 Live Media Player:** Real-time cover art, animated pink equalizer, timeline progress, and interactive playback controls.
* **📞 Native Call Banner:** Incoming call pop-ups with **Accept** / **Decline** options and live duration counters for ongoing calls.
* **🌙 Focus Mode Integration:** Instant visual feedback with custom icons and accent colors for all stock Focus profiles.
* **🛡️ Live Privacy Dots:** Real-time orange (Mic) and green (Camera) indicators with running timers, featuring a option to hide stock iOS indicators.
* **💳 Apple Pay & System Alerts:** Smooth spring animations for Apple Pay authentication, charging states, and silent switch toggles.
* **🔀 Split Multi-Tasking:** Displays two simultaneous background activities using a primary capsule and a secondary mini-bubble.
* **🎛️ Complete Size Control:** Independent width and height sliders for every animation mode so you can tailor the island to your exact display scale.

---

## 📷 Feature Breakdown & UI Specs

| Feature | Compact View | Expanded View |
| :--- | :--- | :--- |
| **Music Player** | 173×38 pill with album art & live pink waveform | 367px panel with timeline bar, title, artist, and full media buttons |
| **Active Calls** | Green pill with live timer & waveform | Wide capsule with caller initials, Accept 🟩 and Decline 🟥 actions |
| **Timers** | Mini timer icon with countdown | Full control panel with **Pause** ⏸️ and **Cancel** ❌ buttons |
| **Focus Modes** | Animated moon icon & profile label | Auto-collapsing badge displaying active mode settings |
| **Privacy Indicators** | Live 🟢 Mic / 🟢 Cam dot with timer | Quick status pop-up for active recording apps |

---

## 🛠️ Installation & Setup

### Prerequisites
* **Jailbreak:** Rootless (Dopamine / Palera1n)
* **Architecture:** `arm64`
* **Dependencies:** `PreferenceLoader`

### Installation Steps
1. Download the latest `.deb` package from the [Releases](../../releases) tab.
2. Open the package in **Sileo**, **Zebra**, or **Filza**.
3. Tap **Install** and perform a **Respring**.
4. Navigate to `Settings > HTMLHomeScreen` to configure your layout and toggle features.

---

## 📦 Release History

<details>
<summary><b>🏷️ v2.9.0 — Advanced UI, Privacy & Size Customization</b> <i>(Latest)</i></summary>

* 🌙 **Focus Mode Indicators:** Animated moon icon and dynamic labels for **Do Not Disturb**, **Sleep**, **Work**, **Personal**, **Driving**, **Fitness**, **Reading**, **Mindfulness**, and **Gaming**.
* 🛡️ **Privacy Indicators:** Real-time **Orange Dot** 🟢 (Mic) and **Green Dot** 🟢 (Camera) with active duration timers + stock dot hider.
* 🎙️ **Voice Recorder Fallback:** Automatic fallback launch to **Voice Memos** if direct SpringBoard capture is restricted.
* 💳 **Apple Pay Interface:** Experimental card pop-up with pulsing wave animation and a **Done** checkmark state.
* ⚡ **Volume HUD Fix:** Increased detection frequency to **~25 Hz** to eliminate visual stock HUD flashing.
* 🎛️ **Granular Size Sliders:** Independent width/height scale controls for:
  * 🔓 Lock / Unlock
  * 🔊 Ringer / Silent / Volume
  * 🌙 Focus Modes
  * 💳 Apple Pay
  * 🎙️️ Microphone / Camera
  * ⚡ Flashlight, AirDrop, Screen Recording & Charging
</details>

<details>
<summary><b>🏷️ v2.5.0 — Native Architecture Overhaul</b></summary>

* 🎵 **Interactive Music Player:** Rebuilt layout using exact Figma component specifications.
* 📞 **Active Call Banners:** Added wide capsule notifications with functional Accept/Decline actions.
* ⏱️ **Timer UI Fixes:** Resolved background thread crashes when fetching active timers.
* 🔀 **Priority Multi-Tasking:** Added dual-event split bubbles for simultaneous app activities.
</details>

<details>
<summary><b>🏷️ v2.1.0 — Initial Dynamic Island Release</b></summary>

* ⚡ **Core Engine:** Morphing notch animations with smooth spring curves.
* 🔋 **Basic Status Tracking:** Support for charging, silent mode, and basic media detection.
</details>

---

## 🐛 Troubleshooting & Debugging

If you encounter issues such as missing artwork or UI glitches, check the local debug log:

```bash
/var/jb/var/mobile/Library/HTMLHomeScreen/debug.log

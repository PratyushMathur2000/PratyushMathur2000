<div align="center">
  <img src="https://mindsnap-3c915.web.app/assets/images/app_icon.png" alt="MindSnap Logo" width="150"/>
  <h1>MindSnap — Blink and You Lose.</h1>
  <p><strong>A Premium Hyper-Casual Puzzle Game</strong></p>

  <a href="https://play.google.com/store/apps/details?id=com.mindsnap.game"><img src="https://img.shields.io/badge/Google_Play-Available-green?style=for-the-badge&logo=google-play" alt="Google Play" /></a>
  <a href="https://mindsnap-3c915.web.app/"><img src="https://img.shields.io/badge/Web_App-Live-blue?style=for-the-badge&logo=firebase" alt="Web App Live" /></a>
  <img src="https://img.shields.io/badge/Android_15-Ready-success?style=for-the-badge&logo=android" alt="Android 15 Ready" />
</div>

<br>

MindSnap is a high-octane, brain-training hyper-casual mobile game designed to test reflexes, memory, and cognitive processing under intense pressure. Built entirely from scratch using a bespoke **Vanilla JS/HTML5** engine and wrapped in **Capacitor**, MindSnap delivers a native-grade, fluid 60FPS experience without the overhead of heavy game engines like Unity.

This project demonstrates end-to-end product ownership: from core game design and UI/UX to advanced native ad integrations, performance optimization, and Google Play Store deployment.

---

## 🚀 Key Highlights

*   **Bespoke Game Engine:** 100% custom architecture utilizing the DOM and HTML5 Canvas. Zero heavy frameworks. Blazing fast.
*   **Capacitor Native Bridge:** Compiled to a native Android APK/AAB targeting Android 15 (API 35), fully utilizing edge-to-edge layouts and native plugins (Haptics, Status Bar, App Tracking).
*   **Robust Monetization:** Production-grade AdMob Mediation integration (Interstitials & Rewarded Video) with highly resilient fallback layers, background caching, and game-state recovery logic.
*   **Dynamic Theme System:** "Pure Dynamic" UI architecture relying on CSS variables to instantly remap the entire app's aesthetics (e.g., Neon Prime, Sunforge, Cyber Grid) while keeping core gameplay colors immutable for fairness.
*   **Firebase Ecosystem:** Integrated Firebase Analytics for precise telemetry and Firebase Hosting for the web distribution.

---

## 🎮 The Game Modes

MindSnap features four distinct mini-games, each pushing a different cognitive threshold:

1.  🔴 **Color Chaos (Stroop Effect Engine)**
    A brutal test of cognitive flexibility. Players must identify shapes based on contradictory text/color prompts. The engine scales dynamically across 5 tiers of shape sizes, negative logic ("TAP NOT BLUE"), and chaotic combinations.
2.  ⚡ **Reverse Reflex (Pattern Recognition)**
    A high-speed directional challenge. Players swipe or tap based on rapidly changing signals, battling "Double Reverse" modifiers and trick prompts as the speed curve exponentially intensifies.
3.  🧠 **Memory Flash (Spatial Recall)**
    A high-stakes spatial memory test. Memorize randomly generated grids of shapes before they disappear, then tap the correct sequences. Features adaptive difficulty and an intricate hint economy.
4.  🔥 **Triple Threat (The Ultimate Test)**
    A chaotic, rapid-fire blend of all three modes, seamlessly shifting mechanics mid-round to keep the player completely off-balance.

---

## 🛠️ Technical Architecture

### 1. The Core Engine (`core.js` & `app.js`)
*   **State Machine:** Centralized `App` manager handling global lifecycle, UI transitions, audio context resuming, and pausing background logic.
*   **PuzzleForge Particle System:** A lightweight, custom-built particle engine rendering 60FPS explosive bursts matched to the hex colors of tapped objects or the active UI theme.
*   **Daily Challenges:** A date-seeded procedural generator crafting 3 unique challenges every 24 hours (e.g., *Speed Demon*, *Survivor*), driving daily retention.

### 2. Monetization & Ad Reliability (`ads.js`)
*   **Auto-Preloading Cache:** Instantly fetches the next ad in the background when an ad is dismissed or fails, eliminating "Ad Timeout" skips and maximizing impressions.
*   **State Guards & Audio Recovery:** Solves common HTML5/Native bridge issues by gracefully pausing the game loop, muting the Web Audio API context during interstitials, and resuming seamlessly without race conditions.
*   **Reward Economy:** "Revive" systems, 2x Score Boosters, and an intricate item economy (Time Freezes, Shields) deeply woven into Rewarded Video hooks.

### 3. Styling & "The Juice" (`style.css`)
*   **Glassmorphism & Micro-Interactions:** High-end frosted glass aesthetic layered with custom cubic-bezier animations for satisfying, premium tactile feedback.
*   **Responsive & Safe-Area Aware:** Complete support for Android 15's edge-to-edge display, utilizing `safe-area-inset` to prevent overlaps with modern gesture navigation.

---

## 📈 Impact & Developer Takeaways

Building MindSnap from the ground up served as a masterclass in:
1.  **Engine Independence:** Proving that high-performance, polished mobile games can be built with pure web technologies.
2.  **Native Resiliency:** Creating bulletproof ad integration logic that survives unexpected plugin failures, background state changes, and OS-level interruptions.
3.  **UI/UX Polish:** Mastering the "game feel" through perfectly timed screen-shakes, particle effects, and typography consistency.

---
<div align="center">
  <i>Portfolio piece showcasing production-ready mobile game development, front-end architecture, and monetization strategy.</i>
</div>

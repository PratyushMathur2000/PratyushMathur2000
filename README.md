# Hi, I'm Pratyush Mathur 👋

<div align="center">
  <h3>Founder & Lead Developer at MindSnap Studios</h3>
  <p><strong>Building High-Impact Mobile Applications, Grounded AI Systems & Interactive Digital Products</strong></p>

  <a href="https://mindsnapstudios.com"><img src="https://img.shields.io/badge/Website-mindsnapstudios.com-4338ca?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Studio Website" /></a>
  <a href="mailto:mindsnapstudios.contact@gmail.com"><img src="https://img.shields.io/badge/Email-mindsnapstudios.contact@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Business Email" /></a>
  <a href="https://github.com/PratyushMathur2000"><img src="https://img.shields.io/badge/GitHub-PratyushMathur2000-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub Profile" /></a>
  <img src="https://img.shields.io/badge/Location-Mumbai%2C%20India-10B981?style=for-the-badge&logo=googlemaps&logoColor=white" alt="Location" />
</div>

<br>

Welcome to my GitHub profile! I am a full-stack engineer, AI systems builder, and mobile developer specializing in taking ambitious software concepts from architectural design to high-volume production releases.

Whether engineering deterministic AI pipelines that eliminate hallucinations, shipping responsive 60FPS mobile apps to the Google Play Store, or orchestrating multi-tier edge microservices on Cloudflare and Firebase, I focus on clean architecture, relentless reliability, and polished user experiences.

---

## 🚀 Featured Open-Source Systems & AI Repositories

Direct links to open-source systems, algorithmic frameworks, and production tools:

### ⭐ [Meeting Assistant](https://github.com/PratyushMathur2000/meeting-assistant)
> **Real-time Q&A co-pilot for high-stakes meetings, panels, and live Q&A sessions.**
* **Tech Stack:** Python 3.10–3.13, OpenAI Whisper (CUDA / CPU), Google Gemini API, Windows WASAPI Loopback
* **Architecture Highlights:**
  * **Zero-Retrieval Guessing:** Sends verified documents directly within the prompt context window rather than relying on brittle semantic vector chunking that selects the wrong paragraph.
  * **Live Red Hallucinated-Figure Detection:** Automatically checks every number and statistic against source documents; ungrounded figures are dynamically flagged in red with a `⚠ NOT IN YOUR FILES` warning.
  * **Contiguous Turn Capture:** Intelligently listens to entire speaking turns (up to 35s windows) without fragmenting mid-sentence when speakers pause.
* **Explore Repo:** [`PratyushMathur2000/meeting-assistant`](https://github.com/PratyushMathur2000/meeting-assistant)

---

### ⭐ [ClaimPulse Simulation](https://github.com/PratyushMathur2000/claimpulse-simulation)
> **High-performance verified-evidence motor insurance claims orchestration simulator.**
* **Tech Stack:** Vanilla JavaScript (ES6+), HTML5, CSS3, SVG Rendering Engine, Zero External Dependencies
* **Architecture Highlights:**
  * **5-Layer Deterministic Decision Tree:** Models Hard Gate, Fraud Ring Detection ($\ge 0.35$ SIU routing), Parts Benchmark, Policy RAG, and statutory IRDAI guidelines (> ₹50k surveyor caps).
  * **Handcrafted SVG Chart Suite:** Custom-built zero-dependency SVG visualization engine (waterfall, cashflow, tornado, bullet, meter, and contribution charts).
  * **Grounded Intelligence Assistant:** Bottom-right interactive assistant deeply grounded in complex actuarial and operational models with clickable navigation triggers.
* **Explore Repo:** [`PratyushMathur2000/claimpulse-simulation`](https://github.com/PratyushMathur2000/claimpulse-simulation)

---

### ⭐ [TwinPulse Asset Prognosis & Digital Twin Framework](https://github.com/PratyushMathur2000/Twin-Pulse-ML-Based-Digital-Twin-Framework-for-AI-Driven-Asset-Prognosis)
> **Industrial predictive maintenance and digital twin framework for equipment degradation modeling.**
* **Tech Stack:** Python, Streamlit, Scikit-learn, Plotly, Pandas, NumPy
* **Architecture Highlights:**
  * Multi-page analytical sandbox featuring Fleet Overview, Digital Twin simulation, Production Simulator, and an AI Diagnostic Agent.
  * Predictive degradation curves modeling Remaining Useful Life (RUL) to eliminate costly industrial downtime.
* **Explore Repo:** [`PratyushMathur2000/Twin-Pulse...`](https://github.com/PratyushMathur2000/Twin-Pulse-ML-Based-Digital-Twin-Framework-for-AI-Driven-Asset-Prognosis) · [Detailed Showcase](./Python_Analytics_Showcase.md)

---

## 📱 MindSnap Studios — Production Apps & Digital Products

Consumer mobile apps and production web platforms published through **MindSnap Studios**:

```
                                  [ MindSnap Studios ]
                               (https://mindsnapstudios.com)
                                             │
      ┌──────────────────────────────┬───────┴──────────────────────┬──────────────────────────────┐
      ▼                              ▼                              ▼                              ▼
[ Before You Sign ]             [ MindSnap ]                 [ PuzzleForge ]                 [ Poise / Prep ]
AI Contract Analyzer        Cognitive Reflex Game          Modular Jigsaw Game           AI Interview Suite
(Android / Cloudflare)      (Capacitor / Android)         (Capacitor / Android)         (Android / Jetpack)
```

### 🛡️ [Before You Sign — AI Legal Document & Contract Risk Analyzer](https://mindsnapstudios.com/before-you-sign/)
*Understand any contract before you sign it. Plain-English summaries and red-flag alerts.*
* **Tech Stack:** Kotlin, Jetpack Compose, Material Design 3, Android 16 (API 36), Cloudflare Worker, Google Gemini 3.x Flash Cascade
* **Capabilities:** Multimodal document ingestion (text, camera OCR, multi-page PDF). Detects predatory clauses (IP grabs, hidden auto-renewals, non-competes, one-sided indemnity), scores overall risk, and drafts polite pushback negotiation emails.
* **Architecture:** Zero-trust Cloudflare Worker reverse proxy isolates API credentials and implements automatic fallback across Gemini 3.7 / 3.6 / 3.5 Flash models.
* **Links:** **[Detailed Showcase](./Before_You_Sign_Showcase.md)** · **[Product Page](https://mindsnapstudios.com/before-you-sign/)** · **[Privacy & Legal](https://mindsnapstudios.com/before-you-sign/privacy-policy.html)**

### ⚡ [MindSnap — Reflex & Brain-Training Mobile Game](https://mindsnapstudios.com/play/)
*Blink and you lose. A high-octane hyper-casual mobile game testing reflexes under pressure.*
* **Tech Stack:** Vanilla JavaScript, HTML5 Canvas, Capacitor Native Bridge, Firebase Analytics & Hosting, Android 15 Ready
* **Game Modes:** Color Chaos (Stroop Effect), Reverse Reflex (Pattern Recognition), Memory Flash (Spatial Recall), and Triple Threat.
* **Highlights:** Bespoke 60FPS particle engine, CSS variable theme swaps, and production-grade resilient AdMob mediation integration.
* **Links:** **[Detailed Showcase](./MindSnap_Showcase.md)** · **[Play Web Demo](https://mindsnapstudios.com/play/)** · **[Google Play Store](https://play.google.com/store/apps/details?id=com.mindsnap.game)**

### 🧩 [PuzzleForge — Modular Jigsaw Puzzle Experience](https://mindsnapstudios.com/puzzleforge/)
*Tactile, polished mobile jigsaw puzzles with fluid piece mechanics.*
* **Tech Stack:** Vanilla JavaScript, HTML5 Canvas slicing engine, Capacitor, CSS Grid/Flexbox
* **Game Modes:** Classic, Zen, Chaos, and Blur modes with curated, high-resolution puzzle galleries.
* **Highlights:** 10px scroll-aware threshold distinguishing page navigation from piece dragging, memory initialization guards, and isolated game-state management.
* **Links:** **[Detailed Showcase](./PuzzleForge_Showcase.md)** · **[Play Web Demo](https://mindsnapstudios.com/puzzleforge/)** · **[Google Play Store](https://play.google.com/store/apps/details?id=com.puzzleforge.game)**

### 🌐 [MindSnap Studios Official Website](https://mindsnapstudios.com)
*The studio's public front door, game hub, and legal disclosure portal.*
* **Tech Stack:** Modern Vanilla HTML5, CSS3, ES6 JavaScript, Firebase Hosting, Web3Forms, Schema.org JSON-LD
* **Highlights:** Softened light theme with dark About band, mobile hamburger navigation, self-hosted Outfit & JetBrains Mono typography, search-engine indexing, and strict CSP headers.
* **Links:** **[Visit mindsnapstudios.com](https://mindsnapstudios.com)**

---

## 🧪 In-Development & Commercial Showcase Projects

* 🎯 **Poise (AI Interview Companion):** Full-suite career training app with on-device resume parsing, 6-category ATS taxonomy, 16 domain curriculum modules across 6 industries, and an interactive voice-enabled AI mock interviewer. *(Android / Compose / Gemini)*
* ⚔️ **Grid Clash:** Tactical turn-based 1v1 grid battler with online matchmaking, responsive canvas rendering, and ranking ladders. *(Capacitor / HTML5 / Firebase)*
* 🔍 **[The Enigma Archives](./Enigma_Archives_Showcase.md):** Co-op multiplayer 2.5D detective mystery game built in Unity featuring synchronized evidence notebooks, dynamic clue voting, and narrative state management. *(Unity / C# / Netcode)*
* 🏢 **[Acme EMS (Enterprise Management System)](./EMS_Showcase.md):** Centralized HR and field operations platform with 6-level Role-Based Access Control, automated attendance, and real-time sales team GPS tracking. *(HTML5 / JS / Capacitor / Firebase)*
* 🛏️ **[SleepOnly — Mattress Web](./Mattress_Web_Showcase.md):** D2C e-commerce experience featuring custom slide-out cart state management and an embedded AI consultation assistant. *(Vanilla JS / Vite)*

---

## 🛠️ Technical Arsenal & Core Skills

| Category | Technologies & Tools |
| :--- | :--- |
| **Languages** | Kotlin, Python, JavaScript (ES6+), TypeScript, C#, SQL, HTML5, CSS3 |
| **AI & LLM Orchestration** | Google Gemini API (3.x Cascade), OpenAI Whisper, Grounded Context Engineering, Prompt Architecture, Hallucination Verification |
| **Mobile & Cross-Platform** | Android Jetpack Compose, Material Design 3, Capacitor (Android & iOS), Progressive Web Apps (PWA) |
| **Backend, Edge & Cloud** | Cloudflare Workers, Firebase (Firestore, Auth, Hosting, Analytics), Node.js, RESTful APIs |
| **Game Development** | Unity (C#, Unity.Netcode), Bespoke HTML5 Canvas 2D Engines, 60FPS Game Loops, AdMob Mediation |
| **Architecture & Tools** | Clean Architecture, Unidirectional Data Flow (UDF), Git, GitHub CLI, Linux/Windows Shell, Gradle, Vite |

---

## 📬 Let's Connect & Collaborate

I am always interested in discussing new opportunities, high-impact consulting, innovative app development, or game publishing:

* 🌐 **Official Studio Website:** [mindsnapstudios.com](https://mindsnapstudios.com)
* ✉️ **Primary Business Inquiries:** [mindsnapstudios.contact@gmail.com](mailto:mindsnapstudios.contact@gmail.com)
* 💼 **GitHub:** [@PratyushMathur2000](https://github.com/PratyushMathur2000)
* 📍 **Base:** Mumbai, Maharashtra, India

---

<div align="center">
  <sub>© 2026 Pratyush Mathur · MindSnap Studios. Crafted with precision and engineered for performance.</sub>
</div>

<div align="center">
  <h1>🛡️ Before You Sign — AI Contract & Legal Risk Analyzer</h1>
  <p><strong>Know What You're Agreeing to Before You Commit</strong></p>

  <a href="https://mindsnapstudios.com/before-you-sign/"><img src="https://img.shields.io/badge/MindSnap_Studios-Official_Product-indigo?style=for-the-badge&logo=firebase" alt="MindSnap Studios" /></a>
  <img src="https://img.shields.io/badge/Android_16-API_36_Ready-success?style=for-the-badge&logo=android" alt="Android 16 API 36 Ready" />
  <img src="https://img.shields.io/badge/Jetpack_Compose-Material_3-blue?style=for-the-badge&logo=jetpackcompose" alt="Jetpack Compose" />
  <img src="https://img.shields.io/badge/Backend-Cloudflare_Worker-F38020?style=for-the-badge&logo=cloudflare" alt="Cloudflare Worker" />
  <img src="https://img.shields.io/badge/AI_Engine-Google_Gemini_3.x-4285F4?style=for-the-badge&logo=google" alt="Google Gemini" />
</div>

<br>

**Before You Sign** is a production Android application engineered to protect freelancers, independent contractors, creators, and small business operators from predatory contract clauses. By turning dense, adversarial legal jargon into clear, plain-English summaries, it identifies hidden liabilities, non-compete traps, and unconscionable indemnification requirements in seconds.

Built natively using modern **Kotlin & Jetpack Compose (Material 3)**, targeting **Android 16 (API 36)**, and backed by a zero-trust **Cloudflare Worker edge reverse proxy** executing a high-resiliency **Google Gemini 3.x Flash cascade**, Before You Sign demonstrates enterprise-grade mobile architecture, strict zero-server data retention, and production-tested GenAI orchestration.

---

## 🚀 Key Highlights & Capabilities

* **Multimodal Document Ingestion:** Analyzes contracts via plain text paste, on-device OCR camera captures, or multi-page PDF document uploads.
* **Granular Red-Flag Analysis:** Automatically flags predatory clauses across six critical risk dimensions:
  1. *Unilateral IP & Copyright Grabs* (e.g., claiming rights to pre-existing or outside work)
  2. *Hidden Auto-Renewal & Fee Traps* (e.g., silent billing roll-overs, aggressive liquidated damages)
  3. *Overbroad Non-Compete & Non-Solicit Restrictions* (e.g., multi-year nationwide bans)
  4. *One-Sided Indemnification & Unlimited Liability* (e.g., shifting client defense costs onto contractors)
  5. *Harsh Termination Penalties* (e.g., termination without cause with zero compensation)
  6. *Missing Standard Safeguards* (e.g., lack of cure periods, absence of mutual confidentiality)
* **Actionable Negotiation Counter-Drafts:** Generates polite, professional counter-proposals and suggested replacement wording tailored for pushback without damaging client relationships.
* **Interactive AI Contract Q&A:** Allows users to ask specific follow-up questions directly about the uploaded agreement with prompt grounding.
* **Strict Privacy by Architecture:** Zero document persistence on edge servers. Scans remain strictly on-device by default, with optional encrypted cloud backup via Firebase Firestore for multi-device sync.

---

## 🛠️ Technical Architecture

```
[ Android Native Client ]
  ├─ Kotlin + Jetpack Compose + Material 3 (Edge-to-Edge, Android 16 API 36)
  ├─ On-Device Document Parser & PDF Ingestion
  ├─ StateFlow & Coroutines Reactive UDF (Unidirectional Data Flow)
  └─ Encrypted SharedPreferences & Room / Local Cache
             │
             │ HTTPS + X-Proxy-Secret + Firebase App Check
             ▼
[ Cloudflare Worker Edge Reverse Proxy ] (proxy/src/index.js)
  ├─ Edge rate-limiting & payload validation
  ├─ Secure Gemini API key isolation (Zero client exposure)
  ├─ CORS & CSP security enforcement
  └─ Resilient Cascade Orchestrator:
        ├─ Tier 1: Gemini 3.7 Flash
        ├─ Tier 2: Gemini 3.6 Flash
        └─ Tier 3: Gemini 3.5 Flash / Flash Lite Fallback
             │
             ▼
[ Google Gemini AI Models ]
  └─ Structured JSON Output schema enforcement & hallucination minimization
```

### 1. Zero-Trust Edge Reverse Proxy (`proxy/src/index.js`)
Client applications never communicate directly with upstream AI providers. All requests flow through a dedicated Cloudflare Worker edge function that:
- Terminates TLS at the closest global edge node for sub-50ms latency.
- Validates the private `X-Proxy-Secret` header and optional Firebase App Check tokens.
- Inserts encrypted server-side secrets (`GEMINI_API_KEY`), ensuring client decompilation yields zero credential leaks.
- Manages an automated **model cascade**: if primary model rate-limits or transient upstream hiccups occur, the proxy silently cascades across verified Gemini tiers before returning a unified, validated JSON response.

### 2. Modern Android Native Stack
- **Declarative UI:** 100% Jetpack Compose using Material Design 3, dynamic color theming, and full support for predictive back gestures and 120Hz smooth scrolling.
- **Strict Architecture:** Clean Architecture with distinct `domain`, `data`, and `feature` modules adhering to single-responsibility and dependency inversion principles.
- **Resilient Offline Mode:** Locally caches past scan summaries and risk verdicts so users can consult their audit history without active connectivity.

---

## 🌐 Live Product & Verification

* **Studio Homepage:** [https://mindsnap-3c915.web.app/](https://mindsnap-3c915.web.app/) *(or [mindsnapstudios.com](https://mindsnapstudios.com))*
* **App Product Hub:** [https://mindsnap-3c915.web.app/before-you-sign/](https://mindsnap-3c915.web.app/before-you-sign/)
* **Privacy Policy:** [https://mindsnap-3c915.web.app/before-you-sign/privacy-policy.html](https://mindsnap-3c915.web.app/before-you-sign/privacy-policy.html)
* **Official Contact:** `mindsnapstudios.contact@gmail.com`

---

<div align="center">
  <sub>Before You Sign is published by MindSnap Studios · Engineered with Kotlin, Jetpack Compose, Cloudflare Edge & Google Gemini</sub>
</div>

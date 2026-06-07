<div align="center">
  <img src="../mattress-company-web/public/logo.png" alt="SleepOnly Logo" width="200" style="margin-bottom: 20px;"/>
  <h1>SleepOnly.in — AI-Powered Premium Mattress Commerce</h1>
  <p><strong>A seamless, high-performance web experience merging luxury e-commerce with advanced conversational AI.</strong></p>

  [![Status](https://img.shields.io/badge/Status-Completed-success)](#)
  [![Tech Stack](https://img.shields.io/badge/Stack-HTML5%20|%20CSS3%20|%20Vanilla%20JS%20|%20Vite-blue)](#)
  [![Design](https://img.shields.io/badge/Design-Premium%20/%20Minimalist-orange)](#)

</div>

<br/>

## 📖 Overview

**SleepOnly.in** is a modern, responsive web application designed for a premium mattress brand operating pan-India. Shifting away from the traditional, high-pressure showroom sales environment, SleepOnly introduces **Taido**, an AI-powered Sleep Expert that guides users toward their perfect mattress using conversational logic and sleep science.

This project showcases a deep understanding of **front-end architecture, state management, and seamless third-party API integration** without the overhead of heavy frameworks. The result is a blazingly fast, visually stunning, and highly converting user experience.

---

## ✨ Key Features & Capabilities

### 1. Conversational Commerce (AI Integration)
- **Seamless Chatbase Integration:** Interfaced with Chatbase AI to provide real-time, context-aware mattress recommendations.
- **Event-Driven Triggers:** AI chat windows are programmatically triggered via tailored CTAs across the site, ensuring users have immediate access to guidance without navigating away from product details.

### 2. Persistent Shopping Cart Logic
- **Custom LocalStorage State Management:** Built a robust, vanilla JavaScript shopping cart (`cart.js`) that safely handles state persistence across browser sessions.
- **Interactive UI Updates:** Implemented a real-time reactive cart drawer and dynamic badge counters that update instantly upon adding/removing items, calculating accurate subtotals on the fly.

### 3. High-Performance Front-End Architecture
- **Vanilla JavaScript & Vite:** Leveraged the Vite build tool to deliver instantaneous hot-module replacement during development and highly optimized, minified bundles for production.
- **Zero-Dependency Animations:** Utilized the native `IntersectionObserver` API to orchestrate fluid `fade-up` and scaling animations as users scroll, avoiding bulky animation libraries.

### 4. Premium, Responsive UI/UX Design
- **Bespoke CSS Styling:** Crafted a warm, inviting color palette (Soft Creme, Muted Charcoal, Earthy Muted Brown) utilizing CSS variables for maintainability.
- **Fluid Typography:** Integrated Google Fonts (`Outfit` & `Playfair Display`) to evoke a sense of luxury and trustworthiness.
- **Mobile-First Responsiveness:** Implemented a flawless grid and flexbox layout that elegantly degrades gracefully on smaller viewports.

---

## 🛠️ Technical Stack

- **Core:** HTML5, CSS3, Vanilla JavaScript (ES6+)
- **Build Tool / Bundler:** Vite
- **Third-Party Integrations:** Chatbase AI (Conversational API)
- **Fonts & Typography:** Google Fonts

---

## 📂 Project Structure Highlights

```text
├── index.html          # Hero page & AI conversational showcase
├── collection.html     # Product listing with dynamic cart integration
├── style.css           # Global CSS variables, animations, and responsive rules
├── main.js             # Core UI logic, IntersectionObservers, and Navbar effects
├── cart.js             # OOP-based Shopping Cart logic utilizing LocalStorage
└── package.json        # Vite configuration and build scripts
```

---

## 🧠 Engineering Decisions & Best Practices

1. **Vanilla JS over Frameworks:**
   *Given the scope of the project, loading a heavyweight framework like React or Vue would have been overkill. By utilizing modern Vanilla JS, the site achieves a near-perfect Lighthouse performance score.*
2. **Object-Oriented Cart Implementation:**
   *The cart logic is encapsulated within a `ShoppingCart` class, ensuring clean separation of concerns between DOM manipulation and state management.*
3. **Glassmorphism & Modern CSS:**
   *The navigation bar utilizes `backdrop-filter: blur(15px)` to create a modern glassmorphism effect, maintaining UI hierarchy while keeping the user immersed in the hero imagery.*

---

## 🚀 How to Run Locally

1. Clone the repository.
2. Ensure you have Node.js installed.
3. Install dependencies:
   ```bash
   npm install
   ```
4. Start the Vite development server:
   ```bash
   npm run dev
   ```
5. To build for production:
   ```bash
   npm run build
   ```

---

<div align="center">
  <br/>
  <p><i>Crafted with precision, designed for comfort.</i></p>
</div>

# The Enigma Archives
**A Data-Driven Multiplayer Mystery Experience Built in Unity**

---

## 🚀 Project Overview

**The Enigma Archives** is an asynchronous, multiplayer mystery-solving game developed in Unity, utilizing Unity Netcode for GameObjects (NGO). It redefines the digital escape-room and deduction genre by introducing an adaptable, clue-driven narrative engine orchestrated by an AI/Server-side Game Master. 

Designed for scalability and rapid content iteration, the project features a robust `ScriptableObject`-based data architecture that completely separates game logic from narrative content. Players work together (or secretly against one another) to explore 2.5D environments, gather clues, and vote on narrative directions that dynamically branch based on their discoveries.

---

## 🎮 Core Gameplay Loop

The game relies on a highly structured, server-authoritative state machine divided into phases:

1. **Explore (Timed):** Players navigate unlocked rooms to investigate environmental anomalies and discover clues. Every clue uncovered unlocks specific "Route Tags."
2. **Discuss & Deduce:** Players communicate their findings, piecing together the overarching mystery. In "Type B" cases, a hidden Culprit works to misdirect the investigation.
3. **Vote:** As time expires, the Game Master evaluates the collective inventory of clues and Route Tags, generating custom narrative options. Players vote on their preferred theory.
4. **Narrate & Advance:** The winning vote determines the narrative consequences, advancing the chapter, unlocking new rooms, and dynamically altering the final ending.

---

## 🛠️ Technical Architecture & Highlights

As a showcase of professional Unity engineering, **The Enigma Archives** prioritizes modularity, network stability, and content scalability.

### 1. Server-Authoritative Network State
The core game loop is driven by the `GameStateManager`, a robust `NetworkBehaviour` that runs authoritatively on the Server/Host. It securely synchronizes game phases, timers, discovered clues (`NetworkList<int>`), and dynamic route tags across all connected clients.
* **Security & Integrity:** Clue discovery and phase transitions are validated entirely server-side to prevent client spoofing.
* **Seamless RPCs:** UI updates, narrative deliveries, and voting payloads are broadcast to clients efficiently using targeted RPCs.

### 2. ScriptableObject Data-Driven Design
Content is completely decoupled from the codebase using Unity's `ScriptableObject` architecture. 
* The `CaseData` structure handles everything: Rooms, Clues, Chapters, GM Options, Endings, and Culprit Configurations.
* **Scalable Content:** New mysteries can be authored and dropped into the project without touching a single line of C# code.

### 3. Dynamic Narrative Engine (`GuidebookEngine`)
The narrative doesn't follow a rigid tree; it acts as a gravity well. The `GuidebookEngine` evaluates a complex web of conditions in real-time. Narrative options dynamically unlock only if players have discovered the necessary prerequisite clues or accumulated specific Route Tags. 

### 4. Custom Python Content Pipeline
To bridge the gap between narrative designers and the Unity Engine, the project features a custom Python-based build pipeline (`build_case_guidebooks.py`). This tooling parses raw JSON case data into highly detailed, beautifully formatted `.docx` guidebooks for production planning and environment design, bridging technical implementation with creative writing.

---

## 📁 Featured Case Portfolios

The engine currently supports incredibly diverse narratives, demonstrating the flexibility of the systems:

* **Case 01: The Watcher on Floor Nine**
  * *Theme:* A gothic urban mystery where a false haunting conceals a real institutional crime. 
  * *Mechanic:* Procedural clue linking and multi-threaded suspect theories.
* **Case 02: MERIDIAN**
  * *Theme:* A sci-fi mystery aboard a generation ship grappling with simulated consciousness.
  * *Mechanic:* Emphasizes ethical voting choices over simple "whodunit" deduction.
* **Case 03: The Longest Group Chat**
  * *Theme:* A grounded, social mystery about manipulation and fractured friendships.
  * *Mechanic:* Focuses on timeline reconstruction, message timestamps, and spatial positioning.

---

## 💡 Developer's Note

*The Enigma Archives* is engineered to be a living platform rather than a static game. By leveraging Unity Netcode for secure state management and ScriptableObjects for infinite content expandability, the architecture is ready to scale from a prototype to a live-ops multiplayer title. The separation of the Game Master logic also ensures that the system is perfectly primed for integration with LLMs (like the Gemini API) to generate fully dynamic, responsive in-game narration in the future.

**Keywords:** Unity3D, C#, Unity Netcode for GameObjects (NGO), Multiplayer, ScriptableObjects, Systems Architecture, Data-Driven Design, UI/UX, Python Tooling.

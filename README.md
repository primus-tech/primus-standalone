# Primus Standalone Addon Suite for Vanilla WoW (1.12.1)

Welcome to the **Primus Standalone Addons** repository. This repository hosts plug-and-play standalone versions of all modules from the [PrimusSuite](https://github.com/primus-tech/primussuite) platform.

## 📦 What's Included

Every addon in this repository is **100% self-contained** and plug-and-play:

| AddOn Directory | Description | Commands |
| :--- | :--- | :--- |
| **`PrimusCore`** | Shared Foundation & Engine (Media, Skinner, Mover, Map & Tooltips) | `/primus`, `/pui` |
| **`PrimusMerchant`** | Auction House 10s Scanner, Pricing Model, Valuation & Offline Explorer | `/primus ah`, `/pui market` |
| **`PrimusRoleplay`** | Comprehensive RP Character Sheet, DiceMaster D20, Directory & Map Pins | `/primus rp`, `/rp` |
| **`PrimusQuest`** | Quest DB (Classic + Turtle WoW), Map Pin Resolver & Tracker | `/primus quest`, `/pq` |
| **`PrimusBags`** | Unified Continuous Grid, Discrete Container & Categorized Inventory with Auto-Sort | `/primus bags`, `/sort` |
| **`PrimusTalk`** | Chat Overhaul, Whisper Tabs, Message Logging & Social Suite | `/primus chat` |
| **`PrimusCombat`** | Tactical Combat HUD, CastBar, Cooldown Pulse & HealComm | `/primus combat` |
| **`PrimusHotbars`** | Action Bars, Micro Bag Bar & XP Tracker | `/primus bars` |
| **`PrimusUnitFrames`** | Unit Frames (Player, Target, Party, Pet) | `/primus uf` |

---

## 🚀 Installation

1. Download or clone this repository.
2. Copy any (or all) desired addon folders directly into your `World of Warcraft/Interface/AddOns/` directory.
3. If you install multiple standalone addons, you can optionally also install **`PrimusCore`** to share a single in-memory engine footprint!

---

## 🛡️ Standalone Architecture (Zero Bloat)
Each standalone addon includes an embedded fallback copy of `Libs/PrimusCore/` and is marked with `## OptionalDeps: PrimusCore`.
- If installed alone: it boots immediately with 0 external dependencies.
- If `PrimusCore` is present: `PrimusCore` loads first and master election yields embedded copies instantly with 0ms / 0 KB overhead.

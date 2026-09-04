# Discord Quest Automator

### Programmatic completion of active Discord quests via developer console

### Please Use The Discord Quest Code file Above README

<p align="center">
  <img src="https://img.shields.io/badge/status-stable-2ea44f?style=for-the-badge">
  <img src="https://img.shields.io/badge/platform-Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white">
  <img src="https://img.shields.io/badge/license-MIT-blue?style=for-the-badge">
  <img src="https://img.shields.io/badge/version-1.0.0-informational?style=for-the-badge">
</p>

---

## Overview

**Discord Quest Automator** is a self‑contained, single‑paste JavaScript module designed to be executed within Discord’s developer console.  
It automatically progresses any active quest by simulating the required user activity – **watching videos, playing games, or streaming** – using Discord’s own internal API endpoints.

The script provides a **live, non‑intrusive progress indicator** in the top‑left corner of the Discord window, styled to match Discord’s native UI. Upon completion, it displays a green confirmation and removes itself.

---

## Supported Quest Types

| Quest Type                     | Supported | Requirement          |
|--------------------------------|-----------|----------------------|
| `WATCH_VIDEO` / `WATCH_VIDEO_ON_MOBILE` | ✅        | Any                  |
| `PLAY_ON_DESKTOP`              | ✅        | Desktop app required |
| `STREAM_ON_DESKTOP`            | ✅        | Desktop app required |
| `PLAY_ACTIVITY`                | ✅        | Any                  |

- Processes **multiple quests** sequentially.
- Updates progress **smoothly** (increments by 1, no jumps).
- Stops automatically if Discord is reloaded (safe to re‑paste).
- Persists across server/DM navigation.

---

## Deployment Instructions

1. Launch **Discord** (desktop client is recommended – browser version will **not** work for desktop‑type quests).
2. Open developer tools:  
   - **Windows/Linux**: `Ctrl + Shift + I` → *Console* tab  
   - **macOS**: `Cmd + Option + I` → *Console* tab
3. **Copy the entire script** from the block below.
4. **Paste** it into the console and press `Enter`.
5. The progress indicator will appear in the **upper‑left corner** of the Discord window and update in real time.

> ⚠️ **Important:** The browser (web) version of Discord will **not** function for `PLAY_ON_DESKTOP` and `STREAM_ON_DESKTOP` quests. The desktop client is required for those.

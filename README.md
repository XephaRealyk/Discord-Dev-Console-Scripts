# Discord Console Scripts

### A curated collection of single‑paste scripts for Discord's developer console

<p align="center">
  <img src="https://img.shields.io/badge/status-active-2ea44f?style=for-the-badge">
  <img src="https://img.shields.io/badge/platform-Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white">
  <img src="https://img.shields.io/badge/license-MIT-blue?style=for-the-badge">
  <img src="https://img.shields.io/badge/version-1.0.0-informational?style=for-the-badge">
</p>

---

## What is this?

This repository is a **hub for verified JavaScript snippets** that you can paste directly into Discord's developer console to automate or enhance various features.

Each script is:
- **Self‑contained** – no external libraries or downloads.
- **Auditable** – you can read every line before running.
- **Safe** – no token logging, no external requests, no persistent storage.

---

## Available Scripts

| Script | Description |
|--------|-------------|
| **Quest Automator** | Automatically completes active quests (video, play, stream, activity). Shows live progress in the top‑left corner. |
| *(more coming soon)* | Additional utility scripts will be added over time. |

---

## How to Use

1. **Open Discord** (desktop app or browser – some scripts may require the desktop client).
2. **Open Developer Console**:
   - Windows/Linux: `Ctrl + Shift + I` → *Console* tab
   - macOS: `Cmd + Option + I` → *Console* tab
3. **Copy the script** from the repository (each script is in its own file, e.g., `quest-automator.js`).
4. **Paste** the entire script into the console and press `Enter`.
5. **Observe the result** – scripts typically provide visual feedback (UI overlays, console logs) and run until completion.

---

## What to Expect

- **Quest Automator**: A progress indicator appears in the top‑left corner of the Discord window, updating in real time. Once the quest is complete, the text turns green, says "Quest Completed", and fades out after 5 seconds.
- Scripts stop automatically if you reload Discord – just re‑paste to restart.

---

## Safety & Verification

Every script in this repository is designed with transparency in mind:

- **Network Audit** – Open DevTools → Network tab while running. All requests go exclusively to `discord.com` or `discordapp.com` – no external domains.
- **No Token Access** – Scripts do not read `localStorage`, `sessionStorage`, `document.cookie`, or any authentication tokens.
- **No Persistent Data** – They only create temporary DOM elements (overlays) which are removed upon completion.
- **Integrity Checks** – Each release includes a SHA‑256 hash of the script file so you can verify it hasn’t been altered.

---

## Limitations

| Issue | Details |
|-------|---------|
| **Reload kills execution** | Scripts do not persist across page reloads – paste again to resume. |
| **Desktop‑only features** | Some scripts (e.g., `PLAY_ON_DESKTOP` quests) require the Discord desktop client. |
| **One script at a time** | Running multiple scripts simultaneously may cause conflicts – run one, let it finish, then run another. |

---

## Contributing

Found a bug? Have an idea for a new script?  
Open an issue or submit a pull request – all contributions are welcome.

---

## License

MIT © 2026

---

<p align="center">
  <b>Built with <span style="color:#e25555;">❤</span> by Deepseek & Contributors</b>
</p>

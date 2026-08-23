<div align="center">
  <img src="Square150x150Logo.png" width="72" alt="Nexus logo" />
  <h1>Nexus</h1>
  <p>Your Browser. Your Notes. Your AI. Local. Private. Yours.</p>

  <p>
    <a href="https://getnexus.app">Website</a> ·
    <a href="https://getnexus.app/download">Download</a> ·
    <a href="https://github.com/getnexusapp/releases/issues">Report an issue</a> ·
    <a href="https://github.com/getnexusapp/docs">Documentation</a> ·
    <a href="https://github.com/getnexusapp/releases">Releases & Changelog</a>
  </p>
</div>

---
## About Nexus

One app that replaces three. Your notes, a real web browser, and an AI assistant — all in the same window, all talking to each other, all stored on your own computer.

Here's what that looks like in practice: you're researching something, so you open the page right inside Nexus's Browser tab — no switching to Chrome. Then you flip to the Assistant tab and ask "does this contradict what I already wrote?" — and it actually knows both, because it's reading your notes *and* the page you have open at the same time. Like the answer? One click saves it as a new note. You never left the app.

That's the specific gap both Obsidian and Notion leave open:
 - **Obsidian** is great for notes and linking ideas together — but there's no browser and no built-in AI. You're constantly alt-tabbing between Obsidian, Chrome, and ChatGPT, copy-pasting context between all three.
 - **Notion** bolts AI on top, but it lives in the cloud, usually needs a paid plan to be any good, and still has no browser tab of its own — same tab-juggling problem, plus your notes live on Notion's servers instead of yours.

Nexus keeps everything on your machine — one file on disk, no account, no server — and still gives you the workflow people normally need three separate apps to get.

---

## Features

**Notes**
- Markdown editor with Edit / Split / Preview modes, full formatting toolbar, and syntax-highlighted code blocks.
- `[[Wiki Links]]` between notes, with automatic backlinks.
- `#tags`, derived straight from what you type — no separate tag manager.
- Folders, pinning, and a fuzzy-search Command Palette (`Cmd/Ctrl+K`).
- Automatic Version History (restore any earlier snapshot) and a full Trash (soft-delete, restore, or delete forever).

**Browser**
- Up to 8 real, persistent browser tabs — built on native webviews, not iframes, so sites that block embedding still work.
- Bookmarks, back/forward/reload, and download tracking, all inside Nexus.

**Assistant**
- Chat that's automatically grounded in your notes via on-device semantic search, and in whatever page is open in the Browser tab.
- Chat history is saved locally and survives a restart.

**Knowledge Graph**
- A force-directed, draggable, zoomable map of how your notes link together.

**Local & Yours**
- Every note lives in a single local SQLite file
- One-click database backup/restore, and Markdown exports your whole vault.
- No account, no Nexus server, no telemetry — only you and your notes.

**Privacy**
- **Notes and search are fully local.** Your notes live in one SQLite file on disk. Search — including semantic ("meaning-based") search — runs through a small embedding model that executes entirely on your device. Nothing about your notes touches the network to be searched.
- **Export and backup are things you do, not things that happen automatically.** Backing up, restoring, and exporting to Markdown are explicit actions in Settings.

**License**
---

Nexus is proprietary, closed-source software. This organization does not
host the app's source code. The repositories here are for release notes,
documentation, and community support.

---

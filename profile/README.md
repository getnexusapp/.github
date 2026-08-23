<div align="center">
  <img src="Square150x150Logo.png" width="72" alt="Nexus logo" />
  <h1>Nexus</h1>
  <p>Your Browser. Your Notes. Your AI. Local. Private. Yours.</p>

  <p>
    <a href="">Website</a> ·
    <a href="">Download</a> ·
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

Here's the part that isn't about convenience: most AI note-taking tools built in the last couple of years still route your notes through someone else's servers to make the AI features work — even ones that market themselves as privacy-conscious. The moment there's a hosted AI layer, your data has to leave your machine to reach it.

Nexus doesn't have that server. It was never built to have one. That's why the Assistant is bring-your-own-key (BYOK) instead of a Nexus-hosted feature: every request goes straight from your device to your provider, because there's nothing of ours in between to route it through. Your notes stay in a single file on your disk, your searches happen entirely on your device, and the one time anything does leave your machine — an AI question — it goes exactly where you told it to go, and nowhere else.

No account required. No cloud sync you didn't ask for. No *"we may share anonymized data with partners"* clause buried in a privacy policy. Just your notes, on your machine, under your control.

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
- Bring your own API key. Every message goes straight from your device to your provider — there's no Nexus server in between, so there's nothing for us to see, log, or store.
- Chat history is saved locally and survives a restart.

**Knowledge Graph**
- A force-directed, draggable, zoomable map of how your notes link together.

**Privacy**
- **Notes and search are fully local.** Your notes live in one SQLite file on disk. Search — including semantic ("meaning-based") search — runs through a small embedding model that executes entirely on your device. Nothing about your notes touches the network to be searched.
- **The one place data leaves your device: AI chat, and only with your own key.** Ask the Assistant something, and Nexus sends that message straight from your machine to whichever provider you've connected, using an API key stored in your OS's own secure credential store — never in a Nexus database. We don't operate a server in that path. There's nothing routing through us to see, log, or sell.
- **Export and backup are things you do, not things that happen automatically.** Backing up, restoring, and exporting to Markdown are explicit actions in Settings.

**License**
---

Nexus is proprietary, closed-source software owned by **Nawrass Andaloussi Dahman**.

This organization does not host the app's source code. The repositories here are for release notes,
documentation, and community support.

Use of the Nexus application is governed by the **Nexus End User License Agreement (EULA)**.

For more information:

- [LICENSE.md](https://github.com/getnexusapp/.github/blob/main/LICENSE.md)
- [EULA.md](https://github.com/getnexusapp/.github/blob/main/EULA.md)
- [PRIVACY_POLICY.md](https://github.com/getnexusapp/.github/blob/main/PRIVACY_POLICY.md)

---

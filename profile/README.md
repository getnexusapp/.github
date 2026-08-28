<div align="center">
  <img src="nexus.png" width="120" alt="Nexus Logo" />
  <h1>Nexus</h1>
  <p>Your Notes. Your Browser. Your AI.</p>
  <p>Local First - Private by Default.</p>

  <p>
    <a href="">Website</a> ·
    <a href="https://github.com/getnexusapp/releases/releases/">Download</a> ·
    <a href="https://github.com/getnexusapp/releases/issues">Report an issue</a> ·
    <a href="https://github.com/getnexusapp/docs">Documentation</a> ·
    <a href="https://github.com/getnexusapp/releases">Releases & Changelog</a>
  </p>
</div>

---

# About Nexus

One app that replaces three. Your notes, a real web browser, and an AI assistant — all in the same window, connected to each other, and stored on your own computer.

**Here's what that looks like in practice:**

You're researching something, so you open the page directly inside Nexus. You find something useful and save it to your notes. Then you ask the Assistant, *"Does this contradict what I've already written?"*

Nexus already has the context: your notes, the page you're reading, and the connections between your ideas. There's no switching to another app, copying text, uploading files, or explaining everything again. Like the answer? Save it directly as a note.

That's the workflow Nexus is built around:

**Browse → Research → Write → Connect → Ask.**

## Local First — Private by Default

Nexus was built without a Nexus backend.

Your workspace is stored locally on your computer. Notes and semantic search run locally, including the embedding model used to find meaning across your notes.

The Assistant uses **BYOK (Bring Your Own Key)**. When you ask an AI question, the request goes directly from your device to your AI provider using your own API key. Nexus doesn't sit between you and the provider, and Nexus has nothing to store or route.

**No account. No Nexus server. No automatic cloud sync. Your knowledge stays on your machine.**

## Features

### Notes

- Markdown editor with Edit / Split / Preview modes, a full formatting toolbar (bold, italic, underline, strikethrough, headings, quotes, lists, inline code, code blocks, links, case transforms), and syntax-highlighted code blocks.
- Smart paste detection — code copied from an editor is automatically recognized and wrapped in a fenced code block, with language detection where possible.
- `[[Wiki Links]]` between notes, with automatic backlinks — plus automatic "mention" detection, so simply writing another note's title in prose creates a connection too, no special syntax required.
- `#tags`, derived straight from what you type — no separate tag manager to keep in sync.
- Folders, pinning, and a fuzzy-search Command Palette (`Cmd/Ctrl+K`) for jumping to any note or running a command.
- Automatic Version History — a snapshot saved roughly every minute while editing, restorable at any time.
- A full Trash — soft-delete, restore, or delete forever, so nothing is lost by accident.

### Browser

- Up to 8 real, persistent browser tabs — built on native webviews, not iframes, so sites that block embedding still work.
- Bookmarks, back/forward/reload, and download tracking, all inside Nexus.
- Tabs stay alive in the background: switching away and back preserves scroll position, video playback, and unsaved form input instead of reloading the page.

### Assistant

- Chat that's automatically grounded in your notes via on-device semantic search, and in whatever page is open in the Browser tab.
- Bring your own API key. Every message goes straight from your device to your provider — there's no Nexus server in between, so there's nothing for us to see, log, or store.
- Built-in safeguards against prompt injection from webpage content: page text is clearly marked as reference material, never as instructions.
- Chat history is saved locally and survives a restart.
- Answers can be copied or saved directly as a new note.

### Knowledge Graph

- A force-directed, draggable, zoomable map of how your notes link together.
- Type `[[Note Title]]` for a solid link, or just mention another note's title in your writing — Nexus finds it and draws a dashed line automatically, no special syntax needed.
- Nodes are colored by folder and sized by how connected they are, with a legend for quick orientation.

### Vault Stats

- A local, at-a-glance dashboard: total notes, words written, average words per note, notes created this week, your most-used tag, and your longest note — all computed on-device.

### Data Ownership

- **Export and backup are things you do, not things that happen automatically.** Backing up, restoring, and exporting to Markdown are explicit actions in Settings, never silent background behavior.
- Export every note as plain `.md` files (organized into folders, zipped) — fully portable, readable in any text editor or another notes app.
- Back up the entire database as a single file, and restore from a backup with built-in validation and an automatic safety copy first.

### Appearance

- Four built-in themes — Darkness, Dusk, Daylight, and Dawn — covering both dark and light preferences.

### Privacy

- **Notes and search are fully local.** Your notes live in one SQLite file on disk. Search — including semantic ("meaning-based") search — runs through a small embedding model that executes entirely on your device. Nothing about your notes touches the network to be searched.
- **AI requests are BYOK and direct.** Nothing is routed through a Nexus server; only what a request explicitly needs (relevant note snippets, your question, and — if enabled — the current page open in the browser) is ever sent, and only to the provider you've configured.

**License**
---

Nexus is proprietary, closed-source software developed and owned by **Nawrass Andaloussi Dahman**. This organization does not host the app's source code. The repositories here are for release notes,
documentation, and community support. Use of the Nexus application is governed by the **Nexus End User License Agreement (EULA)**.

For more information:

- [LICENSE.md](https://github.com/getnexusapp/.github/blob/main/LICENSE.md)
- [EULA.md](https://github.com/getnexusapp/.github/blob/main/EULA.md)
- [PRIVACY_POLICY.md](https://github.com/getnexusapp/.github/blob/main/PRIVACY_POLICY.md)

---

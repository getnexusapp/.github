<div align="center">
  <img src="Nexus.png" width="120" alt="Nexus Logo" />
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

## About Nexus

One app that replaces three. Your notes, a real web browser, and an AI
assistant — all in the same window, connected to each other, and stored
on your own computer.

**Here's what that looks like in practice:**

You're researching something, so you open the page directly inside Nexus.
You find something useful and save it to your notes. Then you ask the
Assistant, *"Does this contradict what I've already written?"*

Nexus already has the context: your notes, the page you're reading, and
the connections between your ideas. There's no switching to another app,
copying text, uploading files, or explaining everything again. Like the
answer? Save it directly as a note.

That's the workflow Nexus is built around:

**Browse → Research → Write → Connect → Ask.**

### Why Nexus?

Most knowledge workflows are split across separate applications:

- **Obsidian** gives you powerful notes and linking, but research happens
  in another browser and AI lives somewhere else.
- **Notion** combines notes and AI, but your workspace lives in the cloud
  and the browser isn't part of the workspace.

Nexus brings those pieces together.

Your browser, notes, AI, and knowledge graph aren't separate tools sitting
next to each other. They're connected parts of the same workspace.

### Local First - Private by Default

Nexus was built without a Nexus backend.

Your workspace is stored locally on your computer. Notes and semantic
search run locally, including the embedding model used to find meaning
across your notes.

The Assistant uses **BYOK (Bring Your Own Key)**. When you ask an AI
question, the request goes directly from your device to your own IP key. Nexus doesn't sit between you and the provider, and Nexus has
nothing to store or route.

**No account. No Nexus server. No automatic cloud sync. Your knowledge
stays on your machine.**

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
- **Export and backup are things you do, not things that happen automatically.** Backing up, restoring, and exporting to Markdown are explicit actions in Settings.

**License**
---

Nexus is proprietary, closed-source software owned by **Nawrass Andaloussi Dahman**. This organization does not host the app's source code. The repositories here are for release notes,
documentation, and community support. Use of the Nexus application is governed by the **Nexus End User License Agreement (EULA)**.

For more information:

- [LICENSE.md](https://github.com/getnexusapp/.github/blob/main/LICENSE.md)
- [EULA.md](https://github.com/getnexusapp/.github/blob/main/EULA.md)
- [PRIVACY_POLICY.md](https://github.com/getnexusapp/.github/blob/main/PRIVACY_POLICY.md)

---

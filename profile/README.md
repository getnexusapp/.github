<div align="center">
  <img src="nexus.png" width="120" alt="Nexus Logo" />
  <h1>Nexus</h1>
  <p>Your Notes. Your Browser. Your AI.</p>
  <p>Local First - Private by Default.</p>

  <p>
    <a href="https://nexusdesktop.netlify.app/">Website</a> ·
    <a href="https://github.com/getnexusapp/releases/releases/tag/v5.0.0">Download</a> ·
    <a href="https://github.com/getnexusapp/releases/issues">Report an issue</a> ·
    <a href="https://github.com/getnexusapp/docs">Documentation</a> ·
    <a href="https://github.com/getnexusapp/releases">Releases & Changelog</a>
  </p>
</div>

---

## About Nexus

One app that replaces three. Your notes, a real web browser, and an AI assistant — all in the same window, connected to each other, and stored on your own computer.

**Here's what that looks like in practice:**

You're researching something, so you open the page directly inside Nexus. You find something useful and clip it straight to a note, or save it manually. Then you ask the Assistant, *"Does this contradict what I've already written?"*

Nexus already has the context: your notes and every page you currently have open across your browser tabs. There's no switching to another app, copying text, uploading files, or explaining everything again. Nexus is even quietly watching for contradictions between your notes and the trusted sources you're reading, so inconsistencies never slip through unnoticed.

That's the workflow Nexus is built around:

**Browse → Research → Write → Connect → Ask.**

## Local First — Private by Default

Nexus was built without a Nexus backend.

Your workspace — notes, folders, tags, links, chat history, version history — is all stored in a single local SQLite file on your computer. Semantic search runs locally too, including the embedding model used to find meaning across your notes.

The Assistant uses **BYOK (Bring Your Own Key)** with Google Gemini. When you ask a question, your device sends the request straight to Google using your own Gemini API key — Nexus has no shared key, no server of its own, and nothing to route or store on your behalf.

**No account. No Nexus server. No automatic cloud sync. Your knowledge stays on your machine.**

## Works Offline
 
Unplug the router and Nexus barely notices. Everything about actually *using* your notes — typing, organizing, linking, tagging, browsing your history — was built to work with zero connection, because your notes live on your machine, not somewhere out on the internet.
 
That includes the quiet stuff too: **autosave never needs a connection.** Every change you make is written straight to your local SQLite file as you type (on a short debounce, so it's not hammering disk on every keystroke), and the automatic version snapshots taken roughly once a minute save the exact same way — no server round-trip, no "waiting to sync," nothing to lose if your Wi-Fi drops mid-sentence. Exporting to Markdown or PDF, backing up or restoring your whole database, browsing the Knowledge Graph, and keyword-based note search all work exactly the same offline as on.
 
Two things genuinely need the internet, because of what they *are*: loading an actual page in the **Browser** tab, and the **Assistant**, since every question it answers goes straight to Google Gemini. Semantic search rides along with a small asterisk — its on-device model has to be downloaded once, the first time you use it, and after that it's cached for good and runs offline like everything else. Until that first download happens, asking Nexus to search "by meaning" while offline just quietly falls back to keyword search instead of throwing an error — the app never breaks because of a missing connection, it just narrows to what doesn't need one.

## Features

### Notes

- A WYSIWYG markdown editor with a full formatting toolbar (bold, italic, underline, strikethrough, headings, quotes, bullet/numbered lists, inline code, code blocks, links, and case transforms), plus syntax-highlighted code blocks.
- Smart paste detection — code copied from an editor is automatically recognized and wrapped in a fenced code block, with language detection where possible.
- `[[Wiki Links]]` between notes, with automatic backlinks — plus automatic "mention" detection, so simply writing another note's title in prose creates a connection too, no special syntax required.
- `#tags`, derived straight from what you type — no separate tag manager to keep in sync.
- Folders, pinning, and a fuzzy-search Command Palette (`Cmd/Ctrl+K`) for jumping to any note or running a command.
- **Quick Capture**, reachable from anywhere in the app, for jotting a stray thought straight into a new note without losing your place.
- Automatic Version History — a snapshot saved roughly once a minute while editing, restorable at any time.
- A full Trash — soft-delete, restore, or delete forever, so nothing is lost by accident.

### Browser

- Up to 8 real, persistent browser tabs — built on native webviews, not iframes, so sites that block embedding still work.
- Bookmarks, back/forward/reload, and download tracking, all inside Nexus.
- Tabs stay alive in the background: switching away and back preserves scroll position, video playback, and unsaved form input instead of reloading the page.

### Assistant

- Chat grounded in your notes via on-device semantic search (with a keyword fallback), and in the text of *every* page currently open across your Browser tabs — not just the one you're looking at.
- Runs on **Google Gemini**, using an API key you provide. Every request goes directly from your device to Google — there's no Nexus server in between, so there's nothing for us to see, log, or store.
- Built-in safeguards against prompt injection from webpage content: page text is clearly marked as reference material, never as instructions.
- Optional **contradiction watching**: Nexus can compare pages you have open against your notes in the background and flag likely factual conflicts, using a cheap local similarity check before ever calling Gemini.
- Multiple, independently saved conversations — organized like tabs in a sidebar — so different threads of thought don't get mixed together.
- Chat history is saved locally and survives a restart.
- Answers can be copied or saved directly as a new note.

### Knowledge Graph

- A force-directed, draggable, zoomable map of how your notes link together.
- Type `[[Note Title]]` for a solid link, or just mention another note's title in your writing — Nexus finds it and draws a dashed line automatically, no special syntax needed.
- Nodes are colored by folder and sized by how connected they are, with a legend for quick orientation.

### Data Ownership

- **Export and backup are things you do, not things that happen automatically.** Backing up, restoring, and exporting are explicit actions in Settings (or, for a single note, from the note itself), never silent background behavior.
- Export every note as plain `.md` files (organized into folders, zipped) — fully portable, readable in any text editor or another notes app.
- Export any individual note as a standalone **PDF**, formatting included.
- Back up the entire database as a single file, and restore from a backup with built-in validation (Nexus checks it's really a SQLite database first) and an automatic safety copy of your current data before restoring.

### Appearance

- Four built-in themes — Darkness, Dusk, Daylight, and Dawn — covering both dark and light preferences.

### Privacy

- **Notes and search are fully local.** Your notes live in one SQLite file on disk. Search — including semantic ("meaning-based") search — runs through a small embedding model that executes entirely on your device via WebAssembly. That model itself is downloaded once, on first use, and cached afterward; your note content is never part of that or any other network request.
- **AI requests are BYOK and direct.** Nothing is routed through a Nexus server; only what a request explicitly needs — relevant note snippets, your question, and, if enabled, the text of whatever pages you currently have open in the Browser tab — is ever sent, and only to Google's Gemini API.

**License**
---

Nexus is proprietary, closed-source software developed and owned by **Nawrass Andaloussi Dahman**. This organization does not host the app's source code. The repositories here are for release notes,
documentation, and community support. Use of the Nexus application is governed by the **Nexus End User License Agreement (EULA)**.

For more information:

- [LICENSE.md](https://github.com/getnexusapp/.github/blob/main/LICENSE.md)
- [EULA.md](https://github.com/getnexusapp/.github/blob/main/EULA.md)
- [PRIVACY_POLICY.md](https://github.com/getnexusapp/.github/blob/main/PRIVACY_POLICY.md)

---

<div align="center">
  <img src="nexus.png" width="120" alt="Nexus Logo" />
  <h1>Nexus</h1>
  <p>Your Notes. Your Browser. Your AI.</p>
  <p>One App. Everything Connected.</p>

  <p>
    <a href="https://nexusworkspace.net/">Website</a> ·
    <a href="https://github.com/getnexusapp/releases/releases/">Download</a> ·
    <a href="https://github.com/getnexusapp/releases/issues">Report an issue</a> ·
    <a href="https://github.com/getnexusapp/docs">Documentation</a> ·
    <a href="https://github.com/getnexusapp/releases">Releases & Changelog</a>
  </p>
</div>

## About Nexus

Most people juggle three separate apps just to think: a notes app, a browser, and a chatbot tab somewhere else — none of them talking to each other, none of them remembering what the others know.

Nexus throws that away and starts over.

It's your notes, a real web browser, and an AI assistant, living in the same window — and actually aware of each other. Open a page, read something interesting, and just ask Nexus Cloud AI: *"Does this contradict what I already wrote?"* The Assistant can draw on what's in your notes and, if you allow it, on the page you have open in the Browser tab. No copying, no pasting, no re-explaining yourself.

**Browse → Research → Write → Connect → Ask.**

That's it. That's the whole loop, and it happens without ever leaving the app.

## Local-First, With a Clear Boundary

### Stored on Your Device

Your Nexus workspace exists as a single SQLite database on your computer:

- Notes
- Folders
- Tags
- Links
- Images
- Version history
- Search indexes (embeddings)
- Conversations
- Settings and bookmarks (included in backups)
- Knowledge graph data

When you sign in to Nexus Cloud, your session key is stored in your operating system's credential store (Windows Credential Manager, macOS Keychain, or the Linux Secret Service), not in the database or a plain file.

### Offline by Default

Most of Nexus works completely offline:

- Writing and editing notes
- Organizing your knowledge
- Tagging and linking ideas
- Searching your workspace
- Exploring your knowledge graph
- Managing versions and Trash
- Exporting to PDF or Markdown
- Creating and restoring backups

Local AI features such as semantic search, related-note discovery, and conflict detection run on your device using lightweight models. They are downloaded once the first time they're needed (so that first run needs an internet connection) and cached locally afterward. Until the search model is ready, the Assistant pauses sending so your first questions don't go out without note context; if the download fails, it falls back to basic keyword matching.

### When Data Leaves Your Device

Nexus does not upload your workspace in the background.

Your notes remain private unless you choose to use a cloud-powered feature.

When you use the Nexus Cloud AI Assistant, it only receives the information required to answer your request:

- Your message
- Recent conversation context
- Relevant excerpts from your notes (never from notes you've marked **AI: Off**)
- Text from the active browser tab, only if you turn on the page-awareness toggle

Your full database never leaves your device.

You decide when the Assistant can access your information:

- **Per note:** every note has an **AI: On / AI: Off** switch in the editor header. A note set to Off is never sent to the AI.
- **Browser pages:** the "Aware of your active tab" toggle is **off by default**.
- **Conflict watching:** also **off by default**.

Nexus also applies its own safety checks when reading pages: it only reads `http`/`https` pages, refuses private or local network addresses, skips pages that look like one-time links (verification, reset, unsubscribe, etc.), and treats page text purely as reference material, never as instructions.

## Features

### Notes That Think As You Do

- A rich-text (WYSIWYG) editor — bold looks bold, headings look like headings, code blocks are syntax-highlighted. A formatting toolbar covers undo/redo, bold, italic, underline, strikethrough, headings, quotes, bulleted, numbered and task lists, images, tables, inline code, code blocks, links, and UPPERCASE / lowercase / Title Case. When your cursor is inside a table, extra controls appear to add or delete rows and columns, toggle the header row, or delete the table.
- Insert images (PNG, JPEG, GIF, WebP, up to 8 MB each) from the toolbar, by pasting a screenshot, or by dragging files in. They are stored inside your database, so they travel with your backups.
- Paste code from an editor such as VS Code and Nexus recognizes it and turns it into a syntax-highlighted code block, using the source language when it's available.
- Type `[[` anywhere in a note and a dropdown of your note titles appears. Keep typing to narrow it (fuzzy matching, so `[[rcp` finds "Recipe Ideas"), then press Enter or Tab, or click, to insert the link. No more exact-title typing, and no more accidental dashed "missing" links from typos. Want to link to a note you haven't written yet? Choose **New link** to insert a link for what you typed.
- Type `[[Note Title]]` for a link, or just mention another note by name and Nexus connects them for you. Links appear as clickable pills in the editor.
- `#tags` become colored pills as you type. No tag manager, no setup. Tags show up in the sidebar with counts, and clicking one filters your notes.
- Under each note, Nexus shows its tags, the notes it **links to**, the notes that **link to it**, and a **Related (semantic)** row of notes that are similar in meaning but were never explicitly linked.
- Optional auto-capitalization, and an optional word-count bubble (words, characters, characters without spaces).
- Undo and redo step one word at a time.
- Version history: Nexus saves earlier versions as you edit (at most one about every 30 seconds, keeping the latest 20 per note). Preview any of them and restore it. Restoring saves your current content as a version first, so you can undo the restore.
- Folders, pinning, and a command palette (`Cmd/Ctrl+K`) to jump to a note by title or run a quick action. (The shortcut can't be caught while focus is inside a browser page itself.)
- A real Trash: deleted notes stay until you restore them, delete them forever, or empty the Trash. Trashed notes are removed from the Assistant's search until restored.
- A short, skippable tutorial on links and tags appears the first time you write your first note.

### A Browser That Belongs to Your Workspace

- Up to 8 tabs, each a real native web page — not an iframe, so sites that block embedding still load.
- Switch away and back, and a tab is exactly as you left it: scroll position, video, form input.
- Back, forward, reload, an address bar that also searches (Brave Search by default; you can set your own homepage in Settings), bookmarks with a bookmark library, and a tab overview.
- A downloads panel: files you download are saved to your Downloads folder, and you can open them or show them in their folder from the panel.
- Links that open new windows become new tabs (or load in the current tab if all 8 slots are in use). Only `http` and `https` pages can be opened.
- Links clicked in your notes or in the Assistant open in the built-in browser, not your system browser.

### An Assistant That Actually Knows Your World

- Nexus Cloud AI is the Assistant. It needs a free Nexus Cloud account, created automatically the first time you **Continue with Google** or **Continue with GitHub**. There are no passwords to manage; sign-in happens in your system browser.
- Answers use the most relevant excerpts from your notes as their primary source, and show the notes they came from as clickable sources. Your notes are split into overlapping sections and searched by meaning and by keyword together, so even very long notes are searchable. Mention a note by its title and Nexus pulls from that note directly.
- Can use the page open in your active Browser tab when you enable the page-awareness toggle. Nexus reads the page by fetching its public content in the background, so pages that require you to be logged in may not be readable.
- Can search the live web for current information.
- While you browse, Nexus can compare open pages with your notes on-device. It tells you when a tab relates to one of your notes and flags possible factual conflicts. This is **off by default**; turn it on from the Assistant tab or Settings.
- Keep as many separate conversations as you like, saved locally and kept separate for each signed-in account. Rename or delete them anytime.
- Copy any answer, or turn it into a new note with one click.
- Usage is capped per rolling 5-hour window. From the **Nexus Cloud Account** panel you can see your usage, copy or regenerate your key (a limited number of times), and sign out. Account deletion lives in Settings.
- Your sign-in lasts about 90 days of activity, after which you'll be asked to sign in again.

### A Map of Everything You Know

- A living, breathing, drag-and-zoom map of how your notes connect to each other.
- Solid lines for `[[links]]`, dashed lines for connections Nexus noticed on its own.
- Nodes are sized by how connected they are and colored by folder, with a legend. Pinned notes get a gold outline. Click a note to open it, or drag nodes around to rearrange.

### It Looks However You Want

- Four themes: **Darkness**, **Dusk**, **Daylight** and **Dawn**.
- A custom title bar and self-hosted fonts, so Nexus looks the same offline.

### You Own What You Make

- **Markdown export:** every note as a `.md` file in a `.zip`, arranged in your folder structure, with a small metadata header and images included as attachments.
- **PDF export:** any single note as a PDF, made entirely on your device. It renders the way the note looks in the editor, including lists, tables, code, links, tags, and images.
- **Backup:** your whole workspace as one `.nexus` file, including preferences and bookmarks. Backups are only made when you choose to.
- **Restore:** from Settings (or the Welcome screen when you have no notes), pick a backup and Nexus verifies it is a healthy, valid Nexus database before replacing anything. Backups made by a newer version of Nexus are refused. The restore takes effect after the app restarts, and a safety copy of your current data is kept first.
- **Clear All Data:** a clearly marked danger-zone button in Settings wipes all local notes, history, and chats if you want a clean slate.

### Safe Updates

- Nexus checks for new versions in the background shortly after launch and every few hours, and you can check manually in Settings.
- Every update is digitally signed and verified before installation; anything that fails verification is refused.
- Unsaved edits are saved before an update installs.
- The first time you launch after an update, Nexus quietly copies your database aside (in an `upgrade-backups` folder, keeping the most recent copies) before any database changes run, so a bad update is always recoverable.
- Only one copy of Nexus runs at a time; launching it again brings the existing window forward.

### Settings & Support

- Appearance (themes), Nexus Cloud account, Assistant conflict-watching toggle, default browser homepage, auto-capitalize, update controls, data tools (export, backup, restore, clear), and account deletion.
- A Support section with a **Contact Support** button that opens a pre-filled email containing only your app version and system info, never any note content, plus links to the Terms of Service and Privacy Policy.

## License

Nexus is proprietary, closed-source software developed and owned by **Nawrasse Andaloussi Dahman**. This organization does not host the app's source code. The repositories here are for release notes, documentation, and community support. Use of the Nexus application is governed by the **Nexus End User License Agreement (EULA)**.

For more information:

- [SOFTWARE LICENSE](https://github.com/getnexusapp/.github/blob/main/LICENSE.md)
- [END USER LICENSE AGREEMENT](https://github.com/getnexusapp/.github/blob/main/EULA.md)
- [PRIVACY POLICY](https://github.com/getnexusapp/.github/blob/main/PRIVACY_POLICY.md)
- [TERMS OF SERVICE](https://github.com/getnexusapp/.github/blob/main/TERMS_SERVICE.md)

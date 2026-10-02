<div align="center">
  <img src="nexus.png" width="120" alt="Nexus Logo" />
  <h1>Nexus</h1>
  <p>Your Notes. Your Browser. Your AI.</p>
  <p>One App. Everything Connected.</p>

  <p>
    <a href="https://letnexusout.vercel.app/">Website</a> ·
    <a href="https://github.com/getnexusapp/releases/releases/">Download</a> ·
    <a href="https://github.com/getnexusapp/releases/issues">Report an issue</a> ·
    <a href="https://github.com/getnexusapp/docs">Documentation</a> ·
    <a href="https://github.com/getnexusapp/releases">Releases & Changelog</a>
  </p>
</div>

## About Nexus

Most people juggle three separate apps just to think: a notes app, a browser, and a chatbot tab somewhere else — none of them talking to each other, none of them remembering what the others know.

Nexus throws that away and starts over.

It's your notes, a real web browser, and an AI assistant, living in the same window — and actually aware of each other. Open a page, read something interesting, and just ask Nexus Cloud AI: *"Does this contradict what I already wrote?"* The Assistant already knows what's in your notes and what's open in every one of your browser tabs. No copying, no pasting, no re-explaining yourself.

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
- Conversations
- Settings
- Knowledge graph data

Your Nexus Cloud key is automatically stored in your operating system's credential store, once you create a Nexus Cloud account.

### Offline by Default

Most of Nexus works completely offline:

- Writing and editing notes
- Organizing your knowledge
- Tagging and linking ideas
- Searching your workspace
- Exploring your knowledge graph
- Managing versions and Trash
- Exporting to PDF or Markdown
- Creating backups

Local AI features such as semantic search, related-note discovery, and conflict detection run on your device using lightweight models downloaded once and cached locally.

### When Data Leaves Your Device

Nexus does not upload your workspace in the background.

Your notes remain private unless you choose to use a cloud-powered feature.

When you use the Nexus Cloud AI Assistant, it only receives the information required to answer your request:

- Your message
- Recent conversation context
- Relevant excerpts from your notes (if you enable note access)
- Text from browser tabs you choose to include

Your full database never leaves your device.

You decide when the Assistant can access your information, and you can disable access to it at any time.

## Features

### Notes That Think As You Do

- A rich-text (WYSIWYG) editor — bold looks bold, headings look like headings, code blocks are syntax-highlighted. A formatting toolbar covers undo/redo, bold, italic, underline, strikethrough, headings, quotes, bulleted, numbered and task lists, images, tables, inline code, code blocks, links, and UPPERCASE / lowercase / Title Case.
- Insert images (PNG, JPEG, GIF, WebP, up to 8 MB each). They are stored inside your database, so they travel with your backups.
- Type `[[` anywhere in a note and a dropdown of your note titles appears. Keep typing to narrow it (fuzzy matching, so `[[rcp` finds "Recipe Ideas"), then press Enter or Tab, or click, to insert the link. No more exact-title typing, and no more accidental dashed "missing" links from typos. Want to link to a note you haven't written yet? Choose **New link** to insert a link for what you typed.
- Type `[[Note Title]]` for a link, or just mention another note by name and Nexus connects them for you. Links appear as clickable pills in the editor.
- `#tags` become colored pills as you type. No tag manager, no setup.
- Optional auto-capitalization, and an optional word-count bubble (words, characters, characters without spaces).
- Undo and redo step one word at a time.
- Version history: Nexus saves earlier versions as you edit. Preview any of them and restore it.
- Folders, pinning, and a command palette (`Cmd/Ctrl+K`) to jump to a note by title or run a quick action.
- A real Trash: deleted notes stay until you restore them, delete them forever, or empty the Trash.

### A Browser That Belongs to Your Workspace

- Up to 8 tabs, each a real native web page — not an iframe, so sites that block embedding still load.
- Switch away and back, and a tab is exactly as you left it: scroll position, video, form input.
- Back, forward, reload, an address bar that also searches (Brave Search by default; you can set your own homepage), bookmarks with a bookmark library, and a tab overview.
- Links that open new windows become new tabs. Only `http` and `https` pages can be opened.
- Links clicked in your notes or in the Assistant open in the built-in browser, not your system browser.

### An Assistant That Actually Knows Your World

- Nexus Cloud AI is the Assistant. It needs a free Nexus Cloud account (email and password).
- Answers use the most relevant excerpts from your notes as their primary source, and name the note they came from. Your notes are searched by meaning and by keyword.
- Can also use the pages open in the Browser tab. Nexus reads a page by fetching its content in the background.
- Can search the live web for current information.
- While you browse, Nexus compares open pages with your notes on-device. It tells you when a tab relates to one of your notes and flags possible factual conflicts (you can switch this off).
- Keep as many separate conversations as you like, all saved locally under your account. Rename or delete them anytime.
- Turn any answer into a new note with one click.
- Usage is capped per rolling 5-hour window. You can check your usage, regenerate your key (limited number of times), reset your password by email, or delete your account from the app.

### A Map of Everything You Know

- A living, breathing, drag-and-zoom map of how your notes connect to each other.
- Solid lines for `[[links]]`, dashed lines for connections Nexus noticed on its own.
- Nodes are sized by how connected they are and colored by folder. Pinned notes get a gold outline. Click a note to open it.

### It Looks However You Want

- Four themes: **Darkness**, **Dusk**, **Daylight** and **Dawn**.
- A custom title bar and self-hosted fonts, so Nexus looks the same offline.

### You Own What You Make

- **Markdown export:** every note as a `.md` file in a `.zip`, arranged in your folder structure, with a small metadata header and images included as attachments.
- **PDF export:** any single note as a PDF, made entirely on your device.
- **Backup:** your whole workspace as one `.nexus` file, including preferences and bookmarks. Backups are only made when you choose to.
- **Restore:** pick a backup and Nexus checks that it is a valid SQLite database before replacing anything, and the restore takes effect after you restart the app.

## License

Nexus is proprietary, closed-source software developed and owned by **Nawrass Andaloussi Dahman**. This organization does not host the app's source code. The repositories here are for release notes, documentation, and community support. Use of the Nexus application is governed by the **Nexus End User License Agreement (EULA)**.

For more information:

- [SOFTWARE LICENSE](https://github.com/getnexusapp/.github/blob/main/LICENSE.md)
- [END USER LICENSE AGREEMENT](https://github.com/getnexusapp/.github/blob/main/EULA.md)
- [PRIVACY POLICY](https://github.com/getnexusapp/.github/blob/main/PRIVACY_POLICY.md)
- [TERMS OF SERVICE](https://github.com/getnexusapp/.github/blob/main/TERMS_SERVICE.md)

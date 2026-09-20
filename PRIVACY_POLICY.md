# Nexus Privacy Policy

**Last Updated: September 20, 2026**

Nexus is developed and operated by **Nawrass Andaloussi Dahman**, an independent software developer based in Morocco.

This Privacy Policy explains how Nexus handles information when you use the Nexus desktop application ("Nexus" or the "Software") and, where applicable, the Nexus Cloud Service that powers the optional AI Assistant.

Nexus's core notes and workspace functionality is local-first: your notes stay on your device unless you choose to export or back them up. The **AI Assistant is different**: it requires a Nexus Cloud account and is powered by a server that Nexus operates. This policy describes both clearly.

---

## 1. Information Nexus Does Not Collect (Local Workspace)

When you use Nexus's core note-taking and browsing functionality, Nexus does not collect or store the following on Nexus-operated servers:

- Your notes, folders, tags, links, and content;
- Your local SQLite database;
- Your local search index and locally generated embeddings;
- Your local version history and Trash contents;
- The contents of websites you browse through the built-in browser.

No Nexus account is required to use this core functionality.

## 1a. Information Nexus Does Collect (Nexus Cloud / AI Assistant)

If you create a Nexus Cloud account to use the AI Assistant, Nexus **does** collect and store, on a server-side database it operates:

- Your email address;
- A hashed (not plaintext) form of your account password;
- A hashed form of your Nexus Cloud API key;
- Usage metadata associated with your account, such as token counts per request and request timestamps, used to enforce usage limits;
- Rate-limiting records (e.g., counts of recent requests) tied to your account or IP address;
- If you request a password reset: a hashed reset code and its expiration time, and your email address is used to send you that code.

Nexus also necessarily receives the content of each AI Assistant request you submit (such as your question, retrieved note excerpts, and, where enabled, text from open browser tabs) in order to forward it to the third-party AI provider described in Section 4 and return the response to you. See Section 4 for how that content is handled.

---

## 2. Local Storage

Nexus is designed to store your notes workspace locally on your device.

Your notes and related workspace information are stored in local files and databases on your computer.

This may include:

- Notes;
- Folders;
- Tags;
- Wiki links;
- Backlinks;
- Version history;
- Trash;
- Search indexes;
- Local embeddings;
- Browser-related application data;
- Locally saved AI conversation history; and
- Other application settings.

This information is stored locally rather than being uploaded to a Nexus cloud service, except to the extent it is submitted as part of an AI Assistant request as described in Section 4.

You are responsible for securing your device and maintaining backups of important information.

---

## 3. Local Search and Embeddings

Nexus provides search functionality, including semantic or meaning-based search.

Where semantic search is used, the embedding model runs locally on your device.

Your notes are not sent to a Nexus-operated server merely to perform local searches or generate local embeddings.

The resulting search indexes and embeddings are stored locally as part of your Nexus workspace.

---

## 4. AI Assistant and the Nexus Cloud Service

The AI Assistant is powered by the **Nexus Cloud Service**, a backend Nexus operates (currently a Cloudflare Worker with an associated database). This is not a "bring your own key" feature, and Nexus does not currently offer an alternative where you supply your own third-party AI provider key.

### How it works

1. You create a Nexus Cloud account (email and password) or sign in to an existing one. Nexus issues you a Nexus Cloud API key.
2. When you submit a message to the AI Assistant, your device sends the request — including relevant portions of your notes and, if you have the "aware of tabs" setting enabled, text from your currently open browser tabs — to the Nexus Cloud Service, authenticated with your Nexus Cloud API key.
3. The Nexus Cloud Service forwards your request to a third-party AI provider (currently accessed via OpenRouter), using API credentials that belong to Nexus, and receives the generated reply.
4. The Nexus Cloud Service returns the reply to your device, where it is saved locally as part of your conversation history.
5. The Nexus Cloud Service records the token usage associated with your account (to enforce usage limits) and timestamps of your requests. It does not intentionally retain the full text of your requests or responses beyond what is needed to generate and return the reply, but see Section 4 below on the AI provider's own handling.

### What this means for you

- Your request content is processed on a Nexus-operated server before it reaches the AI provider — this is different from a local-only or peer-to-peer architecture, and different from a "bring your own key" architecture where your device would talk to the provider directly.
- Nexus does not currently sell the content of your requests, and does not use them to train its own models, but the content does pass through infrastructure Nexus operates and is also processed by the third-party AI provider.
- The AI provider used by the Nexus Cloud Service is selected and paid for by Nexus. You do not have a direct account with that provider through this feature, so you should not expect that provider's own end-user privacy controls to apply to you individually; instead, Nexus's use of that provider is governed by the agreement between Nexus and the provider.

---

## 5. AI Provider Privacy

The third-party AI provider used by the Nexus Cloud Service is an independent company.

That provider may process requests it receives from the Nexus Cloud Service according to its own data-handling practices, to the extent Nexus's agreement with it allows.

Nexus does not control the internal security or data-processing practices of that provider.

---

## 6. Nexus Cloud API Keys and Account Credentials

Your Nexus Cloud API key (issued after signup or login) is stored locally on your device using security facilities provided by your operating system where available.

Your account itself — including your email address, a hashed form of your password, and a hashed form of your API key — is stored on the Nexus Cloud Service's server-side database, not solely on your device.

You are responsible for protecting your device and your account credentials.

If you believe your Nexus Cloud account has been compromised, you can regenerate your API key from within the Software, or contact us using the information below.

---

## 7. Browser

Nexus includes a built-in web browser.

When you visit a website through the Nexus browser, your browser requests may communicate directly with the website and other services operated by third parties.

Those websites may collect information such as:

- IP address;
- Browser and device information;
- Cookies;
- Authentication information;
- Usage information; and
- Other information according to their own privacy policies.

Nexus does not control the privacy practices of websites that you visit.

Your use of those websites is governed by their respective terms and privacy policies.

Separately, if you have the AI Assistant's "aware of tabs" setting enabled, text extracted from pages you have open may be sent to the Nexus Cloud Service as described in Section 4.

---

## 8. Websites and External Services

Nexus may provide links or functionality that allows you to interact with external websites and services.

External websites and services are not operated by Nexus.

Nexus is not responsible for:

- Their privacy practices;
- Their security;
- Their availability;
- Their content;
- Their data retention;
- Their use of cookies;
- Their collection of personal information; or
- Their compliance with applicable privacy laws.

You should review the privacy policy of each external service you use.

---

## 9. Backups and Exports

Nexus is designed so that backups and exports of your local notes workspace are controlled by you.

If you export your notes, copy your workspace, or create a backup, the resulting files are under your control.

If you upload those files to another service, send them to another person, or store them using a cloud-storage provider, that provider may process the information according to its own policies.

Nexus does not control what happens to your data after you intentionally transfer it outside the application.

---

## 10. No Cloud Synchronization of Your Notes Workspace

Nexus does not currently provide automatic cloud synchronization or backup of your local notes workspace.

Your notes, folders, and local search index do not automatically leave your device.

This is distinct from the Nexus Cloud Service described in Section 4, which handles AI Assistant account and request data, and which does involve a Nexus-operated server by design.

If cloud synchronization of your notes workspace is introduced in a future version of Nexus, the applicable privacy practices will be disclosed before or when that feature becomes available, as required by applicable law.

---

## 11. Website, Downloads, and GitHub

The Nexus desktop application is separate from websites, repositories, download services, and other infrastructure used to distribute Nexus.

For example, Nexus may use third-party services such as GitHub to host source code, documentation, releases, or issue trackers.

Those services may collect information according to their own privacy policies.

Nexus does not control the information collected by third-party hosting or distribution platforms.

If you interact with Nexus through a third-party platform, that platform's privacy policy applies to the information it collects.

---

## 12. Analytics and Telemetry

Nexus is designed to avoid unnecessary analytics and telemetry in the core desktop application.

Nexus does not intentionally collect the contents of your local notes, workspace, or local search index for analytics purposes.

The Nexus Cloud Service does record usage metadata (token counts, timestamps, rate-limit counters) associated with your account as described in Section 1a, which is necessary to operate that service — this is distinct from general analytics or telemetry about your device or app usage.

If future versions of Nexus introduce optional or necessary telemetry, diagnostics, crash reporting, or additional analytics, Nexus will provide appropriate information about such functionality and, where required, obtain appropriate consent or provide applicable controls.

---

## 13. Crash Reports and Diagnostics

Nexus may in the future provide optional diagnostic or crash-reporting functionality.

If such functionality is introduced, the information collected will be described in the applicable documentation or user interface.

Nexus does not intentionally include the contents of your private workspace in a crash report unless you explicitly choose to provide that information.

---

## 14. Security

Nexus is designed to minimize unnecessary transmission of user data, but the AI Assistant necessarily depends on the Nexus Cloud Service described in Section 4.

No software or computer system can be guaranteed to be completely secure.

Your device, operating system, installed software, network connection, the Nexus Cloud Service, the third-party AI provider, browser websites, and other third-party services may introduce security risks outside Nexus's control.

You are responsible for:

- Securing your device;
- Using appropriate operating-system security;
- Protecting your Nexus Cloud account credentials and API key;
- Maintaining backups;
- Keeping software updated; and
- Deciding what information to submit to the AI Assistant or to external websites.

---

## 15. Children's Privacy

Nexus is not specifically directed at children.

You should not use Nexus, or create a Nexus Cloud account, in violation of applicable age requirements or laws in your jurisdiction.

If you are a parent or guardian and believe a child has provided personal information to Nexus (for example, by creating a Nexus Cloud account), you may contact us using the information below.

---

## 16. International Users

Nexus is developed by Nawrass Andaloussi Dahman in Morocco and may be used internationally.

Your local notes workspace is not transferred to Nexus-operated servers in another country by default.

If you use the AI Assistant, your account information and request content are processed by the Nexus Cloud Service and the third-party AI provider it uses, which may operate in countries different from your own.

---

## 17. Your Privacy Rights

Depending on where you live, you may have legal rights concerning personal information processed by a service provider, including the account information (such as your email address) processed by the Nexus Cloud Service.

You may request access to, correction of, or deletion of your Nexus Cloud account information by contacting us using the information below.

Because your local notes workspace is not stored on Nexus-operated servers, it remains under your direct control on your device and is not something Nexus can access, export, or delete on your behalf.

Nothing in this Privacy Policy is intended to limit rights that cannot legally be limited under applicable law.

---

## 18. Changes to This Privacy Policy

This Privacy Policy may be updated from time to time.

If material changes are made, we may provide notice through the Nexus website, Software, repository, or another appropriate method.

The "Last Updated" date at the beginning of this Privacy Policy indicates when it was most recently revised.

---

## 19. Contact

Privacy questions and requests may be directed to:

**Nawrass Andaloussi Dahman**  
Developer and Creator of Nexus  
Morocco

**Email:** getnexusupport@gmail.com

---

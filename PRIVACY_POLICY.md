# Nexus Privacy Policy

**Last updated: October 1, 2026**

Nexus is developed and operated by **Nawrass Andaloussi Dahman**, an independent software developer based in Morocco.

This Privacy Policy explains how Nexus handles information when you use the Nexus desktop application (version 6.1.0 and later, "Nexus" or the "Software") and the Nexus Cloud Service that powers the optional AI Assistant.

Nexus's notes and workspace are local-first: your notes stay on your device unless you export or back them up. The **AI Assistant is different**: it requires a Nexus Cloud account and is powered by a server that Nexus operates.

## 1. What Stays on Your Device

When you use notes, folders, tags, links, the graph, search, and the browser, the following is stored on your device and is not uploaded to a Nexus-operated server as part of ordinary local operation:

- Your notes, folders, tags, and links between notes;
- Images you insert into notes;
- Version history and Trash;
- Local search indexes and embeddings generated on your device;
- Your AI Assistant conversations, which are saved in the local database and associated with the email address of the Nexus Cloud account that was signed in;
- Your settings, browser bookmarks, and downloaded-file information stored in the application's local browser storage; and
- Your Nexus Cloud API key, which is stored using your operating system's credential storage, such as Windows Credential Manager or the macOS Keychain.

No Nexus account is required to use these local features.

## 2. Information Nexus Collects (Nexus Cloud / AI Assistant)

If you create a Nexus Cloud account to use the AI Assistant, Nexus does store the following in the Nexus Cloud Service:

- Your email address;
- A salted hash of your password;
- A hash of your current API key;
- Account-security information such as key-generation counts and failed sign-in information;
- Usage information such as token counts and request timestamps;
- Rate-limiting information;
- Temporary password-reset information, including an appropriately protected reset-code value and expiry information; and
- Operational information necessary to maintain, secure, and debug the service.

Your API key itself is stored on your device using your operating system's credential storage. The server stores a hash of the key rather than relying on the local plaintext credential.

Nexus does not store your local notes, folders, local search index, or local conversation history as a synchronized cloud workspace.

## 3. What Is Sent When You Use the AI Assistant

The AI Assistant requires the Nexus Cloud Service. When you submit a request, the Nexus Cloud Service may receive:

- Your new message;
- Up to 20 prior conversation messages;
- Relevant excerpts from notes available to the Assistant;
- The full contents of a note when you specifically identify that note by title;
- The current date and time; and
- Text from pages open in Nexus Browser when that text is included under the applicable browser settings.

The Nexus Cloud Service forwards applicable request content to a third-party AI provider, currently Google through its Gemini models.

The AI model may use web search. Search queries may be sent to Jina AI, and the Nexus Cloud Service may retrieve the text of relevant result pages.

The resulting AI response is returned to your device and your conversation history is stored locally as part of Your Content.

Nexus records usage information such as token usage and request timestamps for account management, rate limiting, and service operation. Nexus does not maintain your complete AI conversation history as a server-side conversation database.

## 4. Third-Party Providers

Nexus uses independent third-party providers to operate portions of its services:

- **Google / Gemini:** third-party AI model provider.
- **Jina AI:** web search provider used by AI Assistant web-search functionality.
- **Resend:** transactional email provider, including password-reset messages where applicable.
- **Cloudflare:** hosting and infrastructure provider for the Nexus Cloud Service.
- **DuckDuckGo:** favicon provider used by the Nexus Browser.

These providers operate independently and may process information under their own terms and policies. Nexus does not control the internal processing practices of those providers.

Nexus uses its own service credentials when communicating with the third-party AI provider. Your Nexus API key is not provided to the third-party AI provider as your own provider credential.

## 5. Account Security

Nexus stores passwords using salted password hashes rather than storing your password in plaintext.

Your Nexus Cloud API key is stored locally using operating-system credential storage such as Windows Credential Manager or the macOS Keychain.

Each successful sign-in may generate a new API key and invalidate the previous key. Nexus may limit API-key regeneration to three times within a relevant period.

Password-reset codes are temporary and may expire after 30 minutes.

Nexus takes reasonable measures appropriate to the service to protect account information. However, no online service or storage system can be guaranteed to be completely secure.

You are responsible for protecting your device, credentials, and API key.

## 6. Retention and Deleting Your Account

You may permanently delete your Nexus Cloud account through the available account settings.

When you delete your account, Nexus deletes the account record, usage history, and password-reset records from the active Nexus Cloud Service and immediately invalidates the account's API key.

Rate-limiting counters, operational logs, and hosting-provider backups may remain for a limited period where necessary for security, abuse prevention, disaster recovery, accounting, or legal obligations.

Such retained information is not maintained as your active Nexus Cloud account and is subject to applicable retention and deletion practices.

Deleting your Nexus Cloud account does not delete notes, conversations, files, bookmarks, or other Your Content stored locally on your device.

## 7. Local Search, Embeddings, and On-Device Models

Nexus may create local search indexes and embeddings from content stored on your device. These indexes and embeddings are stored locally and are used to support local search and related features.

Some Nexus features use small AI models downloaded to your device from public model-hosting infrastructure. Processing performed by those models may occur locally.

Downloading a model file from a public model host is separate from transmitting your notes or AI Assistant requests to the Nexus Cloud Service.

## 8. Built-In Browser

The Nexus Browser connects directly from your device to the websites that you visit. Those websites have their own privacy policies and terms.

Searches typed as non-URL queries into the browser address bar are sent to Brave Search.

Site icons are requested from DuckDuckGo.

Websites may store cookies and other site data on your device. Nexus does not currently provide a separate control for clearing all third-party website cookies and site data.

Nexus may retrieve and read the text of pages open in Nexus Browser tabs from your device even when the "Aware of tabs" setting is turned off. This can support local browser functionality such as conflict detection.

Turning off "Aware of tabs" prevents page text from being automatically included in AI Assistant requests and sent to the Nexus Cloud Service through that feature.

Turning off the setting does not necessarily prevent local browser functionality from retrieving or analyzing page text on your device.

## 9. External Websites and Linked Images

Nexus may allow you to access external websites or load externally hosted content.

When you access an external website, information such as your IP address, browser characteristics, cookies, or other request information may be transmitted directly to that website according to its own policies.

Nexus does not control the privacy practices, security, availability, or content of external websites.

You are responsible for reviewing the privacy policies and terms of external services that you choose to use.

## 10. Backups, Exports, and Clearing Data

Nexus is local-first, so you are responsible for backing up important local content.

Nexus may provide export and backup functionality. You are responsible for verifying that exported and backed-up data is complete and usable.

Using a device-level cleanup tool, uninstalling the application, or clearing application storage may delete local content.

Nexus does not guarantee recovery of local content after accidental deletion, device failure, corruption, storage failure, or other circumstances outside Nexus's reasonable control.

The application may also provide a "Clear All Data" feature. Using that feature may permanently delete local Nexus data from the device.

## 11. No Cloud Synchronization of Your Notes

Nexus does not currently provide automatic cloud synchronization of your local notes and workspace.

Your local notes, folders, tags, links, images, version history, local indexes, embeddings, and locally stored AI conversation history remain on your device unless you explicitly export, back up, or otherwise transmit them.

This does not mean that information is never transmitted. AI Assistant requests and other explicitly cloud-based functionality operate through the Nexus Cloud Service as described in this policy.

## 12. Website, Downloads, and GitHub

The Nexus Website may use hosting, deployment, repository, analytics, or other infrastructure provided by third parties.

Where applicable, the Nexus Website may be hosted or deployed using services such as Vercel or GitHub.

Those services may process technical information according to their own policies when you access their infrastructure or resources.

## 13. Analytics, Telemetry, and Crash Reports

Nexus does not currently use desktop analytics, behavioral telemetry, or automatic crash-reporting services to monitor your local workspace.

This does not prevent the Nexus Cloud Service or hosting providers from maintaining operational logs necessary to provide, secure, rate-limit, and troubleshoot online services.

Operational logs may contain information such as IP addresses, timestamps, requested URLs, error information, and limited request metadata.

## 14. Security and Children

Nexus is intended for users who are at least 16 years old.

Nexus does not knowingly target children under 16 with account-based services.

If you believe a person under the applicable minimum age has created an account without appropriate authorization, please contact Nexus using the contact information below.

No online system can guarantee absolute security. You should avoid submitting highly sensitive information to the AI Assistant unless you understand and accept the applicable transmission and processing.

## 15. International Users and Your Rights

Nexus is developed in Morocco and may be used internationally.

Your local notes are not transferred to Nexus-operated servers merely because you use the local-first features of the Software.

If you use the AI Assistant, your account information and request content are processed by the Nexus Cloud Service and applicable third-party providers. Those providers may operate in countries other than the country where you live.

Depending on where you live, you may have legal rights concerning personal information, including rights to access, correction, deletion, restriction, objection, portability, or other rights provided by applicable law.

You can delete your Nexus Cloud account through the available settings and may contact Nexus to request access to or correction of account information.

Your local notes workspace is under your direct control and is not something Nexus can access, export, or delete for you through the Nexus Cloud Service.

Nothing in this policy limits rights that cannot legally be limited.

## 16. Changes to This Privacy Policy

This policy may be updated from time to time.

For material changes, Nexus may provide reasonable notice through the Website, Software, or another suitable method where required by law.

The "Last updated" date above shows when this policy was most recently revised.

## 17. Contact

Privacy questions and requests may be directed to:

**Nawrass Andaloussi Dahman**  
Developer and Creator of Nexus  
Morocco

**Email:** getnexusupport@gmail.com

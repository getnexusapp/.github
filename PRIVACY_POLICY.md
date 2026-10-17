# Nexus Privacy Policy

*Last updated: October 16, 2026*

Nexus is developed and operated by **Nawrasse Andaloussi Dahman**, an independent software developer based in Morocco.

"Nexus Software" is a trade name used by Nawrasse Andaloussi Dahman, not a separate legal entity.

This Privacy Policy explains how Nexus handles information when you use the Nexus desktop application (version 6.1.0 and later, "Nexus" or the "Software") and the Nexus Cloud Service that powers the optional AI Assistant.

Nexus's notes and workspace are local-first: your notes stay on your device unless you export or back them up. The **AI Assistant is different**: it requires a Nexus Cloud account and is powered by a server that Nexus operates.

Your use of Nexus is also governed by the [Nexus Software License](https://nexusworkspace.net/software-license) and, for the Nexus website and Nexus Cloud Service, the Nexus Terms of Service. Capitalized terms used but not defined in this Privacy Policy, such as "Your Content" and "Nexus Cloud Service," have the meanings given to them in the Nexus Software License.

This Privacy Policy also covers **Nova**, the optional command-line tool for Nexus, published as **@getnexus/nova**. Section 17 explains what Nova stores and sends. Nova is governed by the [Nova CLI License](https://nexusworkspace.net/nova-license) as well as the documents listed above.

## 1. What Stays on Your Device

When you use notes, folders, tags, links, the graph, search, and the browser, the following is stored on your device and is not uploaded to a Nexus-operated server as part of ordinary local operation:

- Your notes, folders, tags, and links between notes;
- Images you insert into notes;
- Version history and Trash;
- Local search indexes and embeddings generated on your device;
- Your AI Assistant conversations, which are saved in the local database and associated with the email address of the Nexus Cloud account that was signed in;
- Your settings, browser bookmarks, and downloaded-file information stored in the application's local browser storage; and
- Your Nexus Cloud API key, which is stored using your operating system's credential storage, such as Windows Credential Manager, the macOS Keychain, or equivalent secure storage on other supported platforms.

No Nexus account is required to use these local features.

If you sign in using Nova, Nova also keeps its own copy of your session key in a file on your computer. See Section 17.

## 2. Information Nexus Collects (Nexus Cloud / AI Assistant)

If you create a Nexus Cloud account to use the AI Assistant, Nexus does store the following in the Nexus Cloud Service:

- your email address and the account identifier provided by your sign-in provider (Google or GitHub);
- a hash of your current API key;
- account-security information such as key-generation counts;
- usage information such as token counts and request timestamps;
- rate-limiting information; and
- operational information necessary to maintain, secure, and debug the service.

Nexus Cloud accounts are created and accessed only by signing in with Google or GitHub; there is no separate email-and-password sign-in. If you sign in and no Nexus Cloud account exists for you, Nexus creates one automatically using the information your provider shares, such as your verified email address and an account identifier. If you already have an account, you are signed in to it. Nexus does not receive or store your Google or GitHub password.

Your API key itself is stored on your device using your operating system's credential storage. The server stores a hash of the key rather than relying on the local plaintext credential.

Nexus does not store your local notes, folders, local search index, or local conversation history as a synchronized cloud workspace.

## 3. What Is Sent When You Use the AI Assistant

The AI Assistant requires the Nexus Cloud Service. When you submit a request, the Nexus Cloud Service may receive:

- your new message;
- up to 20 prior conversation messages;
- relevant excerpts from notes available to the Assistant;
- up to a limited portion of a note's text when relevant-excerpt retrieval is unavailable;
- the full contents of a note when you specifically identify that note by title;
- the current date and time; and
- text from pages open in Nexus Browser when that text is included under the applicable browser settings.

Notes that you mark "AI: Off" are not intentionally included in AI Assistant requests, either as stored contents or as automatically retrieved excerpts. However, "AI: Off" does not prevent transmission of anything you personally type, paste, quote, or otherwise submit to the AI Assistant, and it does not retroactively remove content you previously submitted in an AI conversation.

The Nexus Cloud Service forwards applicable request content to a third-party AI provider, currently Google through its Gemini models. As explained in Section 4, Google may use that content to train its models.

The AI model may use web search. Search queries may be sent to Jina AI, and the Nexus Cloud Service may retrieve the text of relevant result pages.

The resulting AI response is returned to your device and your conversation history is stored locally as part of Your Content.

Nexus records usage information such as token usage and request timestamps for account management, rate limiting, and service operation. Nexus does not maintain your complete AI conversation history as a server-side conversation database.

## 4. Google Model Training and Your Consent

The Nexus Cloud Service currently forwards AI Assistant requests to Google, which provides the Gemini models. Content included in those requests, which may include your messages, prior conversation messages, note excerpts, the contents of notes you identify, and text from pages open in Nexus Browser, may be used by Google to train and improve its AI models, under Google's own terms and privacy practices.

**BY CREATING A NEXUS CLOUD ACCOUNT OR USING THE AI ASSISTANT, YOU ACKNOWLEDGE AND AGREE THAT GOOGLE MAY USE CONTENT SENT THROUGH NEXUS CLOUD AI REQUESTS TO TRAIN AND IMPROVE ITS MODELS. IF YOU DO NOT AGREE, DO NOT CREATE A NEXUS CLOUD ACCOUNT OR USE THE AI ASSISTANT.**

Nexus itself does not use your content to train AI models. Nexus does not control how Google uses information it receives.

Content that stays on your device is not sent to Google through the Nexus Cloud Service. This includes local notes you have not submitted to the AI Assistant, notes marked "AI: Off" (except for anything you type or paste into the Assistant yourself), and content processed by on-device models.

You can stop at any time by no longer using the AI Assistant or by deleting your Nexus Cloud account. However, Nexus cannot recall or delete content that has already been sent to Google, and deleting your account does not reverse any use Google has already made of that content. You should not submit confidential information, information you do not have the right to share, or other people's personal information to the AI Assistant.

## 5. Third-Party Providers

Nexus uses independent third-party providers to operate portions of its services:

- **Google / Gemini:** third-party AI model provider; see Section 4 for how Google may use content sent to its models.
- **Jina AI:** web search provider used by AI Assistant web-search functionality.
- **Cloudflare:** hosting and infrastructure provider for the Nexus Cloud Service.
- **Vercel:** hosting provider for the Nexus Website. Vercel receives ordinary request information, such as your IP address and browser details, when you visit the website.
- **UptimeRobot:** monitors the availability of Nexus services and provides the uptime data shown on the status page.
- **Google and GitHub (sign-in):** third-party authentication providers used to create and access Nexus Cloud accounts.
- **Brave Search:** search provider for non-URL queries typed into the Nexus Browser address bar.
- **DuckDuckGo:** favicon provider used by the Nexus Browser.
- **Hugging Face and jsDelivr:** distribution infrastructure for on-device model files and related components.
- **GitHub:** update distribution and, where applicable, website or repository hosting.
- **npm:** distribution infrastructure for the Nova command-line tool. npm receives ordinary network request information when you install Nova.

These providers operate independently and may process information under their own terms and policies. Nexus does not control the internal processing practices of those providers.

Nexus uses its own service credentials when communicating with the third-party AI provider. Your Nexus API key is not provided to the third-party AI provider as your own provider credential.

## 6. Account Security

Sign-in is handled by the provider you choose (Google or GitHub). Nexus does not receive or store your Google or GitHub password.

Your Nexus Cloud API key is stored locally using operating-system credential storage such as Windows Credential Manager, the macOS Keychain, or equivalent secure storage on other supported platforms.

Each successful sign-in may generate a new API key and invalidate the previous key. Nexus may limit API-key regeneration to three times within a relevant period.

Nexus takes reasonable measures appropriate to the service to protect account information. However, no online service or storage system can be guaranteed to be completely secure.

You are responsible for protecting your device, your Google or GitHub account, your credentials, and your API key.

## 7. Retention and Deleting Your Account

You may permanently delete your Nexus Cloud account through the available account settings.

When you delete your account, Nexus deletes the account record and usage history from the active Nexus Cloud Service and immediately invalidates the account's API key.

Rate-limiting counters, operational logs, and hosting-provider backups may remain for a limited period where necessary for security, abuse prevention, disaster recovery, accounting, dispute resolution, record-keeping, or legal obligations.

Such retained information is not maintained as your active Nexus Cloud account and is subject to applicable retention and deletion practices.

Deleting your Nexus Cloud account does not delete notes, conversations, files, bookmarks, or other Your Content stored locally on your device.

## 8. Local Search, Embeddings, and On-Device Models

Nexus may create local search indexes and embeddings from content stored on your device. These indexes and embeddings are stored locally and are used to support local search and related features.

Some Nexus features use small AI models downloaded to your device from public model-hosting infrastructure, such as Hugging Face or jsDelivr. Processing performed by those models may occur locally.

Those hosts may receive your IP address and ordinary network request information when your device connects to them to download model files.

Downloading a model file from a public model host is separate from transmitting your notes or AI Assistant requests to the Nexus Cloud Service.

## 9. Built-In Browser

The Nexus Browser connects directly from your device to the websites that you visit. Those websites have their own privacy policies and terms.

Searches typed as non-URL queries into the browser address bar are sent to Brave Search.

Site icons are requested from DuckDuckGo.

Websites may store cookies and other site data on your device. Nexus does not currently provide a separate control for clearing all third-party website cookies and site data.

Nexus may retrieve and read the text of pages open in Nexus Browser tabs from your device even when the "Aware of tabs" setting is turned off. This can support local browser functionality such as conflict detection.

Turning off "Aware of tabs" prevents page text from being automatically included in AI Assistant requests and sent to the Nexus Cloud Service through that feature.

Turning off the setting does not necessarily prevent local browser functionality from retrieving or analyzing page text on your device.

## 10. External Websites and Linked Images

Nexus may allow you to access external websites or load externally hosted content.

When you access an external website, information such as your IP address, browser characteristics, cookies, or other request information may be transmitted directly to that website according to its own policies.

Nexus does not control the privacy practices, security, availability, or content of external websites.

You are responsible for reviewing the privacy policies and terms of external services that you choose to use.

## 11. Backups, Exports, and Clearing Data

Nexus is local-first, so you are responsible for backing up important local content.

Nexus may provide export and backup functionality. You are responsible for verifying that exported and backed-up data is complete and usable.

Using a device-level cleanup tool, uninstalling the application, or clearing application storage may delete local content.

Nexus does not guarantee recovery of local content after accidental deletion, device failure, corruption, storage failure, or other circumstances outside Nexus's reasonable control.

The application may also provide a "Clear All Data" feature. Using that feature may permanently delete local Nexus data from the device.

## 12. No Cloud Synchronization of Your Notes

Nexus does not currently provide automatic cloud synchronization of your local notes and workspace.

Your local notes, folders, tags, links, images, version history, local indexes, embeddings, and locally stored AI conversation history remain on your device unless you explicitly export, back up, or otherwise transmit them.

This does not mean that information is never transmitted. AI Assistant requests and other explicitly cloud-based functionality operate through the Nexus Cloud Service as described in this policy.

## 13. Website, Downloads, Updates, and GitHub

The Nexus Website may use hosting, deployment, repository, analytics, or other infrastructure provided by third parties.

The Nexus Website is hosted on Vercel. The status page at status.nexusworkspace.net uses uptime data from UptimeRobot, which Nexus retrieves from its servers; your browser does not contact UptimeRobot when you view the page.

Nexus may periodically check for updates by contacting an update-distribution service such as GitHub. Update requests may disclose your IP address and ordinary network request information to the relevant provider.

Those services may process technical information according to their own policies when you access their infrastructure or resources.

## 14. Analytics, Telemetry, and Crash Reports

Nexus does not currently use desktop analytics, behavioral telemetry, or automatic crash-reporting services to monitor your local workspace.

This does not prevent the Nexus Cloud Service or hosting providers from maintaining operational logs necessary to provide, secure, rate-limit, and troubleshoot online services.

Operational logs may contain information such as IP addresses, timestamps, requested URLs, error information, and limited request metadata.

## 15. Security and Children

Nexus is intended for users who are at least 16 years old.

Nexus does not knowingly target children under 16 with account-based services.

If you believe a person under the applicable minimum age has created an account without appropriate authorization, please contact Nexus using the contact information below.

No online system can guarantee absolute security. You should avoid submitting highly sensitive information to the AI Assistant unless you understand and accept the applicable transmission and processing.

## 16. International Users and Your Rights

Nexus is developed in Morocco and may be used internationally.

Nexus processes personal data in accordance with Moroccan Law No. 09-08 on the protection of individuals with regard to the processing of personal data, which is supervised by the Commission Nationale de contrôle de la protection des Données à caractère Personnel (CNDP), and with other laws that apply to it.

Where Law No. 09-08 applies to you, you have the right to be informed about the processing of your personal data and to access, rectify, and object, on legitimate grounds, to that processing. You can exercise these rights by contacting Nexus using the contact information below, and you may also contact the CNDP.

Your local notes are not transferred to Nexus-operated servers merely because you use the local-first features of the Software.

If you use the AI Assistant, your account information and request content are processed by the Nexus Cloud Service and applicable third-party providers. Those providers, including Google, may operate in countries other than the country where you live, including outside Morocco. By creating a Nexus Cloud account or using the AI Assistant, you consent to these transfers and to the processing described in this policy.

Depending on where you live, you may have legal rights concerning personal information, including rights to access, correction, deletion, restriction, objection, portability, or other rights provided by applicable law.

You can delete your Nexus Cloud account through the available settings and may contact Nexus to request access to or correction of account information.

Your local notes workspace is under your direct control and is not something Nexus can access, export, or delete for you through the Nexus Cloud Service.

Nothing in this policy limits rights that cannot legally be limited.

## 17. Nova Command-Line Tool

Nova is an optional command-line tool for Windows that installs, updates, and signs in to Nexus. You do not need Nova to use Nexus. This section describes what Nova stores and sends. Nova never opens or reads your Nexus notes database, and it does not send Your Content to Nexus Cloud or anyone else.

### What Nova stores on your device

- **Its own session.** After you sign in, Nova saves a file at `%APPDATA%\nova\credentials.json` containing your Nexus Cloud session key, the time it was saved, your account email (when available), and whether the session was shared with the Nexus app. This is an ordinary file protected by the permissions of your Windows user account. Unlike the Nexus app's own copy of the key, Nova does not encrypt it or store it in Windows Credential Manager.
- **A copy for the Nexus app.** So that the app is signed in too, Nova writes the same key to Windows Credential Manager, where the Nexus app reads it.
- **Temporary installer files.** Nova downloads Nexus installers to your system's temporary folder. It deletes the file after a passive or silent install. For a normal interactive install, the file remains while the installer runs.

Running `nova logout` revokes the session on the Nexus Cloud Service, deletes Nova's credential file, and, if the session was shared with the app, removes the app's copy from Windows Credential Manager.

### What Nova reads on your device

To tell whether Nexus is installed, which version it is, and whether it is running, Nova reads Windows' installed-program records and looks in the usual install folders. It also checks the list of running programs for Nexus. To sign the app in, it runs a short Windows PowerShell step that writes to Credential Manager, and it passes the key to that step through the environment rather than a command line.

### What Nova sends, and to whom

- **GitHub.** Nova requests the Nexus release information and downloads the installer from GitHub. GitHub receives your IP address and ordinary request information, including a user-agent identifying the Nova version. If you set a `GITHUB_TOKEN` environment variable, Nova sends it to GitHub's API to avoid rate limits, and only there.
- **Nexus Cloud.** For sign-in, Nova sends the provider you chose and a hash of a random secret it generated, and later the sign-in session identifier and the secret itself to collect the result. After sign-in, Nova sends your session key to Nexus Cloud to fetch your account details and usage, to sign out, and, without the key, to check service health. These requests are handled like other Nexus Cloud requests, as described in Section 2 and Section 14, and may appear in operational logs with information such as IP address and timestamps.
- **Google or GitHub (sign-in).** You authenticate with the provider in your browser. Nova never sees your password.
- **Your browser.** Nova can open Nexus pages and the sign-in link in your default browser.

Nova includes no analytics, telemetry, or crash reporting. After you install it, Nova does not contact npm.

### Your choices

Sign-in is optional. You can sign out at any time with `nova logout`, delete your Nexus Cloud account as described in Section 7, or uninstall Nova with `npm uninstall -g @getnexus/nova`, which removes only the command-line tool and does not affect Nexus or your notes.

## 18. Changes to This Privacy Policy

This policy may be updated from time to time.

For material changes, Nexus may provide reasonable notice through the Website, Software, or another suitable method where required by law.

The "Last updated" date above shows when this policy was most recently revised.

## 19. Contact

Privacy questions and requests may be directed to:

**Nawrasse Andaloussi Dahman**\
Operator of Nexus\
Morocco

**Email:** [support@nexusworkspace.net](mailto:support@nexusworkspace.net)

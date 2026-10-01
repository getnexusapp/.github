# Nexus End User License Agreement

**Last Updated: October 1, 2026**

This End User License Agreement ("Agreement") is a legal agreement between you, either an individual or an entity you represent ("You" or "User"), and **Nawrass Andaloussi Dahman**, an individual developer based in Morocco and the creator and operator of the Nexus software ("Operator," "We," "Us," or "Our").

> **Nexus is currently an independently developed product operated by Nawrass Andaloussi Dahman. No corporation named "Nexus, Inc." operates the Software or is a party to this Agreement. If Nexus is later transferred to or operated by a separate legal entity, this Agreement may be updated accordingly.**

> **BY DOWNLOADING, INSTALLING, ACCESSING, OR USING THE SOFTWARE, YOU ACKNOWLEDGE THAT YOU HAVE READ, UNDERSTOOD, AND AGREE TO BE BOUND BY THIS AGREEMENT. IF YOU DO NOT AGREE, DO NOT DOWNLOAD, INSTALL, ACCESS, OR USE THE SOFTWARE.**

This Agreement governs your download, installation, access to, and use of the Nexus Application on supported desktop and mobile devices, including its software, features, updates, and accompanying documentation, as well as your use of the Nexus Cloud Service described in Section 5, where applicable.

---

## 1. Definitions

**"Nexus"** means the software, applications, services, and related products made available by the Operator under the Nexus name.

**"Nexus Application"** means the official Nexus software applications made available by the Operator for supported desktop and mobile platforms, including Windows, macOS, Linux, iOS, and Android, together with any updates, upgrades, and related components provided by the Operator.

**"Software"** means the Nexus Application in object-code form, including its features, user interface, notes editor, built-in browser, knowledge graph, AI Assistant interface, updates, documentation, and other components made available as part of the Nexus Application. It does not include source code that is not expressly licensed to you.

**"Your Content"** means notes, text, images, files, bookmarks, AI conversation history, browser-related content, and other content you create, import, access, or store using the Software.

**"Nexus Cloud Service"** means the backend service operated by the Operator under the Nexus name, including the infrastructure and systems used to provide account creation and sign-in, AI request processing, forwarding of AI requests to third-party providers, web search for the Assistant, usage tracking, rate limiting, and password-reset email delivery.

**"Third-Party Provider"** means an external service or provider used with the Software or Nexus Cloud Service, including providers of AI models, web search, email delivery, hosting, content retrieval, authentication, analytics, or other infrastructure or services used to operate or support Nexus.

## 2. Grant of License

Subject to your compliance with this Agreement, the Operator grants you a limited, non-exclusive, non-transferable, non-sublicensable, revocable license to download, install, and use the Software in object-code form for your personal or internal business purposes on supported devices that you own or are authorized to control.

This license does not transfer ownership of the Software or any intellectual property rights to you. All rights not expressly granted are reserved.

## 3. Restrictions

You shall not, and shall not knowingly permit or assist any third party to:

- copy, modify, translate, or create derivative works based on the Software, except as expressly permitted by applicable law;
- reverse engineer, decompile, disassemble, or attempt to derive source code from the Software, except to the extent applicable law expressly permits such activity;
- distribute, sell, rent, lease, sublicense, or otherwise make the Software available to third parties;
- remove or alter proprietary notices, copyright notices, or branding;
- bypass, disable, defeat, or interfere with security mechanisms, authentication, rate limits, or usage restrictions;
- use automated scripts, bots, or similar mechanisms to abuse or overload the Nexus Cloud Service;
- use the Software or Nexus Cloud Service to develop or operate a competing service through unauthorized access to, extraction of, or use of the Software, Nexus Cloud Service, or their proprietary components;
- use a Nexus Cloud API key outside the Nexus Software or in another application;
- access the Nexus Cloud Service through means other than the Nexus application or other expressly authorized interfaces; or
- use the Software or Nexus Cloud Service for unlawful purposes or to infringe the rights of others.

## 4. Ownership and Intellectual Property

The Software, including its object code, user interface, visual design, documentation, branding, and other proprietary components, is owned by or licensed to Nawrass Andaloussi Dahman and is protected by applicable intellectual property laws. Source code, where applicable, remains proprietary unless expressly made available under separate license terms.

Your Content remains your property. Nothing in this Agreement transfers ownership of Your Content to the Operator.

You grant the Operator only the limited rights necessary to provide the features and services you request, including processing AI Assistant requests through the Nexus Cloud Service and applicable third-party providers.

## 5. Nexus Cloud Service and AI Assistant

### (a) Local-First Architecture

Nexus is designed as a local-first application. Your notes and local workspace are stored on your device unless you explicitly export or back them up elsewhere.

Local data may include notes, folders, tags, links, images, version history, Trash contents, search indexes, embeddings, AI conversation history, browser settings, bookmarks, downloaded files, and other application data.

### (b) On-Device Models

Some Nexus features use small AI models that are downloaded to your device from public model-hosting infrastructure. Such models and the indexes they produce may operate locally without sending the underlying content to the Nexus Cloud Service.

Third-party model hosts may be involved in downloading model files. The download process is separate from sending your notes or AI requests to the Nexus Cloud Service.

### (c) AI Assistant Processing

The AI Assistant requires a Nexus Cloud account and uses the Nexus Cloud Service.

Depending on the request and enabled features, an AI Assistant request may contain:

- your new message;
- up to 20 prior conversation messages;
- relevant excerpts from notes available to the Assistant;
- the full contents of a note when you specifically identify that note by title;
- the current date and time; and
- text from pages open in Nexus Browser when that text is included under the applicable browser settings.

The Nexus Cloud Service forwards applicable request content to a third-party AI provider using credentials controlled by the Operator.

The AI model may search the web. Search queries may be sent to a third-party web-search provider, and the Nexus Cloud Service may retrieve the text of relevant result pages.

The Nexus Cloud Service applies rolling usage limits and per-minute rate limits. The Operator may decline, delay, or restrict requests that exceed applicable limits and may change those limits.

### (d) Nexus Cloud Account and Credential Storage

Your API key is stored on your device using your operating system's credential storage, such as Windows Credential Manager or the macOS Keychain.

Your account record, including your email address, a salted hash of your password, a hash of your API key, and usage information such as token counts and request timestamps, is stored by the Nexus Cloud Service.

The service may also maintain temporary password-reset records and short-lived rate-limiting information. Operational logs maintained by the Operator or its hosting provider may contain request metadata such as IP addresses, timestamps, URLs, error information, or search-query fragments.

You are responsible for protecting your device and credentials and for activity under your account, except to the extent caused by the Operator's own failure to maintain required security measures.

**Deleting your account.** You can permanently delete your Nexus Cloud account from the available account settings. Upon account deletion, the Operator will delete or otherwise dispose of account information and associated records in accordance with the Nexus Privacy Policy, subject to information that may be retained for security, abuse prevention, disaster recovery, legal obligations, or other legitimate operational purposes.

Rate-limiting counters, hosting-provider backups, and operational logs may remain for a limited period where necessary for security, abuse prevention, disaster recovery, or legal obligations.

Deleting your account does not delete Your Content stored locally on your device.

### (e) Third-Party Providers

The Nexus Cloud Service relies on independent Third-Party Providers. The Operator selects and pays for these providers. You do not receive a separate account with those providers through the Nexus Cloud Service.

The Operator does not control how third-party providers process information they receive and their own terms and policies may apply.

### (f) Local AI Conversation History

AI conversation history is saved locally as part of Your Content and is not maintained as a conversation-history database by the Nexus Cloud Service.

The Nexus Cloud Service and applicable Third-Party Providers do, however, process the content of each AI request and the resulting response while that request is being generated.

### (g) Built-In Browser

The Nexus Browser connects your device directly to the websites you visit. Those websites operate under their own privacy policies and terms.

Searches typed as non-URL queries into the browser address bar are sent to Brave Search. Site icons are requested from DuckDuckGo. Websites may store cookies and site data on your device.

Nexus may retrieve and read the text of pages open in Nexus Browser tabs on your device even when the "Aware of tabs" setting is off. This allows local browser features, including conflict detection, to operate.

Turning off "Aware of tabs" prevents that page text from being automatically included in AI Assistant requests and sent to the Nexus Cloud Service through that feature. It does not necessarily prevent local browser functionality from retrieving or analyzing page text.

### (h) Data Transmission Summary

Local operations such as notes storage, local search, version history, graph functionality, export, and local backup do not require transmission to the Nexus Cloud Service.

Using the AI Assistant does require transmission of the information needed to process your request. Using the browser requires communication with the websites you visit and, where applicable, search and favicon services.

You are responsible for determining what information you submit through the AI Assistant or to third-party websites.

## 6. Nexus Cloud Accounts

Some features require a Nexus Cloud account. You must provide accurate information when creating an account and must keep your credentials secure.

Each successful sign-in may issue a new API key and invalidate the previous key. Nexus may limit API-key regeneration to three times within a relevant period.

Password-reset codes may expire after 30 minutes and may only be used for their intended account.

If you believe your account has been compromised, you should stop using the affected credentials and use the available account-reset or regeneration functionality.

Account deletion does not delete local Your Content. See the Nexus Privacy Policy for additional information concerning account information and retention.

## 7. Backups and Data Loss

Nexus is local-first, and you are responsible for maintaining backups of important local content.

Nexus may provide backup and export functionality, but you are responsible for verifying that backup and export files are complete and usable.

The Operator does not guarantee recovery of local content following device failure, accidental deletion, corruption, operating-system failure, storage failure, or other events outside the Operator's reasonable control.

Clearing application data, uninstalling the Software, or using a device-level cleanup tool may delete local content. You should make a backup before taking actions that may remove local data.

## 8. Updates and Changes

The Operator may provide updates, fixes, security patches, or new features and may modify or discontinue the Nexus Cloud Service.

The Operator is not obligated to provide updates or continue supporting any particular version, feature, or the Nexus Cloud Service except as required by law.

Unless an update has separate terms, this Agreement applies to updated versions of the Software.

## 9. Term and Termination

This Agreement begins when you first download, install, access, or use the Software and continues until terminated.

The Operator may terminate or suspend your license, Nexus Cloud account, or access to the Nexus Cloud Service if you materially breach this Agreement, use the Software or service unlawfully, abuse usage limits, compromise service security, or otherwise create a material risk to the Operator or other users, subject to applicable law.

You may terminate this Agreement at any time by uninstalling the Software and ceasing to use it. You may also stop using the AI Assistant or delete your Nexus Cloud account without affecting your local workspace.

On termination, you must cease using the Software and, to the extent reasonably practicable, delete copies in your possession, except where retention is required by law or reasonably necessary for legitimate archival, backup, or record-keeping purposes.

Termination does not delete Your Content from your device.

Provisions concerning intellectual property, Third-Party Providers, disclaimers, limitations of liability, indemnification, privacy, and other provisions that by their nature should survive termination will remain in effect after termination.

## 10. Disclaimer of Warranties

> **TO THE MAXIMUM EXTENT PERMITTED BY LAW, THE SOFTWARE AND THE NEXUS CLOUD SERVICE ARE PROVIDED "AS IS" AND "AS AVAILABLE," WITHOUT WARRANTIES OF ANY KIND, EXPRESS, IMPLIED, OR STATUTORY.**

THE OPERATOR DISCLAIMS IMPLIED WARRANTIES INCLUDING MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, TITLE, AND NON-INFRINGEMENT, AND DOES NOT WARRANT THAT THE SOFTWARE OR THE NEXUS CLOUD SERVICE WILL BE UNINTERRUPTED, ERROR-FREE, COMPLETELY SECURE, ALWAYS AVAILABLE, COMPATIBLE WITH EVERY DEVICE, FREE FROM DEFECTS, OR PREVENT DATA LOSS.

THE OPERATOR DOES NOT GUARANTEE THE ACCURACY, COMPLETENESS, OR RELIABILITY OF RESPONSES GENERATED BY THE AI ASSISTANT, THE ON-DEVICE MODELS, OR THIRD-PARTY AI PROVIDERS, INCLUDING ANY "POSSIBLE CONFLICT" OR "RELATED NOTE" SUGGESTIONS.

AI-generated information may be inaccurate, incomplete, or outdated and is not professional, legal, medical, financial, or other regulated professional advice. You are responsible for evaluating it before relying on it.

> **YOU USE THE SOFTWARE AND THE NEXUS CLOUD SERVICE AT YOUR OWN RISK.**

Nothing in this Agreement excludes or limits any warranty or right that cannot lawfully be excluded or limited.

## 11. Limitation of Liability

To the maximum extent permitted by law, the Operator will not be liable for any indirect, incidental, special, consequential, exemplary, or punitive damages, or for loss of profits, revenue, business opportunities, goodwill, or data, arising from or related to the Software, Nexus Cloud Service, or this Agreement.

To the maximum extent permitted by law, the aggregate liability of the Operator for claims arising from or relating to the Software, Nexus Cloud Service, or this Agreement will not exceed the greater of:

- the total amount you paid to Nexus for the relevant service during the twelve months immediately preceding the event giving rise to the claim; or
- USD $100.

This limitation does not apply to liability that cannot legally be limited or excluded under applicable law.

## 12. Indemnification

To the extent permitted by law, you agree to indemnify and hold harmless the Operator from claims, liabilities, damages, losses, and reasonable expenses arising directly from:

- your unlawful use of the Software or Nexus Cloud Service;
- your material breach of this Agreement;
- your violation of applicable law; or
- your infringement of a third party's rights through content you intentionally transmit or use through the Software or Nexus Cloud Service.

This section does not apply to the extent a claim results from the Operator's own unlawful conduct or where indemnification is prohibited by law.

## 13. Governing Law and Disputes

Except to the extent mandatory law provides otherwise, this Agreement is governed by the laws of the Kingdom of Morocco, without regard to conflict-of-law principles.

Subject to any mandatory consumer protections or other mandatory legal rights applicable to you, disputes arising from or relating to this Agreement, the Software, or the Nexus Cloud Service shall be submitted to the competent courts of the Kingdom of Morocco.

Nothing in this section deprives you of mandatory rights or remedies that cannot legally be waived or restricted.

## 14. General Provisions

### (a) Entire Agreement

This Agreement, together with the Nexus Privacy Policy and any additional terms expressly incorporated by reference, forms the agreement between you and the Operator concerning the Software and the Nexus Cloud Service.

The Nexus Terms of Service separately govern the Nexus Website and any other services or features expressly covered by those Terms. If there is a conflict concerning the Software or the license granted under this Agreement, this Agreement controls. If there is a conflict concerning the processing of personal information, the Nexus Privacy Policy controls to the extent applicable. If there is a conflict concerning the Website, the Nexus Terms of Service control.

### (b) Severability

If any provision is found invalid or unenforceable, it will be enforced to the maximum extent permitted by law, and the remaining provisions will remain in effect.

### (c) No Waiver

Failure to enforce any provision is not a waiver of that provision or any other provision.

### (d) Assignment

You may not assign or transfer your rights or obligations without the Operator's prior written consent, except where such a restriction is prohibited by law.

The Operator may assign this Agreement in connection with a reorganization, sale, merger, acquisition, transfer of the Software or Nexus Cloud Service, or establishment of a successor legal entity.

### (e) Modifications

The Operator may update this Agreement from time to time. For material changes, the Operator may provide reasonable notice through the Software, Website, or another suitable method where required by law.

Continued use after an update takes effect constitutes acceptance to the extent permitted by law.

### (f) Export Compliance

You agree to use the Software and Nexus Cloud Service in compliance with applicable export-control, sanctions, and trade laws.

### (g) Eligibility

You must have the legal capacity to enter into this Agreement and must be at least 16 years old.

If you enter into this Agreement for an organization, you represent that you have authority to bind that organization.

### (h) No Partnership or Agency

Nothing in this Agreement creates a partnership, joint venture, employment, agency, or fiduciary relationship between you and the Operator.

## 15. Privacy

Your use of the Software and Nexus Cloud Service is also governed by the **Nexus Privacy Policy**.

The Privacy Policy distinguishes information stored locally on your device from account and usage information processed by the Nexus Cloud Service and information sent to Third-Party Providers on your behalf.

[Nexus Privacy Policy](/PRIVACY-POLICY.md)

## 16. Third-Party Licenses

Nexus includes third-party software, models, fonts, and other components distributed under separate licenses, which may grant rights independent of this Agreement.

Where required, notices are provided with the Software or in the Nexus repository. Nothing in this Agreement limits rights granted to you under applicable open-source licenses.

## 17. Contact

Questions regarding this Agreement may be directed to:

**Nawrass Andaloussi Dahman**  
Operator of Nexus  
Morocco

**Email:** [getnexusupport@gmail.com](mailto:getnexusupport@gmail.com)

---

**Copyright © 2026 Nawrass Andaloussi Dahman. All Rights Reserved.**

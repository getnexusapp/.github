# Nexus End User License Agreement

**Last Updated: September 2, 2026**

This End User License Agreement ("Agreement") is a legal agreement between you, either an individual or an entity you represent ("You" or "User"), and **Nawrass Andaloussi Dahman**, an individual developer based in Morocco and the creator and current operator of the Nexus software ("Nexus," "we," "us," or "our").

This Agreement governs your download, installation, access to, and use of the Nexus desktop application, including its software, features, updates, and accompanying documentation (collectively, the "Software"), as well as your use of the Nexus Cloud Service described in Section 5.

**Nexus is currently an independently developed software product operated by Nawrass Andaloussi Dahman. No corporation named "Nexus, Inc." currently operates the Software or is a party to this Agreement. If Nexus is later transferred to or operated by a separate legal entity, this Agreement may be updated accordingly.**

**BY DOWNLOADING, INSTALLING, ACCESSING, OR USING THE SOFTWARE, YOU ACKNOWLEDGE THAT YOU HAVE READ, UNDERSTOOD, AND AGREE TO BE BOUND BY THIS AGREEMENT. IF YOU DO NOT AGREE TO THIS AGREEMENT, DO NOT DOWNLOAD, INSTALL, ACCESS, OR USE THE SOFTWARE.**

---

## 1. Definitions

**"Software"** means the Nexus desktop application in object-code form, including its features, updates, and accompanying documentation. The Software does not include source code that is not expressly provided or licensed to you.

**"Your Content"** means notes, text, files, information, browser-related content, AI conversation history, and other content that you create, import, access, or store using the Software.

**"Nexus Cloud Service"** means the backend service operated by Nexus (currently hosted on Cloudflare Workers with an associated database) that powers the optional AI Assistant feature, including account creation and sign-in, forwarding of AI requests to a third-party AI provider, usage tracking and rate limiting, and password-reset email delivery.

**"Third-Party Provider"** means an external service provider used in connection with the Software, including the third-party AI provider used by the Nexus Cloud Service to generate AI Assistant responses.

**"Nexus"** means the Nexus software product and, where the context requires, Nawrass Andaloussi Dahman as the current developer and operator of the Software and the Nexus Cloud Service.

---

## 2. Grant of License

Subject to your compliance with this Agreement, Nawrass Andaloussi Dahman grants you a limited, non-exclusive, non-transferable, non-sublicensable, revocable license to download, install, and use the Software in object-code form for your personal or internal business purposes on devices that you own or are authorized to control.

This license does not transfer ownership of the Software or any intellectual property rights to you.

All rights not expressly granted under this Agreement are reserved by Nawrass Andaloussi Dahman.

---

## 3. Restrictions

You shall not, and shall not knowingly permit or assist any third party to:

(a) copy, modify, translate, or create derivative works based on the Software, except to the extent expressly permitted by applicable law;

(b) reverse engineer, decompile, disassemble, or otherwise attempt to derive or access the source code, underlying structure, algorithms, or proprietary components of the Software, except to the limited extent that such restriction is prohibited by applicable law;

(c) distribute, sell, rent, lease, sublicense, lend, publish, or otherwise transfer the Software or rights granted under this Agreement to a third party, except as expressly authorized by Nexus;

(d) remove, alter, or obscure copyright, trademark, licensing, or other proprietary notices contained in or accompanying the Software;

(e) use the Software to develop, train, or improve a competing product or service, to the extent permitted by applicable law;

(f) circumvent, disable, or interfere with security, licensing, authentication, or other technical protections incorporated into the Software or the Nexus Cloud Service;

(g) use the Software or the Nexus Cloud Service to violate any applicable law or regulation;

(h) attempt to exceed, circumvent, or abuse the usage limits or rate limits applied to your Nexus Cloud account; or

(i) intentionally interfere with the normal operation of the Software or the Nexus Cloud Service, or attempt to gain unauthorized access to functionality or accounts that are not made available to you.

Nothing in this section is intended to restrict rights that cannot legally be restricted under applicable law.

---

## 4. Ownership and Intellectual Property

The Software is licensed, not sold.

All rights, title, and interest in and to the proprietary portions of the Software, including its source code, object code, architecture, design, user interface, documentation, graphics, logos, and other proprietary elements, are owned by or licensed to Nawrass Andaloussi Dahman, except for third-party materials that are subject to their own licenses.

Nothing in this Agreement grants you ownership of the Software or any intellectual property rights in the Software except for the limited license expressly granted in Section 2.

The Nexus name, logo, and other branding are proprietary assets of Nexus and/or Nawrass Andaloussi Dahman to the extent protected by applicable law.

### Feedback

If you voluntarily provide suggestions, ideas, bug reports, feature requests, or other feedback regarding the Software ("Feedback"), you grant Nawrass Andaloussi Dahman a worldwide, royalty-free, perpetual, irrevocable, transferable, and sublicensable right to use, reproduce, modify, distribute, display, and otherwise exploit that Feedback for any lawful purpose without compensation or attribution to you.

---

## 5. Local-First Architecture, Your Content, and the Nexus Cloud Service

Nexus's core note-taking and browsing functionality is designed as a **local-first** experience. The optional AI Assistant, however, depends on the **Nexus Cloud Service**, which is not local-first — it is a server-side service operated by Nexus. This section explains both.

### (a) Local Storage (Notes and Workspace)

Your Content related to notes, folders, tags, links, version history, and trash is primarily stored locally on your device, including in a local SQLite database where applicable.

This local workspace remains on your device unless you explicitly choose to export, back up, copy, or otherwise transmit it, or unless you use the AI Assistant, which transmits relevant portions of your notes to the Nexus Cloud Service as described below.

### (b) Local Search

Nexus's semantic search functionality, including generation of local embeddings, is designed to run locally on your device and does not require your notes to be uploaded to a Nexus-operated server to be indexed or searched.

### (c) Local Version History and Trash

Nexus maintains version history, deleted content, and related workspace information locally on your device.

### (d) The AI Assistant and the Nexus Cloud Service

The AI Assistant is powered by the Nexus Cloud Service, not by a "bring your own key" model. To use the AI Assistant:

- You must create a **Nexus Cloud account** using an email address and password, or sign in to an existing one.
- Upon signup or sign-in, Nexus issues you a Nexus Cloud API key, which the Software uses to authenticate your requests to the Nexus Cloud Service.
- When you submit a question or message through the AI Assistant, your request — including relevant portions of Your Content (such as retrieved note excerpts) and, where you have enabled it, text from your currently open browser tabs — is transmitted from your device to the Nexus Cloud Service.
- The Nexus Cloud Service forwards your request to a third-party AI provider using API credentials that belong to Nexus, and returns the generated response to your device. You are not required to, and currently cannot, supply your own third-party AI provider API key for this feature.
- The Nexus Cloud Service is subject to rolling usage limits; Nexus may decline or delay requests that exceed those limits.

### (e) Nexus Cloud Account and Credential Storage

Your Nexus Cloud API key is stored locally on your device using operating-system or application-level credential-storage mechanisms where available.

Your underlying Nexus Cloud account record — including your email address, a hashed form of your password, a hashed form of your API key, and usage information such as token counts and request timestamps — is stored and processed by the Nexus Cloud Service (a server-side database operated by or on behalf of Nexus), not solely on your device.

You are responsible for protecting access to your device and your Nexus Cloud credentials, and for any activity that occurs through your Nexus Cloud account.

### (f) Third-Party AI Provider

The Nexus Cloud Service relies on a third-party AI provider to generate AI Assistant responses. Nexus selects and pays for this provider; you do not have a direct account or contractual relationship with that provider through this feature. Nexus does not control how that provider internally processes requests it receives from the Nexus Cloud Service, and that provider's own terms may apply to Nexus's use of it.

### (g) Local AI Chat History

The Software saves AI conversation history locally on your device as part of Your Content. The Nexus Cloud Service also necessarily processes the content of each request and response at the time it is generated, and may retain associated usage metadata (such as token counts and timestamps) as described in Section 5(e); see the Nexus Privacy Policy for further detail.

### (h) Built-In Browser

Nexus includes a browser that allows you to access third-party websites and online services. When you access a third-party website through the Nexus browser, that website may communicate directly with its own servers according to its own privacy policy and terms. Nexus does not control the privacy practices of third-party websites.

### (i) Data Transmission Summary

Local workspace operations (notes storage, local search, local version history) do not require transmission to a Nexus-operated server. Using the AI Assistant does require transmission to the Nexus Cloud Service, and using the built-in browser or a linked website requires communication with that website's own servers. You are responsible for deciding what information you submit through the AI Assistant or to third-party websites.

---

## 6. Nexus Cloud Accounts

Unlike your local notes workspace, the AI Assistant **does require a Nexus Cloud account**, created and authenticated through the Nexus Cloud Service as described in Section 5(d)–(e). You may use the core note-taking and browsing functionality of the Software without creating a Nexus Cloud account, but you cannot use the AI Assistant without one.

Nexus does not currently provide automatic cloud synchronization of your local notes workspace; a Nexus Cloud account governs access to the AI Assistant only, and does not back up or synchronize your notes.

If Nexus introduces additional online services, synchronization, analytics, or other network-based features in the future, those features may be governed by additional or updated terms and privacy disclosures.

---

## 7. Backups and Data Loss

Because your notes workspace is stored locally, you are responsible for maintaining backups of Your Content.

Nexus may provide tools for exporting, copying, or backing up your workspace.

You are solely responsible for deciding whether and where to create backups.

To the maximum extent permitted by applicable law, Nexus is not responsible for loss, corruption, deletion, or unavailability of Your Content resulting from:

* device failure;
* storage failure;
* operating-system failure;
* accidental deletion;
* malware or security incidents;
* user actions;
* third-party software;
* hardware failure;
* improper backups;
* unavailability or discontinuation of the Nexus Cloud Service; or
* other events beyond the reasonable control of Nexus.

**You should maintain independent backups of important data.**

---

## 8. Updates and Changes

Nexus may provide updates, upgrades, bug fixes, patches, security fixes, or new features from time to time, and may modify or discontinue the Nexus Cloud Service.

Nexus is not obligated to provide updates or continue supporting any particular version, feature, or the Nexus Cloud Service, except where required by applicable law.

Unless an update is accompanied by separate terms, this Agreement will continue to apply to the updated Software.

---

## 9. Term and Termination

This Agreement begins when you first download, install, access, or use the Software and continues until terminated.

Nexus may terminate or suspend your license, your Nexus Cloud account, or your access to the Nexus Cloud Service if you materially breach this Agreement or use the Software or Nexus Cloud Service unlawfully, subject to applicable law.

You may terminate this Agreement at any time by uninstalling the Software and ceasing to use it. You may also stop using the AI Assistant at any time without affecting your local notes workspace.

Upon termination, you must cease using the Software and delete copies of the Software in your possession or control, except where retention is required by applicable law.

Termination of your license does not automatically delete Your Content from your device.

Sections concerning intellectual property, Feedback, Third-Party Providers, disclaimers, limitations of liability, indemnification, and provisions that by their nature should survive termination will survive termination.

---

## 10. Disclaimer of Warranties

**TO THE MAXIMUM EXTENT PERMITTED BY APPLICABLE LAW, THE SOFTWARE AND THE NEXUS CLOUD SERVICE ARE PROVIDED "AS IS" AND "AS AVAILABLE," WITHOUT WARRANTIES OF ANY KIND, WHETHER EXPRESS, IMPLIED, OR STATUTORY.**

TO THE MAXIMUM EXTENT PERMITTED BY LAW, NEXUS DISCLAIMS IMPLIED WARRANTIES INCLUDING MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, TITLE, AND NON-INFRINGEMENT.

NEXUS DOES NOT WARRANT THAT THE SOFTWARE OR THE NEXUS CLOUD SERVICE WILL:

* be uninterrupted;
* be error-free;
* be completely secure;
* be available at all times;
* be compatible with every device or operating system;
* be free from defects; or
* prevent data loss.

NEXUS DOES NOT GUARANTEE THE ACCURACY, COMPLETENESS, OR RELIABILITY OF INFORMATION OR RESPONSES GENERATED BY THE AI ASSISTANT OR THE UNDERLYING THIRD-PARTY AI PROVIDER.

AI-generated information may be inaccurate, incomplete, outdated, or inappropriate for a particular purpose.

You are responsible for evaluating AI-generated information before relying upon it.

**YOU USE THE SOFTWARE AND THE NEXUS CLOUD SERVICE AT YOUR OWN RISK.**

Nothing in this Agreement excludes or limits any warranty or right that cannot lawfully be excluded or limited under applicable law.

---

## 11. Limitation of Liability

**TO THE MAXIMUM EXTENT PERMITTED BY APPLICABLE LAW, NEXUS AND NAWRASS ANDALOUSSI DAHMAN SHALL NOT BE LIABLE FOR INDIRECT, INCIDENTAL, SPECIAL, CONSEQUENTIAL, EXEMPLARY, OR PUNITIVE DAMAGES, OR FOR LOSS OF DATA, PROFITS, REVENUE, BUSINESS OPPORTUNITY, OR GOODWILL, ARISING OUT OF OR RELATED TO YOUR USE OF OR INABILITY TO USE THE SOFTWARE OR THE NEXUS CLOUD SERVICE.**

TO THE MAXIMUM EXTENT PERMITTED BY APPLICABLE LAW, THE TOTAL AGGREGATE LIABILITY OF NEXUS AND NAWRASS ANDALOUSSI DAHMAN ARISING OUT OF OR RELATING TO THE SOFTWARE, THE NEXUS CLOUD SERVICE, OR THIS AGREEMENT SHALL NOT EXCEED THE GREATER OF:

(a) the amount you actually paid to Nexus for the Software or the Nexus Cloud Service during the twelve (12) months preceding the event giving rise to the claim; or

(b) USD $100.

THE LIMITATIONS ABOVE APPLY TO THE MAXIMUM EXTENT PERMITTED BY LAW.

SOME JURISDICTIONS DO NOT PERMIT CERTAIN LIMITATIONS OF LIABILITY, WARRANTIES, OR DAMAGES. WHERE SUCH LIMITATIONS ARE NOT PERMITTED, THEY SHALL APPLY ONLY TO THE MAXIMUM EXTENT PERMITTED BY APPLICABLE LAW.

---

## 12. Indemnification

To the extent permitted by applicable law, you agree to indemnify and hold harmless Nawrass Andaloussi Dahman from claims, liabilities, damages, losses, and reasonable expenses arising directly from:

(a) your unlawful use of the Software or the Nexus Cloud Service;

(b) your material breach of this Agreement;

(c) your violation of applicable law; or

(d) your infringement or violation of the rights of a third party through content or information that you intentionally transmit or use through the Software or the Nexus Cloud Service.

This section does not require you to indemnify Nexus or Nawrass Andaloussi Dahman to the extent a claim results from their own unlawful conduct or where such indemnification is prohibited by applicable law.

---

## 13. Governing Law and Disputes

Nexus is currently operated by an individual developer based in Morocco and may be used by individuals and organizations in different jurisdictions.

This Agreement is subject to applicable law and any mandatory consumer protections that apply to you based on your jurisdiction.

Nothing in this Agreement is intended to deprive you of rights or protections that cannot legally be waived under the laws applicable to you.

If Nexus is later transferred to a separate legal entity, this Agreement may be updated to identify the applicable contracting entity and appropriate governing-law and dispute-resolution provisions.

---

## 14. General Provisions

### (a) Entire Agreement

This Agreement, together with the Nexus Privacy Policy and any additional terms expressly incorporated into it, constitutes the agreement between you and Nexus concerning the Software and the Nexus Cloud Service and supersedes prior agreements concerning the same subject matter.

### (b) Severability

If any provision of this Agreement is determined to be invalid or unenforceable, that provision will be enforced to the maximum extent permitted by applicable law, and the remaining provisions will remain in effect.

### (c) No Waiver

Failure to enforce any provision of this Agreement does not constitute a waiver of that provision or any other provision.

### (d) Assignment

You may not assign or transfer your rights or obligations under this Agreement without Nexus's prior written consent, except where such restriction is prohibited by applicable law.

Nexus may assign or transfer this Agreement in connection with a reorganization, sale, merger, acquisition, transfer of the Software or the Nexus Cloud Service, or establishment of a successor legal entity.

### (e) Modifications

Nexus may update this Agreement from time to time.

If material changes are made, Nexus may provide reasonable notice through the Software, website, or another appropriate method where required by applicable law.

Your continued use of the Software after an updated Agreement becomes effective constitutes acceptance of the updated Agreement to the extent permitted by applicable law.

### (f) Export Compliance

You agree to use the Software and the Nexus Cloud Service in compliance with applicable export-control, sanctions, and other trade laws that apply to your use of them.

### (g) Eligibility

You must have the legal capacity to enter into this Agreement under the laws applicable to you.

If you are entering into this Agreement on behalf of an organization, you represent that you have authority to bind that organization.

### (h) No Partnership or Agency

Nothing in this Agreement creates a partnership, joint venture, employment relationship, agency relationship, or other fiduciary relationship between you and Nexus.

---

## 15. Privacy

Your use of the Software and the Nexus Cloud Service is also governed by the **Nexus Privacy Policy**.

The Privacy Policy describes how Nexus handles information, distinguishing information stored locally on your device from account and usage information processed by the Nexus Cloud Service, and from information transmitted to the third-party AI provider on your behalf.

**[Nexus Privacy Policy](./PRIVACY_POLICY.md)**

---

## 16. Third-Party Licenses

Nexus may include third-party software and components that are distributed under separate licenses.

Those licenses may grant rights that are independent of this Agreement.

Where required, applicable third-party license notices are provided separately with the Software or in the Nexus repository.

Nothing in this Agreement is intended to limit rights granted to you under applicable third-party open-source licenses.

---

## 17. Contact

Questions regarding this Agreement may be directed to:

**Nawrass Andaloussi Dahman**  
Developer and Creator of Nexus  
Morocco

**Email:** [getnexusupport@gmail.com](mailto:getnexusupport@gmail.com)

---

**Copyright © 2026 Nawrass Andaloussi Dahman. All Rights Reserved.**

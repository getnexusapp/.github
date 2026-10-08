# Nexus Terms of Service

**Last Updated: October 8, 2026**

These Terms of Service ("Terms") are a legal agreement between you, either an individual or an entity you represent ("You" or "User"), and **Nawrasse Andaloussi Dahman**, an individual developer based in Morocco and the creator and current operator of Nexus ("Nexus," "we," "us," or "our").

These Terms govern your use of the Nexus website and the Nexus Cloud Service. Your use of the Nexus desktop application is additionally governed by the **Nexus End User License Agreement ("EULA")** and the Nexus Software License.

**Nexus is currently an independently developed product operated by Nawrasse Andaloussi Dahman. No corporation named "Nexus, Inc." operates the Software or is a party to these Terms. If Nexus is later transferred to or operated by a separate legal entity, these Terms may be updated to identify that entity.**

**BY ACCESSING OR USING THE NEXUS WEBSITE OR NEXUS CLOUD SERVICE, YOU ACKNOWLEDGE THAT YOU HAVE READ, UNDERSTOOD, AND AGREE TO BE BOUND BY THESE TERMS. IF YOU DO NOT AGREE, DO NOT ACCESS OR USE THE WEBSITE OR NEXUS CLOUD SERVICE.**

---

## 1. Scope and Document Hierarchy

These Terms apply primarily to the Nexus website and, together with the EULA, to the Nexus Cloud Service. The EULA governs your license to and use of the Nexus desktop application and related installed Software, and the Nexus Software License supplements the EULA with respect to intellectual-property rights in the proprietary Software.

If these Terms conflict with the EULA, the EULA controls with respect to the desktop Software, your license to use it, and your use of the Nexus Cloud Service through the Software. These Terms control with respect to the Nexus website and any other use of the Nexus Cloud Service.

The Nexus Privacy Policy governs the processing of personal information described in that policy. The Privacy Policy does not grant a license to the Software or create rights concerning intellectual property.

Nothing in these Terms, the EULA, or the Privacy Policy limits or excludes any right or protection that cannot lawfully be limited or excluded.

## 2. Definitions

**"Nexus Website"** means the websites and web pages operated by Nexus, including pages through which the Software or related information may be made available.

**"Nexus Cloud Service"** means the backend service operated by Nexus that provides optional AI Assistant functionality, account creation and sign-in, forwarding of AI requests to third-party providers, web search for the Assistant, usage tracking, and rate limiting.

**"Software"** means the Nexus desktop application, as defined more fully in the EULA.

**"Your Content"** means notes, text, images, files, bookmarks, AI conversation history, browser-related content, and other content that you create, import, access, or store through Nexus.

**"Third-Party Provider"** means an external service used with Nexus, including the AI model provider (currently Google through its Gemini models), web search provider (currently Jina AI), sign-in providers (Google and GitHub), hosting provider (currently Cloudflare), and favicon provider (currently DuckDuckGo), and, for the Software, search, model-distribution, and update-distribution providers such as Brave Search, Hugging Face, jsDelivr, and GitHub.

## 3. Eligibility

You must have the legal capacity to enter into these Terms and must be at least 16 years old.

If you use Nexus on behalf of an organization, you represent that you have authority to bind that organization to these Terms.

## 4. Nexus Website and Cloud Service

The Nexus Cloud Service is an optional online service used primarily for the AI Assistant and associated account functionality. Core local-first features of the desktop Software do not require a Nexus Cloud account.

The Nexus Cloud Service is currently hosted using Cloudflare infrastructure and may use associated databases and other infrastructure needed to operate the service.

When you use the AI Assistant, the Nexus Cloud Service receives the information necessary to process your request and forwards applicable request content to a third-party AI provider, currently Google through its Gemini models. As explained in Section 7, Google may use that content to train its models.

The AI Assistant may use web search. When it does, the search query may be sent to Jina AI, and the Nexus Cloud Service may retrieve relevant result content.

Nexus applies usage and rate limits to the Nexus Cloud Service. Current limits may include a rolling token allowance and per-minute request limits. Nexus may change, suspend, or decline requests that exceed applicable limits.

## 5. Your Content and Local-First Architecture

You retain ownership of Your Content. These Terms do not transfer ownership of Your Content to Nexus.

Nexus is designed as a local-first application. Notes, folders, tags, links, local search indexes, version history, embeddings, conversation history, browser settings, bookmarks, and other local workspace data are generally stored on your device rather than synchronized to a Nexus-operated cloud database.

The AI Assistant is different. When you use it, information necessary to answer your request may be transmitted to the Nexus Cloud Service and third-party providers as described in these Terms and the Nexus Privacy Policy.

Depending on your request and enabled features, an AI Assistant request may contain your new message, up to 20 prior conversation messages, relevant excerpts from a note, up to a limited portion of a note's text when relevant-excerpt retrieval is unavailable, the full contents of a note when you specifically identify it by title, the current date and time, and text retrieved from pages open in the Nexus Browser when that text is included under the applicable browser settings.

Notes that you mark "AI: Off" are not intentionally included in AI Assistant requests. However, "AI: Off" does not prevent transmission of anything you personally type, paste, or otherwise submit to the AI Assistant.

You are responsible for determining whether information you submit to the AI Assistant is appropriate for transmission to the Nexus Cloud Service and its third-party providers.

## 6. Accounts and Credentials

Some Nexus Cloud features require an account. Accounts are created and accessed only by signing in with Google or GitHub. If you sign in and no Nexus Cloud account exists for you, Nexus creates one automatically; if you already have an account, you are signed in to it. Nexus does not receive or store your Google or GitHub password.

Account information may include your email address, the account identifier provided by your sign-in provider, a hash of your current API key, usage information, and rate-limiting information.

Your Nexus Cloud API key is stored on your device using your operating system's credential storage, such as Windows Credential Manager, the macOS Keychain, or equivalent secure storage on other supported platforms.

Each successful sign-in may issue a new API key and invalidate the previous key. Nexus may limit the number of key regenerations available within a given period.

You are responsible for protecting your device, your Google or GitHub account, your credentials, and your API key and for activity occurring through your account, except to the extent caused by Nexus's own failure to maintain required security measures.

**Deleting your account.** You may permanently delete your Nexus Cloud account through the available account settings. Account deletion removes the account record and usage history from the Nexus Cloud Service and immediately invalidates the account's API key.

Rate-limiting counters, operational logs, and hosting-provider backups may remain for a limited period where necessary for security, accounting, abuse prevention, disaster recovery, dispute resolution, record-keeping, or legal obligations. Deleting your Nexus Cloud account does not delete Your Content stored locally on your device.

## 7. Third-Party Providers

Nexus uses independent third-party providers to operate portions of the Nexus Cloud Service and related functionality.

- **Google / Gemini:** provides the third-party AI models used by the AI Assistant.
- **Google and GitHub (sign-in):** authentication providers used to create and access Nexus Cloud accounts.
- **Jina AI:** may provide web search functionality for AI Assistant requests.
- **Cloudflare:** provides hosting and infrastructure for the Nexus Cloud Service.
- **Brave Search:** receives non-URL queries typed into the Nexus Browser address bar.
- **DuckDuckGo:** may provide favicon services used by the Nexus Browser.
- **Hugging Face and jsDelivr:** may distribute on-device model files and related components.
- **GitHub:** may provide update distribution and website or repository hosting.

These providers operate independently from Nexus and may process information under their own terms and policies. Nexus does not control the internal processing practices of third-party providers.

Nexus does not provide your own API credentials to third-party AI providers through the Nexus Cloud Service. Nexus uses credentials associated with its own service.

### Google Model Training and Your Consent

The AI Assistant currently uses Google's Gemini models. Content included in AI Assistant requests forwarded through the Nexus Cloud Service may be used by Google to train and improve its models, under Google's own terms and policies.

**BY CREATING A NEXUS CLOUD ACCOUNT OR USING THE AI ASSISTANT, YOU ACKNOWLEDGE AND AGREE THAT GOOGLE MAY USE CONTENT SENT THROUGH NEXUS CLOUD AI REQUESTS TO TRAIN AND IMPROVE ITS MODELS. IF YOU DO NOT AGREE, DO NOT CREATE A NEXUS CLOUD ACCOUNT OR USE THE AI ASSISTANT.**

Nexus does not itself use Your Content to train AI models and does not control how Google uses information it receives. Nexus cannot recall content that has already been sent to Google. See Section 5(c) of the EULA and Section 4 of the Nexus Privacy Policy for details, including what stays on your device.

## 8. Built-In Browser

The Nexus Browser connects directly from your device to the websites that you visit. Those websites operate under their own terms and privacy policies.

Searches entered as non-URL queries in the browser address bar are sent to Brave Search. Site icons may be requested from DuckDuckGo. Websites may store cookies and other site data on your device.

Nexus may retrieve and read the text of pages open in Nexus Browser tabs on your device even when the "Aware of tabs" setting is turned off. This allows local browser features, such as conflict detection, to operate.

Turning off "Aware of tabs" prevents page text from being automatically included in AI Assistant requests and transmitted to the Nexus Cloud Service through that feature. It does not necessarily prevent the Software from retrieving or locally analyzing page text for other local browser functionality.

If you do not want page text included in an AI Assistant request, you should ensure that the relevant setting is disabled before submitting that request.

## 9. Acceptable Use

You may not use Nexus or the Nexus Cloud Service to violate applicable law or the rights of others.

You may not:

- use the Nexus Cloud Service to facilitate unlawful activity;
- attempt to gain unauthorized access to Nexus accounts, systems, or infrastructure;
- circumvent or interfere with usage limits, rate limits, or security mechanisms;
- use automated scripts or other mechanisms to abuse the Nexus Cloud Service;
- use the Nexus Cloud Service to transmit malware or malicious code;
- intentionally interfere with the availability or operation of the service;
- use another person's account or credentials without authorization; or
- use the service in a manner that infringes another person's intellectual-property, privacy, or other rights.

## 10. Intellectual Property

Nexus, including its software, interface, branding, logos, design, documentation, and other original materials, is owned by or licensed to Nawrasse Andaloussi Dahman and is protected by applicable intellectual property laws.

Except for the rights expressly granted under the EULA, no ownership or other intellectual-property rights in Nexus are transferred to you.

Your Content remains yours. You grant Nexus only the limited rights necessary to operate the services you request, including processing information through the Nexus Cloud Service and applicable third-party providers.

## 11. Feedback

If you voluntarily provide suggestions, ideas, or feedback concerning Nexus, you grant Nexus permission to use that feedback to improve the Software and services without compensation to you, provided that such use does not disclose Your Content or personal information contrary to the Privacy Policy.

## 12. Paid Features and Availability

Core local-first functionality of the Nexus desktop application is currently provided without a subscription fee.

Nexus may introduce optional paid features or services in the future. Any paid feature will be separately identified, and applicable pricing and terms will be presented before you are charged.

Nexus does not guarantee that any particular feature or service will remain available indefinitely. Features may be modified, suspended, or discontinued where permitted by law.

## 13. Backups, Exports, and Data Loss

Because Nexus is local-first, you are responsible for maintaining backups of important local content.

Nexus may provide export and backup functionality, but you are responsible for verifying that exported or backed-up files are complete and usable.

Nexus does not guarantee that local data can be recovered after device failure, accidental deletion, corruption, operating-system failure, or other events outside Nexus's control.

Clearing local application data or uninstalling the Software may remove local content depending on the operating system and storage method. You should create an appropriate backup before taking actions that may delete local data.

## 14. Disclaimers

**TO THE MAXIMUM EXTENT PERMITTED BY LAW, THE NEXUS WEBSITE, SOFTWARE, AND NEXUS CLOUD SERVICE ARE PROVIDED "AS IS" AND "AS AVAILABLE," WITHOUT WARRANTIES OF ANY KIND, EXPRESS, IMPLIED, OR STATUTORY.**

Nexus disclaims implied warranties including merchantability, fitness for a particular purpose, title, and non-infringement to the extent permitted by law.

Nexus does not warrant that the website, Software, or Cloud Service will be uninterrupted, error-free, completely secure, always available, compatible with every device, or free from defects or data loss.

AI-generated information may be inaccurate, incomplete, outdated, or inappropriate for your circumstances. AI output, including information generated through third-party models, is not professional, legal, medical, financial, or other regulated professional advice.

You are responsible for evaluating AI-generated information before relying on it.

Nothing in these Terms excludes or limits any warranty, remedy, or right that cannot legally be excluded or limited.

## 15. Limitation of Liability

To the maximum extent permitted by law, Nawrasse Andaloussi Dahman will not be liable for any indirect, incidental, special, consequential, exemplary, or punitive damages, or for loss of profits, revenue, business opportunities, goodwill, or data, arising from or related to the Nexus Website, Software, Nexus Cloud Service, or these Terms.

To the maximum extent permitted by law, the aggregate liability of Nawrasse Andaloussi Dahman for claims arising from or relating to the Nexus Website, Software, Nexus Cloud Service, or these Terms will not exceed the greater of:

- the total amount you paid to Nexus for the relevant service during the twelve months immediately preceding the event giving rise to the claim; or
- USD $100.

This limit applies in the aggregate across these Terms and the EULA and is not cumulative across the two.

This limitation does not apply to liability that cannot legally be limited or excluded under applicable law.

## 16. Indemnification

To the extent permitted by law, you agree to indemnify and hold harmless Nawrasse Andaloussi Dahman from claims, liabilities, damages, losses, and reasonable expenses arising directly from:

- your unlawful use of the Nexus Website, Software, or Nexus Cloud Service;
- your material breach of these Terms;
- your violation of applicable law; or
- your infringement of a third party's rights through content you intentionally transmit or use through Nexus.

This section does not apply to the extent a claim results from Nexus's own unlawful conduct, fraud, or intentional misconduct, or where indemnification is prohibited by law.

## 17. Suspension and Termination

Nexus may suspend or terminate your access to the Nexus Cloud Service if you materially breach these Terms, use the service unlawfully, abuse usage limits, compromise service security, or otherwise create a material risk to Nexus or other users, subject to applicable law.

Section 11 of the EULA, including the notice and opportunity to remedy it provides where reasonably practicable, also applies to suspension or termination in connection with the Software.

You may stop using the Nexus Website or Nexus Cloud Service at any time. You may also delete your Nexus Cloud account without deleting local content stored on your device.

Termination or suspension of the Nexus Cloud Service does not itself delete Your Content stored locally on your device.

Sections concerning intellectual property, feedback, third-party providers, disclaimers, limitations of liability, indemnification, privacy, and other provisions that by their nature should survive will survive termination.

## 18. Governing Law and Disputes

Except to the extent mandatory law provides otherwise, these Terms are governed by the laws of the Kingdom of Morocco, without regard to conflict-of-law principles.

Subject to any mandatory consumer protections or other mandatory legal rights applicable to you, disputes arising from or relating to these Terms, the Nexus Website, or the Nexus Cloud Service shall be submitted to the competent courts of the Kingdom of Morocco.

Nothing in this section deprives you of mandatory rights or remedies that cannot legally be waived or restricted.

## 19. General Provisions

### (a) Entire Agreement

These Terms, the EULA, the Nexus Software License, and the Nexus Privacy Policy, together with any additional terms expressly incorporated by reference, form the agreement between you and Nexus concerning the subjects they cover.

The documents are intended to operate together. The EULA controls matters specifically concerning the desktop Software, its license, and use of the Nexus Cloud Service through the Software; the Nexus Software License supplements the EULA concerning intellectual-property rights in the proprietary Software; these Terms control matters specifically concerning the Nexus Website and any other use of the Nexus Cloud Service; and the Privacy Policy controls matters concerning the processing of personal information.

### (b) Severability

If any provision is found invalid or unenforceable, it will be enforced to the maximum extent permitted by law, and the remaining provisions will remain in effect.

### (c) No Waiver

Failure to enforce any provision is not a waiver of that provision or any other provision.

### (d) Assignment

You may not assign or transfer your rights or obligations without Nexus's prior written consent, except where such a restriction is prohibited by law.

Nexus may assign these Terms in connection with a reorganization, sale, merger, acquisition, transfer of the Software or Nexus Cloud Service, or establishment of a successor legal entity.

### (e) Modifications

Nexus may update these Terms from time to time. For material changes, Nexus may provide reasonable notice through the Website, Software, or another suitable method where required by law.

Continued use after an update takes effect constitutes acceptance to the extent permitted by law.

### (f) Export Compliance

You agree to use the Nexus Website, Software, and Nexus Cloud Service in compliance with applicable export-control, sanctions, and trade laws.

### (g) No Partnership or Agency

Nothing in these Terms creates a partnership, joint venture, employment, agency, or fiduciary relationship between you and Nexus.

## 20. Privacy

Your use of the Nexus Website, Software, and Nexus Cloud Service is also subject to the Nexus Privacy Policy.

The Privacy Policy explains what information remains on your device, what information is processed by the Nexus Cloud Service, what information may be sent to third-party providers, and how account information is handled.

[Nexus Privacy Policy](https://nexusworkspace.net/privacy-policy)

## 21. Third-Party Licenses

Nexus includes third-party software, models, fonts, and other components distributed under separate licenses, which may grant rights independent of these Terms.

Where required, notices are provided with the Software, within the application, or through associated documentation or repositories. Nothing in these Terms limits rights granted to you under applicable open-source or third-party licenses.

## 22. Contact

Questions regarding these Terms may be directed to:

**Nawrasse Andaloussi Dahman**  
Operator of Nexus  
Morocco

**Email:** [support@nexusworkspace.net](mailto:support@nexusworkspace.net)

---

**Copyright © 2026 Nawrasse Andaloussi Dahman. All Rights Reserved.**

# AdImmunity — Privacy Policy

**Last updated: 30 July 2026**

---

## 1. Who We Are / Contact

AdImmunity is a Chrome browser extension that blocks ads, trackers and pop-ups, removes unwanted page weight, and warns you before known phishing or malware sites load. It is developed and maintained by an independent maker based in the United States.

If you have any questions about this Privacy Policy, please contact us at:

**Email:** omiteyt@gmail.com

We will respond to all privacy-related enquiries within a reasonable time, and no later than 30 days for requests under applicable data protection law.

---

## 2. Summary

AdImmunity is built with a privacy-first design.

**Everything the extension does happens locally on your device.**

The extension has no user accounts, does not require you to sign in, and does not send your browsing activity, personal information, or any usage data to us or to any third party.

We operate no servers that receive your data. There is no analytics and no telemetry of any kind. There is nothing to sign up for; every feature works immediately and anonymously.

---

## 3. What Stays on Your Device

AdImmunity relies exclusively on local browser storage. The following is stored in your browser and **never transmitted to us or anyone else**:

- **Blocking statistics** — counts of ads, trackers, pop-ups and scripts blocked, including the on-device "all-time" totals. These are counts only. No record of *which* site a block happened on is ever kept.
- **Extension settings** — your master on/off toggle, the per-feature switches, theme and other preferences. Settings may sync across your own signed-in Chrome profiles via Chrome's built-in `chrome.storage.sync`; this is handled entirely by Google Chrome and is never sent to us.
- **Element Zapper hides** — any elements you have chosen to hide on a page using the visual Zapper tool.
- **A cached copy of the public phishing blocklist** described in Section 4.
- **Session-only choices you make.** If you click "Proceed anyway" on a phishing warning, that decision is remembered so the warning does not reappear for that site while you keep browsing. If you click to load a deferred embed, a temporary browser rule permits that one embed. Both are held in session storage and are erased when you close Chrome; the embed permission is also removed as soon as you navigate away from the page or close the tab.

This data lives entirely on your device (or, for settings, within your own Google Chrome account). We have no access to it and no ability to retrieve it.

The blocking mechanism matches network requests against filter lists using Chrome's built-in `declarativeNetRequest` API, plus content scripts that hide ad elements. This happens entirely within your browser.

**We do not intercept, log, or store the URLs you visit, the requests you make, or any other browsing data.**

The optional **Anonymous** tool simply reopens the current page in a standard Chrome Incognito window. It uses Chrome's built-in incognito mode (which you enable for the extension once in your browser's settings) and transmits nothing to us. Note that Incognito mode is a local browser feature; it does not make you anonymous to the websites you visit, your network, or your internet provider.

---

## 4. The One Network Request AdImmunity Makes

To warn you before you load a known phishing or malware site, AdImmunity downloads a **public blocklist of malicious domains** once per day from URLhaus (`urlhaus.abuse.ch`), a free threat-intelligence feed operated by abuse.ch.

This is a one-way download of a public file. It works exactly like your browser downloading any public web page:

- **We do not send URLhaus anything about you** — no URL you visited, no identifier, no browsing data. The extension simply requests the public list.
- The blocklist is stored on your device and checked **locally** against sites you navigate to. **The check never leaves your browser.**

You can turn phishing protection off, or turn the whole extension off, with the master toggle — after which no network requests are made at all.

---

## 5. How AdImmunity Changes the Pages You Visit

Blocking ads means altering the page you are looking at. So that there is no surprise about what that involves, here is everything AdImmunity does to a page. All of it happens locally in your browser, and none of it is reported to us.

- **Hides and removes ad elements** — ad containers, sponsored placements, and the empty boxes left behind when an ad request is blocked are hidden with CSS or removed from the page.
- **Blocks network requests** to advertising and tracking hosts using Chrome's `declarativeNetRequest` API.
- **Removes tracking parameters from links** — campaign tags and ad click identifiers (`utm_*`, `gclid`, `fbclid`, `msclkid`, etc.) are stripped from links and the address bar. Parameters required for site functionality (unsubscribe links, affiliate attribution, etc.) are deliberately **not** removed.
- **Dismisses cookie-consent banners** *(optional, enabled by default)*. AdImmunity clicks **Reject**, **Decline**, or **Close** buttons where available. It **never** clicks **Accept** or **Agree**, and it never grants consent on your behalf.
- **Skips video advertisements** by clicking a "Skip Ad" button or seeking past an ad break.
- **Blocks pop-up windows** opened by known advertising and pop-under networks.
- **Reports a neutral answer to ad-block detection scripts** without affecting real page content.

### Turbo (Optional)

Turbo is a performance feature that blocks page extras beyond advertising.

**Turbo is disabled by default.**

The first time you enable it, AdImmunity automatically enables:

- Defer embeds
- Block chat widgets
- Block A/B testing
- Ask for lighter pages

**Block web fonts is never enabled automatically** because it noticeably changes how websites look.

Available Turbo features:

- **Defer embeds** — delays loading YouTube, Vimeo, Spotify, Instagram, Facebook, X, TikTok, Reddit, Disqus, OpenWeb, and similar embeds until requested.
- **Block chat widgets** — blocks Intercom, Drift, Zendesk, Tawk, and similar live chat widgets.
- **Block A/B testing** — blocks experiment and tag-manager scripts.
- **Ask for lighter pages** — sends the standard `Save-Data: on` request header.
- **Block web fonts** — prevents website font downloads, causing pages to use browser default fonts.

Turbo never blocks anything required for payments, sign-ins, or CAPTCHA verification.

Turning the master toggle off disables Turbo as well.

---

## 6. The Permissions AdImmunity Asks For

Chrome displays these permissions during installation:

- **Access to all websites** — required so filtering and content scripts can run everywhere. Never used to collect page content.
- **declarativeNetRequest** — Chrome's built-in filtering engine.
- **storage** — stores local settings, statistics, and cached blocklists.
- **tabs** — updates open tabs and resets tab counters.
- **alarms** — schedules daily statistic resets and blocklist updates.
- **webNavigation** — checks destination hostnames against the local phishing blocklist.
- **scripting** — registers and unregisters content scripts when enabled or disabled.

AdImmunity contains **no remote code**. Everything is packaged inside the extension reviewed by the Chrome Web Store.

---

## 7. What We Never Collect

AdImmunity **never** collects:

- Browsing history
- URLs of pages you visit
- Web page contents
- Search queries
- Names, email addresses, phone numbers, or account information
- Payment or financial information
- Location data
- Persistent identifiers tied to you

We have no servers, analytics, or telemetry.

---

## 8. No Accounts, No Third-Party Processors

AdImmunity has no login or sign-up.

We do not use:

- Analytics services
- Advertising services
- Error reporting services
- Databases containing user information

The only external request is the public URLhaus blocklist download described in Section 4.

We do not sell or share personal information because we do not collect any.

---

## 9. Your Rights (GDPR / UK GDPR / CCPA-CPRA)

Because AdImmunity stores no personal data on our servers, there is no personal information for us to access, delete, correct, or export.

- Local settings, statistics, and Zapper hides remain entirely under your control.
- Chrome Sync settings are governed by Google's privacy policy.

Questions:

**Email:** omiteyt@gmail.com

You may also contact your local data protection authority where applicable.

---

## 10. Children

AdImmunity is a general-audience extension.

It collects no personal information from anyone, including children.

---

## 11. Changes to This Policy

We may update this Privacy Policy to reflect changes to AdImmunity or applicable law.

Material updates will:

- Update the **Last updated** date.
- Be noted within the extension where reasonably practical.

Version history is available in the public GitHub repository.

**Last updated: 30 July 2026**

---

*AdImmunity — privacy-first ad & tracker blocking.*

**Contact:** omiteyt@gmail.com

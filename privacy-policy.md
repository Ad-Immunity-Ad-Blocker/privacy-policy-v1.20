# privacy-policy-v1.20
# AdImmunity — Privacy Policy

**Last updated: 29 May 2026**

*This policy will be hosted at a GitHub Pages URL once the repository's Pages site is configured. That URL will be linked from the Chrome Web Store listing and from within the extension.*

---

## 1. Who We Are / Contact

AdImmunity is a Chrome browser extension that blocks ads, trackers, and phishing attempts. It is developed and maintained by an independent maker based in the United States.

If you have any questions or requests regarding this Privacy Policy or your personal data, please contact us at:

**Email:** omiteyt@gmail.com

We will respond to all privacy-related enquiries within a reasonable time, and no later than 30 days for requests under applicable data protection law.

---

## 2. Summary

AdImmunity is built with a privacy-first design. The extension performs all ad and tracker blocking locally on your device using Chrome's built-in `declarativeNetRequest` API and content scripts. Your browsing activity never leaves your device as part of normal extension operation.

An account is entirely optional. You can use every blocking and filtering feature in AdImmunity without creating an account or providing any personal information whatsoever. An account is only needed if you wish to sync settings or access features that require authentication in the future.

Optional anonymous diagnostics are also available, but they are turned **off by default**. You must explicitly opt in to enable them, and you can turn them off again at any time.

---

## 3. What Stays on Your Device

AdImmunity relies exclusively on local browser storage for all core functionality. The following data is stored in `chrome.storage.local` and **never transmitted to any server**:

- **Blocking statistics** — counts of ads, trackers, and phishing attempts blocked during your sessions.
- **Extension settings** — your chosen blocking mode, enabled filter categories, and any other user preferences.
- **Whitelist (allowlist)** — the list of domains or pages you have chosen to exclude from blocking.
- **Element Zapper rules** — any custom element-hiding rules you have created using the visual Zapper tool.

This data lives entirely on your device. It is not uploaded, synced, or accessible to us under any circumstances unless you choose to create an optional account in the future and a sync feature is explicitly added (which would be disclosed in an updated policy).

The blocking mechanism itself works by matching network requests against filter lists using Chrome's `declarativeNetRequest` API. This process happens entirely within your browser. We do not intercept, log, or store URLs you visit, network requests you make, or any other browsing data.

---

## 4. Data We Collect with an Optional Account

Creating an account is entirely optional and has no effect on the core blocking functionality.

If you choose to create an account, we collect:

- **Email address** — used solely to authenticate you and allow you to log in. Your email is stored securely in Supabase Auth (see Section 7 on our processor and data location).

We do not collect your name, phone number, payment information, or any other personal details in connection with your account. Your account email is not used for marketing, is not shared with third parties for advertising, and is not combined with any browsing data.

You may delete your account at any time from within the extension using the **Delete account** button. Deletion is permanent and removes your email address from our systems.

---

## 5. Optional Anonymous Diagnostics

AdImmunity includes an optional, opt-in diagnostics feature that helps us identify and fix software errors. This feature is **off by default**. You must actively enable it in the extension settings.

When diagnostics are enabled, the following limited, anonymised information may be sent when the extension encounters an internal error:

- **Error signature (hash)** — a hash of the error type and location in code, used to identify the kind of error without revealing any personal information.
- **Capped stack trace sample** — a partial code stack trace, truncated to a fixed maximum length, showing which internal functions were involved in the error.
- **Extension version** — the version number of AdImmunity that produced the error (e.g., 1.1.0).
- **Browser version** — the version of Chrome or the Chromium-based browser you are using.
- **Operating system version** — the OS platform and version (e.g., Windows 10).

**What is explicitly NOT included in diagnostics:**

- Visited URLs or any part of a URL
- Page content, text, or HTML
- Any user identifier, account ID, or email address
- Browsing history or session information
- Search queries
- Usernames, passwords, or credentials
- Any data from your local extension storage (whitelist, settings, Zapper rules, stats)

Diagnostic reports contain no information that can identify you as an individual. They are used only to improve the stability and reliability of the extension.

You can disable diagnostics at any time in the extension settings. Doing so takes effect immediately; no further diagnostic data will be sent.

---

## 6. What We Never Collect

Regardless of whether you have an account or have opted in to diagnostics, AdImmunity **never** collects:

- Your browsing history
- The URLs of pages you visit
- The content of any web page you view
- Search queries you enter
- Usage statistics or patterns about how you browse the web
- Any form of persistent user identifier tied to your browsing activity
- Location data
- Financial or payment information

We have no technical capability to collect this data, and we have no interest in doing so. This is a foundational design principle of AdImmunity.

---

## 7. Processor & Data Location

We use **Supabase** as our data processor for account data. Supabase is a managed database and authentication platform that acts as our data processor under a Data Processing Agreement.

Account data (email addresses stored in Supabase Auth) is stored in the **European Union**, in the **Frankfurt, Germany (eu-central-1)** region.

Supabase processes your data solely on our behalf and in accordance with our instructions and applicable data protection law. Supabase does not use your data for its own purposes and does not sell it. For more information about Supabase's security and compliance, visit [https://supabase.com/security](https://supabase.com/security).

Anonymous diagnostic data, if you have opted in, is sent to the same Supabase instance in the EU/Frankfurt region, where it is aggregated and anonymised before retention (see Section 11 on data retention).

---

## 8. Legal Bases (GDPR Article 6)

If you are located in the European Economic Area (EEA), the United Kingdom, or Switzerland, we process personal data only when we have a valid legal basis under Article 6 of the General Data Protection Regulation (GDPR).

The legal bases we rely on are:

- **Consent (Article 6(1)(a))** — We process your email address only when you freely choose to create an account, which constitutes your explicit consent. We process anonymous diagnostic data only when you opt in to that feature. You may withdraw consent at any time (see Section 9).

We do not rely on legitimate interests or any other legal basis for the data described in this policy. We do not process any special category data (Article 9 GDPR).

---

## 9. Your Rights — GDPR

If you are in the EEA, UK, or Switzerland, you have the following rights regarding your personal data:

- **Right of access** — You may request a copy of the personal data we hold about you (your email address).
- **Right to rectification** — You may ask us to correct inaccurate personal data.
- **Right to erasure ("right to be forgotten")** — You may delete your account at any time using the **Delete account** button within the extension. This permanently removes your email address and any associated account data from our systems. You may also contact us at omiteyt@gmail.com to request erasure.
- **Right to data portability** — You may request your personal data in a structured, commonly used, machine-readable format.
- **Right to withdraw consent** — You may withdraw consent for account creation by deleting your account, and withdraw consent for diagnostics by disabling the opt-in setting. Withdrawal of consent does not affect the lawfulness of any processing that occurred before withdrawal.
- **Right to lodge a complaint** — You have the right to lodge a complaint with a supervisory authority in your country of residence. In Germany (where data is stored), the competent authority is the Hessian Commissioner for Data Protection and Freedom of Information (HBDI) at [https://datenschutz.hessen.de](https://datenschutz.hessen.de). You may also contact the supervisory authority in your own EU member state.

To exercise any of these rights, contact us at omiteyt@gmail.com. We will respond within one month. We do not charge a fee for these requests.

---

## 10. Your Rights — US / California (CCPA / CPRA)

If you are a California resident, you have the following rights under the California Consumer Privacy Act (CCPA) as amended by the California Privacy Rights Act (CPRA):

- **Right to know** — You have the right to know what personal information we collect about you, the categories and specific pieces of information, the purpose for collection, and whether we disclose it to third parties. This Privacy Policy provides that information. You may also contact us at omiteyt@gmail.com to make a formal request.
- **Right to delete** — You have the right to request deletion of personal information we have collected from you. You can delete your account directly within the extension, or contact us at omiteyt@gmail.com.
- **Right to non-discrimination** — We will not discriminate against you for exercising any of your CCPA rights. The extension's core blocking functionality is available to all users regardless of whether they have an account or have exercised any privacy rights.

**AdImmunity does not sell or share your personal information.** We do not sell personal information to third parties. We do not share personal information with third parties for cross-context behavioural advertising. This applies to all users, not just California residents.

Because we do not sell or share personal information, there is no opt-out required for data sales or sharing.

---

## 11. Data Retention

- **Account data (email address):** We retain your email address for as long as your account is active. When you delete your account — either through the in-app Delete account button or by contacting us — your email address is permanently deleted from Supabase Auth with no further retention.
- **Anonymous diagnostics:** Diagnostic reports are aggregated shortly after receipt. Aggregated, non-identifiable data may be retained for analysis; however, raw diagnostic submissions are retained for **no more than 90 days** before deletion. Because diagnostic data contains no user identifier, it cannot be linked to any individual after the aggregation period.
- **On-device data:** Your local storage data (stats, settings, whitelist, Zapper rules) is retained on your device indefinitely unless you uninstall the extension or clear browser data. We have no access to this data and therefore cannot delete it on your behalf; uninstalling the extension removes it.

---

## 12. Children

AdImmunity is not directed to children. You must be at least **16 years old** to create an account or to enable optional diagnostics. We do not knowingly collect personal information from anyone under 16. If you become aware that a child under 16 has provided us with personal data, please contact us at omiteyt@gmail.com and we will take prompt steps to delete it.

---

## 13. Changes to This Policy

We may update this Privacy Policy from time to time to reflect changes in the extension's features, applicable law, or our data practices. When we make a material change, we will update the "Last updated" date at the top of this document. We will also notify users via a notice within the extension where reasonably practicable.

We encourage you to review this policy periodically. Continued use of the extension after a policy update constitutes acceptance of the revised terms, subject to any rights you may exercise under applicable law.

The version history of this document is available in the extension's public GitHub repository.

**Last updated: 29 May 2026**

# Privacy Policy — Yoyatta

**Company:** Smart Soft K.K. (“we”, “us”, “our”)  
**Product:** Yoyatta iOS app, App Clip, booking pages, and related web services (“Yoyatta”)  
**Contact:** contact@smartsofuto.co.jp

**Registered office:**  
3-4-27 Takeshima, Takeshima Plaza 302,  
Nishiyodogawa-ku, Osaka City, Osaka Prefecture, Japan

**Last updated:** August 19, 2025

---

## 1) Overview
This Privacy Policy explains what personal data we collect, how we use it, how long we keep it, and your choices. Yoyatta helps Hosts publish availability and lets Bookers reserve time and automatically create online meetings (Zoom, Google Meet, Microsoft Teams, Cisco Webex).  
We do **not** access or store meeting audio, video, or chat content.

---

## 2) Scope
This Policy applies to:
- The **Yoyatta iOS app** and **App Clip** for Hosts and Bookers,
- **Booking pages** and related web UI (including free-tier pages that may show ads),
- Our APIs and background jobs hosted on **Cloudflare Workers** (with D1/KV/R2),
- Transactional emails we send (via **AWS SES**),
- Optional notifications to **Slack/Discord** if the Host connects webhooks.

---

## 3) Roles & Definitions
- **Host**: Creates and manages calendars (currently via iOS).  
- **Booker**: Reserves a time slot via web, App Clip, or app.  
- **Calendar**: A scheduling page at a unique slug/URL that a Host shares.  
- **Booking**: A reservation for a time slot on a Calendar.  
- **Meeting Link**: Join URL for Zoom/Teams/Meet/Webex.  
- **Calendar Key Pair**: Per-calendar Ed25519 keys used by the Host app to sign requests (private key stored on the Host device Keychain).  
- **Device Attestation**: Apple App Attest–based device binding used for certain host actions.  
- **Viewer Secret / Passcode**: Codes that gate access to booking details/cancellation links.  
- **Identity Providers (IdPs)**: Apple, Google, GitHub, Slack, LINE, Yahoo Japan (for sign-in).  
- **Gravatar**: Avatar service derived from an MD5 hash of an email, if enabled.

---

## 4) Data We Collect

### 4.1 Data you provide
**Hosts**
- Email address, display name (optional), profile image (or Gravatar),
- Calendar settings: name, description, rules (e.g., one-upcoming-booking limit, buffer time, allow/deny email domains, country allow/deny lists, password protection),
- Integrations you connect (Zoom/Google/Teams/Webex) and your choices for meeting creation,
- Optional Slack/Discord webhook URLs for notifications.

**Bookers**
- If you sign in with an IdP (Apple/Google/GitHub/Slack/LINE/Yahoo Japan): account subject identifier, email (or relay email where applicable), display name/avatar if the provider shares them,
- If you book by **entering an email**: the email address and any booking note/title you add,
- Selected time slot and timezone.

### 4.2 From integrations you link (Hosts)
- **Zoom**: user ID/email, OAuth scope, **access/refresh tokens**, meeting IDs, join URLs, passcodes (if enforced).  
- **Google/Meet** (usually via Google Calendar APIs): event IDs, **Meet join URLs**, and (if granted) **access/refresh tokens**.  
- **Microsoft Teams**: meeting IDs/join links and (if granted) **access/refresh tokens**.  
- **Cisco Webex**: person ID/email, OAuth scope, **access/refresh tokens**, meeting ID/number, join URL, password (if configured).  
We use these tokens **only** to create/update/cancel meetings you ask us to manage and to send .ics updates. We never read meeting content.

### 4.3 Collected automatically
- **Technical logs**: IP address, user-agent, timestamps, request IDs, error traces (with token redaction).  
- **Network/abuse signals**: country (geo-IP), **ASN**, VPN/hosting heuristics; used for anti-abuse and to enforce Host rules and may be **shown to the Host** in the iOS app.  
- **Security events**: results of Apple App Attest device checks, signature verification statuses, CAPTCHA (e.g., Cloudflare Turnstile) outcomes.  
- **Push delivery**: device push token (APNs) to send Host mobile notifications.  
- **Edge caches**: minimal, transient metadata for performance and DDoS/WAF protection.

### 4.4 Cookies & local/browser storage (web)
- **Strictly necessary cookies** for sessions and security (e.g., to remember a verified viewer).  
- **Analytics cookies** for feature-usage measurement (see §4.6).  
- **Advertising cookies** on **web pages** that show Google Ads (see §8).  
- **Local/session storage**: we may cache non-sensitive values (e.g., the presence of a calendar password or viewer secret) so the page can function. Avoid re-using sensitive passwords you use elsewhere.

### 4.5 iOS diagnostics (“auto bug reporting”)
- **Apple crash logs** if you enabled *Share with App Developers* in iOS. Logs can include device model, OS version, stack traces.  
- **In-app diagnostics** (if present and you opt in): anonymized performance/crash events. You can disable in **Settings → Diagnostics** or by turning off Apple’s sharing.

### 4.6 Analytics & feature usage
- **Feature-usage events** (e.g., “opened booking page,” “connected Zoom,” “booking success/fail type”) that do **not** include meeting content.  
- **IP handling for analytics**: IPs may be **hashed** (one-way) for deduplication/abuse control. We do not re-identify from these hashes.

### 4.7 Purchases & subscriptions
- **App Store receipts**, transaction IDs, product identifiers, entitlement status for in-app purchases/subscriptions. We do not receive your payment card details from Apple.

### 4.8 Passkeys (WebAuthn) (if you choose to use them)
- **Public credential ID** and **public key** associated with your account or booking claim. Biometric data never leaves your device; we do **not** receive it.

---

## 5) How We Use Data
- **Scheduling**: create/update/cancel bookings; generate and send **.ics** invites/updates.  
- **Integrations**: create/update/delete Zoom/Meet/Teams/Webex meetings on your behalf.  
- **Security**: verify device integrity (App Attest), enforce viewer secrets/passcodes, prevent abuse (Cloudflare WAF/Turnstile), anti-spam/disposable-email checks, rate limiting.  
- **Communications**: send confirmation, update (including ICS **REQUEST**), cancellation, and limited Host reminder emails (free-tier email caps may apply).  
- **Notifications**: deliver Host push notifications; optionally post to Slack/Discord **only if the Host connects a webhook**.  
- **Reliability & analytics**: monitor uptime/performance (aggregated) and feature usage to improve the service.  
- **Advertising (web)**: show and measure Google Ads on free-tier **web pages** (not in the iOS app).  
- **Compliance**: comply with law, enforce Terms, and protect rights and safety.

---

## 6) Sharing & Service Providers
We do **not** sell personal data. We share with processors/partners under contract or under their applicable terms:

- **Cloudflare** (Workers, D1/KV/R2, WAF/Zero-Trust, Turnstile, global network).  
- **Amazon Web Services (SES)** for transactional email delivery.  
- **Zoom / Google / Microsoft / Cisco Webex** used **only** when a Host connects them.  
- **Apple** (OS-level crash logs if you opted in; App Store purchase verification flows).  
- **Google Ads** on **web pages**: Google and partners may act as **independent controllers** for ad personalization/measurement under their policies (see §8).  
- **Slack/Discord**: if a Host adds a webhook, we deliver booking/cancellation metadata to that destination.

We may disclose data if required by law, regulation, legal process, or to protect people, property, and our services.

---

## 7) Legal Bases (EEA/UK where applicable)
- **Contract** (Art. 6(1)(b)): providing the scheduling service you request.  
- **Legitimate interests** (Art. 6(1)(f)): security/abuse prevention, service reliability, product improvement, non-invasive analytics, and showing ads on free-tier web pages.  
- **Consent** (Art. 6(1)(a)): where required for ads cookies on web pages, certain analytics, or when you choose to connect third-party integrations.  
- **Legal obligation** (Art. 6(1)(c)): compliance and regulatory requirements.

---

## 8) Advertising (Web Pages Only)
On **free-tier web pages** (e.g., booking pages or homepage), we may show ads via **Google Ads/AdSense/Ad Manager**.  
- When ad tags load, your browser may share IP address, user-agent, approximate location, and cookie identifiers with Google/partners.  
- Manage ad personalization in your Google account (Ads Settings) or via AdChoices/NAI opt-out tools; browsers/extensions can restrict third-party cookies.  
- We do **not** use third-party advertising SDKs or cookies **inside the iOS app**.

---

## 9) Data Retention
- **Bookings**: retained while active; after cancellation, either hard-deleted or marked cancelled based on Host settings and our operational needs (e.g., fraud prevention, audit).  
- **OAuth tokens**: retained while an integration remains connected; deleted when you disconnect or after repeated refresh failures.  
- **Logs & security events**: typically **30–90 days** for raw logs; aggregated analytics may be retained longer without direct identifiers.  
- **Push tokens**: retained while you receive notifications; removed when invalid/unsubscribed.  
- **Support**: retained as long as necessary to resolve your request and for reasonable archiving.

---

## 10) Security
- **In transit**: TLS 1.2/1.3, HSTS; HTTP/3 where supported.  
- **At rest**: Cloudflare D1/KV/R2 encryption; secrets in Cloudflare Workers Secrets; iOS tokens/keys in **Keychain** (Secure Enclave where available).  
- **Controls**: per-calendar signed requests (Ed25519), **Apple App Attest**, CAPTCHA, passcodes/viewer secrets, allow/deny rules, IP/country/ASN checks, rate limiting, least-privilege access, and regular review of access keys.  
No system is 100% secure; protect your devices and do not re-use sensitive passwords as calendar passcodes.

---

## 11) International Transfers
Our infrastructure (Cloudflare/AWS) may process data globally. Where required, we use appropriate safeguards consistent with applicable law (e.g., standard contractual clauses, intra-group measures, or adequacy decisions).

---

## 12) Your Choices & Controls
- **Disconnect integrations**: iOS app → **Settings → Integrations** → disconnect Zoom/Google/Teams/Webex.  
- **Manage bookings**: cancel via the link in emails or by signing in; .ics updates are sent.  
- **Diagnostics & analytics**: turn off OS-level sharing in iOS; contact us to request reduced analytics where feasible.  
- **Ads (web)**: use browser settings and Google/industry tools to control ad personalization.  
- **Gravatar**: upload a custom avatar or use an email without a Gravatar profile.  
- **Passkeys**: you can remove passkeys from your device’s passkey manager if you no longer wish to use them.  
- **Email preferences**: transactional emails are necessary for bookings; we do not send marketing emails without consent.

---

## 13) Data Subject Rights
Depending on your location (e.g., EEA/UK, Japan APPI, certain U.S. states), you may have rights to **access, correct, delete, export**, or **restrict** processing of your personal data, and the right to **object** to certain processing (including direct marketing).  
To exercise rights, email **contact@smartsofuto.co.jp**. We may need to verify your identity and identify the relevant booking(s) or account.

---

## 14) Participant Notice (Invitees who aren’t Yoyatta customers)
If you book time with a Yoyatta Host, we process your **email**, **selected time**, **timezone**, and may display **country/ASN** indicators to the Host for security and booking rules. We share the **meeting join link** with the Host and with you. We do not access meeting content.  
To request deletion or to make a data request, email **contact@smartsofuto.co.jp** with the booking details (date/time and Host).

---

## 15) Children’s Privacy
Yoyatta is not directed to children. Do not use the service if you are under 13 (or the minimum age in your jurisdiction).

---

## 16) Changes
We may update this Policy. We will update the “Last updated” date above and, where required, provide notice in-app or by email. Your continued use means you accept the changes.

---

## 17) Contact
Smart Soft K.K.  
3-4-27 Takeshima, Takeshima Plaza 302, Nishiyodogawa-ku, Osaka City, Osaka Prefecture, Japan  
Email: **contact@smartsofuto.co.jp**

---

## 18) Additional Disclosures & Notes

- **Identity Providers**: When you sign in with Apple/Google/GitHub/Slack/LINE/Yahoo Japan, those providers process your data under their own terms and privacy policies. We receive identifiers (and possibly email/display name) to operate your account and show your avatar.  
- **Slack/Discord Webhooks**: If a Host supplies a webhook URL, we send booking/cancellation metadata to that destination on the Host’s instructions. Slack/Discord will process that data under their policies; the Host controls what channels receive it.  
- **Disposable emails / abuse defense**: We may use third-party lists and heuristics to limit disposable or abusive sign-ups and to protect Hosts’ calendars.  
- **Calendar passwords & viewer secrets**: We process passcodes/secrets to enforce access controls. Do not reuse sensitive passwords you use for other services.  
- **Free vs. paid tiers**: Free Hosts may have email sending limits and see ads on web pages associated with their calendars; paid tiers reduce limits and remove ads on such pages.  
- **No meeting content**: We never record or store audio/video/screenshares/chat from your meetings. Meeting metadata (e.g., join URL, meeting ID) is stored only as needed to operate the feature.

---

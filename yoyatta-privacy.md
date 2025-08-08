# Privacy Policy — Yoyatta iOS App

**Company:** Smart Soft K.K. (“we”, “us”, “our”)  
**Product:** Yoyatta iOS app and related web services (“Yoyatta”)  
**Contact:** contact@smartsofuto.co.jp

**Registered office:**  
3-4-27 Takeshima  
Takeshima Plaza 302  
Nishiyodogawa-ku  
Osaka City, Osaka Prefecture  
Japan

**Last updated:** August 8, 2025

## 1) Overview
This Privacy Policy explains what personal data we collect, how we use it, how long we keep it, and your choices. Yoyatta helps you publish availability and automatically create online meetings (Zoom, Google Meet, Cisco Webex). We do **not** access or store meeting audio, video, or chat content.

## 2) Scope
This Policy applies to:
- The Yoyatta iOS app and booking pages,
- Our APIs hosted on Cloudflare Workers,
- Transactional emails we send (via AWS SES).

## 3) Data We Collect
### 3.1 Data you provide
- **Account & contact:** email address, name (optional), profile image (or Gravatar).
- **Booking data:** selected slot, timezone, meeting title/note (if provided), invitee email.
- **Integration consent:** when you connect Zoom/Google/Webex we receive authorization to create and manage meetings on your behalf.

### 3.2 Collected automatically
- **Technical logs:** IP address, user-agent, timestamps, request IDs, error traces (with token redaction).
- **Cookies (web):**  
  - **Strictly necessary** cookies for sessions and security,  
  - **Analytics** cookies for feature-usage measurement (see §3.6),  
  - **Advertising** cookies on our **web pages** to serve Google Ads (see §3.8).  
  We do not use third-party advertising cookies inside the iOS app.

### 3.3 iOS diagnostics (“auto bug reporting”)
- **Apple crash logs:** If you’ve enabled *Share with App Developers* in iOS, Apple may share crash logs with us that can include device model, OS version, and stack traces.  
- **In-app diagnostics (if enabled):** The app may collect anonymized performance and crash events. You can disable this in **Settings → Diagnostics** inside the app (if present) or by turning off Apple’s sharing.

### 3.4 From integrations you link
- **Zoom:** Zoom user ID and email, OAuth scope, **access/refresh tokens**, meeting IDs, join URLs, and passcodes (if enforced).  
- **Google Meet:** Typically created via Google Calendar APIs. We store the Calendar event ID and **Meet join URL**; if you grant offline access we store **access/refresh tokens**.  
- **Cisco Webex:** Webex person ID/email, OAuth scope, **access/refresh tokens**, meeting ID/number, join URL, and password (if configured).

> We use these tokens **only** to create/update/delete meetings you ask us to manage. We never read meeting content.

### 3.5 Account identity (Apple)
- **Apple-provided identifiers:** We use Apple-provided identifiers to identify your account, such as a **CloudKit record identifier** or, if you use Sign in with Apple, the **Apple subject identifier** (and relay email if you choose “Hide My Email”). We do **not** receive your Apple ID password.

### 3.6 Analytics & feature usage
- **Event analytics:** We collect **feature-usage events** to understand which parts of the app are used most (e.g., “opened booking page,” “connected Zoom”). These events do **not** include personal message content or meeting content.  
- **IP handling for analytics:** For abuse detection and de-duplication, IP addresses related to analytics events may be **hashed** (one-way) before storage. We do not attempt to re-identify you from these hashes.

### 3.7 Purchases & subscriptions
- **Subscription verification:** To validate in-app purchases and subscriptions, we process **App Store receipts, transaction IDs, product identifiers, and entitlement status**. Verification may occur on-device and server-side (e.g., with Apple’s App Store Server APIs). We do **not** receive your payment card details from Apple.

### 3.8 Advertising on the web (Google Ads)
- **Web ads only:** Our **web pages** (not the iOS app) may show ads via **Google Ads/AdSense/Ad Manager**. Google and its partners may use cookies and similar technologies to serve and measure ads based on prior visits to our site and other sites.  
- **Data involved:** When ad tags load, your browser may share standard information such as IP address, user-agent, approximate location, and cookie identifiers directly with Google or its partners.  
- **Your choices:** You can manage ad personalization in your Google account (Google Ads Settings) or via industry tools such as AdChoices/NAI opt-out. Browser settings and extensions can also restrict third-party cookies. Disabling cookies may impact ad relevance.

## 4) How We Use Data
- **Scheduling:** create/update/cancel bookings; generate calendar files (.ics).  
- **Integrations:** create/delete meetings in Zoom/Google/Webex on your behalf.  
- **Security:** verify device integrity (Apple App Attest), prevent abuse (Cloudflare WAF/Turnstile), investigate fraud.  
- **Communications:** send confirmation and cancellation emails.  
- **Reliability & analytics:** monitor uptime/performance in aggregate; measure feature usage (see §3.6) to improve the service.  
- **Advertising (web):** show and measure Google Ads on our **web pages** (see §3.8).  
- **Compliance:** comply with applicable laws and enforce our Terms.

## 5) Sharing & Service Providers
We do not sell personal data. We share with processors/partners under contract or their applicable terms:
- **Cloudflare** (hosting, D1/KV/R2 storage, WAF/Zero-Trust, Turnstile),  
- **Amazon Web Services (SES)** (transactional email),  
- **Zoom / Google / Cisco Webex** (only when you connect them for meetings),  
- **Apple** (crash logs if you’ve opted in at the OS level),  
- **Google Ads** (ads on our **web pages**; Google may act as an independent controller for ad personalization under its own policies).  
Disclosures may occur if required by law or to protect rights and safety.

## 6) Data Retention
- **Bookings:** kept while active; on cancellation we either hard-delete or mark cancelled per host settings.  
- **OAuth tokens:** retained while the integration is connected; deleted when you disconnect or after repeated refresh failures.  
- **Logs & analytics:** minimal PII; typical retention **30–90 days** for raw logs; analytics may be retained longer in aggregated, non-identifying form.  
- **Support:** retained as long as necessary to resolve your request.

## 7) Security
- **In transit:** TLS 1.2/1.3, HSTS, HTTP/3 on supported clients.  
- **At rest:** Cloudflare D1/KV/R2 encrypted; secrets in Cloudflare Workers Secrets; iOS tokens in **Keychain** (Secure Enclave where supported).  
- **Controls:** device attestation, HMAC-signed links, rate limiting, WAF rules, least-privilege access.

## 8) International Transfers
Our infrastructure (Cloudflare/AWS) may process data globally. Where required, we use appropriate safeguards consistent with applicable law.

## 9) Your Choices & Controls
- **Unlink Zoom/Google/Webex:** In the app, go to **Settings → Integrations → (Zoom/Google/Webex) → Disconnect**. This revokes our use and removes the tokens from our DB.  
- **Delete bookings:** Cancel bookings via the app or cancellation links.  
- **Diagnostics & analytics:** You can turn off iOS developer sharing in system settings; if you wish to opt out of in-app analytics, contact us at **contact@smartsofuto.co.jp** and we will honor your request where feasible.  
- **Ads on the web:** Manage Google ad personalization in your Google account or via AdChoices/NAI industry tools; you can also restrict cookies in your browser.  
- **Email preferences:** Transactional emails are necessary for bookings; we do not send marketing emails without consent.

## 10) Participant Notice (Invitees who aren’t Yoyatta customers)
If you book a time with a Yoyatta host, we process your **email**, **selected time**, and **timezone** to schedule the meeting and send confirmations. We share the meeting join link with the host and with you. We do **not** access meeting content. To request deletion of your booking data or to make another data request, email **contact@smartsofuto.co.jp** and include the booking details (date/time and host).

## 11) Children’s Privacy
Yoyatta is not directed to children. Do not use the service if you are under 13 (or the minimum age in your jurisdiction).

## 12) Changes
We may update this Policy and will post the new date above. Material changes may be notified in-app or by email.

## 13) Contact
Smart Soft K.K.  
3-4-27 Takeshima, Takeshima Plaza 302, Nishiyodogawa-ku, Osaka City, Osaka Prefecture, Japan  
Email: **contact@smartsofuto.co.jp**

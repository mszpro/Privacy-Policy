Privacy Policy for Mini Walkie Talkie

Effective Date: May 14, 2026

This Privacy Policy explains how Mini Walkie Talkie (the "App," "Service," "we," "us," or "our") collects, uses, stores, and protects information when you use the App.

Please replace the bracketed items above before publishing this policy.

1. Summary

Mini Walkie Talkie is an end-to-end encrypted push-to-talk walkie talkie app. The App lets users add trusted contacts by scanning QR codes and send voice messages through nearby routes, direct internet routes, and, for Pro background receiving, an encrypted online relay fallback.

We design the App so that voice audio is encrypted before it leaves your device. Direct nearby or WebRTC traffic is carried as encrypted packets. When Pro background receiving uses the online relay fallback, the relay stores only encrypted audio data and deletes it after the recipient receives it, with a 24-hour purge rule as a backup.

We do not sell your personal information. We do not use your voice audio for advertising.

2. Information We Collect

2.1 Account and Device Identity Information

The App may create or process:

- A user ID generated for the App.
- Your display name or profile label, if you set one.
- Public cryptographic identity keys used for contact verification and end-to-end encryption.
- Signed contact profile data used in QR code contact exchange.
- Contact approval records between you and other users.
- Push notification tokens, including Push-to-Talk tokens, used to notify your device of incoming walkie talkie activity.
- Subscription status or entitlement status, such as whether Pro background receiving is active.

2.2 Contact and QR Code Information

The App lets users add contacts by scanning each other's QR code. QR codes may contain signed public identity information, an invite nonce, issue and expiry timestamps, and related contact setup data.

The App does not need access to your phone address book unless a future version asks for that permission. App contacts are trusted walkie talkie contacts created inside the App.

2.3 Voice Audio and Messages

When you press and hold to talk, the App records voice audio on your device and encodes it for push-to-talk delivery.

Direct routes:
- When sent through nearby networking or WebRTC, voice messages are transmitted as encrypted packets.
- We do not store direct-route audio on our servers.

Encrypted relay fallback:
- Pro background receiving may use an online relay fallback when direct routes are not available.
- The relay stores encrypted audio only.
- The relay does not receive the decryption key.
- For each sender-to-recipient pair, the relay keeps only the latest audio piece.
- The relay deletes the audio piece when the recipient successfully fetches it.
- A 24-hour purge rule is used as a backup cleanup mechanism for relay audio that was not fetched or deleted normally.
- Relay uploads are limited in duration and size by both the client and the server.

2.4 Transfer Metadata and Diagnostics

To provide the Service, debug delivery problems, and show users recent transfer details, the App and server may process limited metadata such as:

- Sender and recipient user IDs.
- Delivery IDs or talk session IDs.
- Message route used, such as Nearby, WebRTC, or encrypted relay.
- Approximate audio duration.
- Encrypted payload size or transferred byte count.
- Timestamps.
- Delivery acknowledgements, such as wake, route, received, queued, or playback status.
- Error states, such as route unavailable, WebRTC unavailable, or relay fallback used.

This metadata helps the App decide the best route, show recent sent/received transfer information, and improve reliability.

2.5 Subscription and Purchase Information

If you purchase Pro, Apple processes your payment through the App Store. We do not receive your full payment card details.

We may receive or process App Store receipt or transaction information needed to verify your subscription status and unlock Pro features.

2.6 Technical Information

When your device communicates with our server, our infrastructure may process standard technical information, such as:

- IP address.
- Request time.
- App version or API version.
- Device platform.
- Network request headers.
- Error logs or server logs.
- Security and abuse-prevention logs.

2.7 Support Communications

If you contact us for support, we may collect the information you provide, such as your email address, screenshots, logs, diagnostic files, and messages.

3. Information We Do Not Intentionally Collect

We do not intentionally collect:

- Your precise GPS location.
- Your phone address book contacts, unless a future version explicitly asks for permission.
- Your payment card number.
- Unencrypted relay audio.
- Data for third-party advertising.
- Data to sell to data brokers.

4. How We Use Information

We use information to:

- Provide push-to-talk communication features.
- Add and verify trusted contacts.
- Route messages through Nearby, WebRTC, or encrypted relay fallback.
- Send Push-to-Talk and other notifications.
- Verify Pro subscription status.
- Provide Pro background receiving.
- Maintain security and prevent abuse.
- Diagnose failed deliveries and network issues.
- Show recent sent and received transfer details inside the App.
- Respond to support requests.
- Comply with legal obligations.

5. End-to-End Encryption and Security

The App uses device-generated cryptographic identity keys and signed contact verification. Voice sessions use authenticated encryption and replay protection.

The current design uses technologies such as P-256 identity and key agreement keys, signed QR contact verification, per-session key exchange, HKDF-SHA256 key derivation, and ChaChaPoly authenticated encryption.

Your audio is encrypted before it leaves your device. The online relay, when used, handles encrypted audio data only and is not designed to decrypt your voice messages.

No security system is perfect. We cannot guarantee that unauthorized access, data loss, or service failure will never occur.

6. Online Relay Fallback

The online relay exists to improve background receiving reliability for Pro users when direct nearby or WebRTC routes are unavailable.

The relay is designed with these limits:

- It is a fallback route, not the first route.
- Nearby is preferred first.
- WebRTC is preferred second.
- R2 encrypted relay fallback is used only when needed and allowed.
- Audio relay data is encrypted client-side.
- The server keeps only the latest audio piece for each sender-to-recipient pair.
- The relay deletes the audio after the recipient fetches it.
- A 24-hour purge rule is used as backup cleanup.
- Client and server enforce duration and upload size limits.

7. Notifications

The App uses notifications, including Push-to-Talk notifications, to alert your device that someone is trying to send you a walkie talkie message.

For free users, background receiving is best-effort. Notifications may tell you that a message is available and that you should unlock Pro or keep the App open to listen in the background.

You can control notification permissions in your device settings.

8. Data Sharing

We may share information with service providers only as needed to operate the App, such as:

- Apple, for App Store purchases, subscriptions, Push Notifications, Push-to-Talk, and platform services.
- Cloud infrastructure providers, for API hosting, database storage, encrypted relay object storage, and network delivery.
- Diagnostic or crash reporting providers, if used in the App or enabled through Apple diagnostics.
- Legal or safety authorities, if required by law or necessary to protect rights, safety, or security.

We do not sell your personal information.

9. Data Retention

We keep information only for as long as reasonably necessary for the purposes described in this policy.

Typical retention includes:

- App account and contact approval records: retained while your account or contact relationship is active.
- Push tokens: retained while needed to send notifications and replaced when updated.
- Subscription status: retained while needed to provide Pro features and handle account history.
- Transfer metadata and acknowledgements: retained for service reliability, debugging, abuse prevention, and in-app recent transfer history.
- Encrypted relay audio: normally deleted when fetched by the recipient; backup lifecycle purge after 24 hours.
- Local message history and diagnostics: stored on your device unless sent to us for support or synced through features you enable.

10. Your Choices and Rights

Depending on your location, you may have rights to access, correct, delete, or export your personal information.

You can:

- Remove contacts in the App.
- Disable notifications in system settings.
- Cancel Pro through your Apple App Store account settings.
- Delete local App data by deleting the App from your device.
- Contact us to request account-related deletion or privacy help.

Some server-side records may be retained if required for security, fraud prevention, legal compliance, or legitimate business needs.

11. Children

The App is not intended for children under 13 or the minimum age required by local law. If you believe a child has provided personal information to us, contact us so we can take appropriate action.

12. International Data Transfers

Our service providers may process data in countries other than where you live. Those countries may have different data protection laws. Where required, we use appropriate safeguards for international transfers.

13. Legal Bases for Processing

If you are in the European Economic Area, United Kingdom, or another region requiring legal bases, we process information based on:

- Contract necessity, to provide the App and Pro features.
- Consent, where required, such as notification permissions.
- Legitimate interests, such as security, reliability, debugging, and abuse prevention.
- Legal obligations, when we must comply with applicable law.

14. California Privacy Notice

We do not sell personal information. We do not knowingly share personal information for cross-context behavioral advertising.

California users may have rights to know, access, delete, correct, and limit certain uses of personal information. To exercise these rights, contact us using the contact details above.

15. Changes to This Policy

We may update this Privacy Policy from time to time. If we make material changes, we will update the effective date and may provide notice in the App or on our website.

16. Contact

If you have questions about this Privacy Policy or your data, contact:

Developer / Company: AsterKit Software Limited
Contact Email: me@mszpro.com

Terms of Service for Mini Walkie Talkie

Effective Date: May 14, 2026

These Terms of Service ("Terms") govern your access to and use of Mini Walkie Talkie (the "App," "Service," "we," "us," or "our").

Please replace the bracketed items above before publishing these Terms.

These Terms are in addition to Apple's Standard End User License Agreement ("Standard EULA"), which is available at:
https://www.apple.com/legal/internet-services/itunes/dev/stdeula/

By installing, accessing, or using the Service, you agree to these Terms. If you do not agree, do not use the Service.

1. Scope of Service

Mini Walkie Talkie is an end-to-end encrypted push-to-talk walkie talkie app. It lets users add trusted contacts through QR code exchange and send voice messages using nearby routes, direct internet routes, and, for eligible Pro background receiving, encrypted online relay fallback.

The Service may use technologies such as:

- Nearby networking, including Bluetooth and Wi-Fi based peer-to-peer communication when available.
- Internet WebRTC direct connection when available.
- Apple Push Notifications and Push-to-Talk notifications.
- Encrypted online relay fallback for eligible Pro background receiving.
- Local device storage for contacts, settings, and recent transfer details.
- Server-side account, contact approval, subscription verification, push token, and encrypted relay metadata.

The Service is designed for casual and private communication with trusted contacts. It is not an emergency communication service.

2. Relationship to Apple's Standard EULA

If you download the App from the Apple App Store, Apple's Standard EULA applies unless a custom license agreement is provided in App Store Connect. These Terms supplement Apple's Standard EULA and govern your use of the Service and related online features.

If these Terms conflict with Apple's Standard EULA, Apple's Standard EULA controls only to the extent required by Apple or applicable law.

3. User Content

"User Content" means content that you create, send, receive, upload, or process through the Service, including voice messages, contact names, display names, QR code contact information, message metadata, and support communications.

You retain ownership of your User Content. You grant us a limited license to process User Content only as needed to provide, secure, maintain, and improve the Service, including routing encrypted messages, sending notifications, verifying subscriptions, handling support, and preventing abuse.

You are solely responsible for your User Content and your use of the Service.

4. End-to-End Encryption

The Service is designed to encrypt voice audio before it leaves your device. Direct nearby and WebRTC routes carry encrypted packets. The encrypted online relay fallback, when used, stores encrypted audio only and is not designed to decrypt your voice messages.

The App may use device-generated cryptographic identity keys, signed QR contact verification, per-session key exchange, HKDF-SHA256 key derivation, and ChaChaPoly authenticated encryption.

You understand that no security system is perfect. We do not guarantee that unauthorized access, service interruption, or data loss can never happen.

5. Online Relay Fallback

The App prefers routes in this order:

1. Nearby route, when available.
2. WebRTC direct route, when available.
3. Encrypted online relay fallback, when allowed and needed.

Encrypted online relay fallback is intended to improve background receiving reliability for Pro users when direct routes are unavailable.

The relay is subject to limits:

- Relay uploads may be available only for messages to users who have Pro background receiving or an override entitlement.
- The relay keeps only the latest encrypted audio piece for each sender-to-recipient pair.
- The relay deletes the encrypted audio after the recipient fetches it.
- A 24-hour purge rule is used as backup cleanup.
- The client and server enforce duration and size limits.
- Relay delivery is not guaranteed.

6. Free and Pro Features

Free users can use nearby and direct internet routes on a best-effort basis. For best reliability on Free, keep the App open.

Pro may unlock additional features, including more reliable background receiving with encrypted relay fallback when direct routes are unavailable.

We may change Free and Pro feature availability from time to time, subject to applicable law and App Store rules. We will not intentionally remove paid features during an active subscription period except where necessary for security, legal, technical, or operational reasons.

7. Subscriptions, Billing, Cancellation, and Refunds

Pro subscriptions are purchased through Apple's App Store.

Subscriptions automatically renew unless cancelled through your Apple App Store account settings before the renewal date. Apple handles billing, cancellation, and refunds according to Apple's terms and policies.

We do not receive your full payment card details. We may receive receipt or transaction information needed to verify your Pro entitlement.

If you cancel a subscription, your Pro access continues until the end of the current paid subscription period unless Apple determines otherwise. We do not provide credits, refunds, or prorated billing directly. Refund requests are handled by Apple.

8. Push Notifications and Background Receiving

The Service uses notifications, including Push-to-Talk notifications, to alert devices of incoming communication.

Background receiving is not guaranteed. Device settings, network conditions, battery state, operating system limits, App Store entitlements, and service availability may affect whether a message is delivered or played in the background.

Free background receiving is best-effort using direct routes such as nearby and WebRTC when available. Pro background receiving may use encrypted relay fallback when eligible.

9. No Emergency Use

The Service is not a replacement for emergency calling, public safety radio, disaster communication systems, or professional dispatch systems.

Do not rely on the Service for emergencies, life safety, medical emergencies, law enforcement, fire response, rescue operations, or any critical communication where delay, failure, or missed messages could cause harm.

10. Acceptable Use

You agree not to use the Service to:

- Violate any law or regulation.
- Harass, threaten, abuse, stalk, impersonate, or defame another person.
- Send unlawful, harmful, exploitative, hateful, or abusive content.
- Violate privacy, publicity, copyright, trademark, contractual, or other rights.
- Record or transmit communications without required consent.
- Interfere with, disrupt, reverse engineer, overload, or attack the Service.
- Attempt to bypass subscriptions, entitlements, rate limits, size limits, encryption, or security controls.
- Use the Service for spam, scams, fraud, or unauthorized commercial messaging.
- Use the Service for emergency, safety-critical, or regulated radio communication where the Service is not approved for that purpose.

11. Contact Consent and QR Code Exchange

You should add contacts only with their consent. You are responsible for verifying that the person whose QR code you scan is the person you intend to communicate with.

We are not responsible for impersonation, mistaken identity, unauthorized QR sharing, or contact setup mistakes caused by users.

12. Availability and Route Selection

The App attempts to choose the best available route, but route selection and message delivery are not guaranteed.

Nearby routes may fail due to distance, interference, device settings, Bluetooth/Wi-Fi conditions, operating system restrictions, or app state.

WebRTC routes may fail due to NAT, firewall, network conditions, missing dependencies, relay restrictions, or platform behavior.

Relay fallback may fail due to subscription status, entitlement state, upload size, server availability, network failure, or expiration.

You accept that voice messages may be delayed, missed, dropped, duplicated, or unavailable.

13. Third-Party Services

The Service may depend on third-party or platform services, including Apple services, push notification services, App Store subscription services, WebRTC-related services, and cloud infrastructure providers.

We are not responsible for outages, changes, limitations, or failures of third-party services.

14. Privacy

Our Privacy Policy explains how we collect, use, store, and protect information. By using the Service, you agree to our Privacy Policy.

Privacy Policy URL: https://raw.githubusercontent.com/mszpro/Privacy-Policy/refs/heads/main/WalkieTalkie-privacy.md

15. Warranty Disclaimer

TO THE MAXIMUM EXTENT PERMITTED BY APPLICABLE LAW, THE SERVICE IS PROVIDED "AS IS" AND "AS AVAILABLE," WITH ALL FAULTS AND WITHOUT WARRANTIES OF ANY KIND.

WE DISCLAIM ALL WARRANTIES, EXPRESS, IMPLIED, OR STATUTORY, INCLUDING WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, TITLE, NON-INFRINGEMENT, ACCURACY, RELIABILITY, AVAILABILITY, SECURITY, AND QUIET ENJOYMENT.

WE DO NOT WARRANT THAT THE SERVICE WILL BE UNINTERRUPTED, ERROR-FREE, SECURE, PRIVATE, AVAILABLE IN ALL LOCATIONS, OR THAT MESSAGES WILL ALWAYS BE DELIVERED OR PLAYED.

16. Limitation of Liability

TO THE MAXIMUM EXTENT PERMITTED BY APPLICABLE LAW, WE WILL NOT BE LIABLE FOR ANY INDIRECT, INCIDENTAL, SPECIAL, CONSEQUENTIAL, EXEMPLARY, OR PUNITIVE DAMAGES, INCLUDING LOSS OF PROFITS, LOSS OF DATA, LOSS OF BUSINESS, LOSS OF GOODWILL, DEVICE DAMAGE, MISSED MESSAGES, FAILED DELIVERIES, SERVICE INTERRUPTION, OR COMMUNICATION FAILURE.

TO THE MAXIMUM EXTENT PERMITTED BY APPLICABLE LAW, OUR TOTAL LIABILITY FOR ALL CLAIMS RELATING TO THE SERVICE WILL NOT EXCEED THE GREATER OF:

- THE AMOUNT YOU PAID US THROUGH THE APP STORE FOR THE SERVICE IN THE 12 MONTHS BEFORE THE CLAIM; OR
- USD $50.

Some jurisdictions do not allow certain exclusions or limitations. In those jurisdictions, our liability is limited to the maximum extent permitted by law.

17. Indemnification

You agree to indemnify, defend, and hold harmless the Company, its owners, officers, directors, employees, contractors, agents, licensors, and service providers from and against claims, losses, liabilities, damages, costs, and expenses, including reasonable attorneys' fees, arising from or related to:

- Your use or misuse of the Service.
- Your User Content.
- Your violation of these Terms.
- Your violation of law.
- Your violation of another person's rights.
- Your communications with other users.

18. Suspension and Termination

We may suspend, restrict, or terminate your access to the Service if we believe that:

- You violated these Terms.
- Your use creates risk or legal exposure.
- Your use harms other users, the Service, or third parties.
- We are required to do so by law or platform rules.
- Technical, operational, security, or business reasons require it.

You may stop using the Service at any time. Deleting the App may remove local data from your device but may not delete server-side records immediately.

19. Ownership and Intellectual Property

The Service, including software, design, trademarks, logos, technology, documentation, and related intellectual property, is owned by us or our licensors.

Except for rights expressly granted to you, all rights are reserved. You may not copy, modify, distribute, sell, lease, reverse engineer, or create derivative works from the Service except as permitted by law or applicable open-source licenses.

20. Feedback

If you provide feedback, suggestions, ideas, bug reports, or feature requests, you grant us the right to use them without restriction or compensation.

21. Export Compliance

You may not use, export, or re-export the App except as authorized by applicable law. You represent that you are not located in a country or on a list where use of the App is prohibited by applicable export control or sanctions laws.

22. Changes to the Service

We may modify, suspend, or discontinue parts of the Service at any time. We may update route selection, relay behavior, subscription features, size limits, duration limits, cryptographic implementation, or supported platforms for technical, security, legal, operational, or product reasons.

23. Changes to These Terms

We may update these Terms from time to time. If we make material changes, we will update the effective date and may notify you in the App or on our website. Your continued use of the Service after changes become effective means you accept the updated Terms.

24. Governing Law

Unless required otherwise by applicable law or Apple's Standard EULA, these Terms are governed by the laws of [Governing Law Jurisdiction], without regard to conflict of law rules.

If you are a consumer in a jurisdiction that gives you mandatory local rights, nothing in these Terms limits those mandatory rights.

25. Severability

If any provision of these Terms is found unenforceable, the remaining provisions will remain in effect.

26. Entire Agreement

These Terms, together with the Privacy Policy and Apple's Standard EULA where applicable, form the entire agreement between you and us regarding the Service.

27. Contact

If you have questions about these Terms, contact:

Developer / Company: AsterKit Software Limited
Email: me@mszpro.com

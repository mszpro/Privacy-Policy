Yoyatta — Terms of Service (ToS)

Last updated: August 19, 2025 (JST)

Summary (non-binding): Yoyatta (also referred to as Yoyakun) is scheduling software. “Hosts” make calendars; “Bookers” reserve time. We provide tools (iOS app for Hosts, web/app for Bookers), optional sign-in via third parties, and integrations with meeting providers (e.g., Zoom/Teams/Meet/Webex). We are not a party to any meeting you schedule. Some features are free (1 calendar), paid tiers unlock more (up to 10 calendars). Use must be lawful and respectful; no spam, abuse, or fraud. These Terms include important limitations and disclaimers—please read them carefully.

⸻

1) Agreement & Operator

These Terms of Service (“Terms”) are a binding agreement between Smart Soft K.K. (the “Company”, “we”, “us”, or “our”) and you (“you”). They govern your access to and use of Yoyatta/Yoyakun (the “Service”), including our iOS app, App Clip, websites, APIs, and related communications.

By accessing or using the Service, you agree to these Terms and our Privacy Policy (separate document). If you are using the Service for an organization, you represent that you have authority to bind that organization.

Placeholders to customize
• Operator/Company: Smart Soft K.K.
• Contact email: me@smartsofuto.co.jp
• Address: 555-0011
Nishiyodogawa-ku, Osaka City, Osaka Prefecture
3-4-27 Takeshima
Takeshima Plaza 302

⸻

2) Definitions
	•	Host: A user who creates and manages a calendar others can book. Hosts currently use the iOS app.
	•	Booker: A user who reserves a time slot via the web, App Clip, or app.
	•	Calendar: A scheduling page a Host shares via a unique slug/URL.
	•	Booking: A reservation for a time slot on a Calendar.
	•	Meeting Link: A join URL for Zoom, Microsoft Teams, Google Meet, Webex, or similar.
	•	Calendar Key Pair: Per-calendar Ed25519 keys used by the Host app to sign requests. Private keys are stored on the Host device (Keychain).
	•	Device Attestation: Apple App Attest–based device binding used for certain host actions.
	•	Viewer Secret / Passcode: Codes that gate access to booking detail or cancellation links.
	•	Third-Party Providers: Identity providers (Apple, Google, GitHub, Slack, LINE, Yahoo Japan) and meeting providers (Zoom, Teams, Meet, Webex), among others.
	•	Gravatar: Avatar service; we may derive an avatar by hashing an email address (MD5) unless customized.

⸻

3) The Service

3.1 For Hosts (iOS app)
	•	Create calendars (1 on free tier; up to 10 on paid tiers).
	•	Configure name/description and system-generated slug (not manually editable).
	•	Set weekly availability via ruler selector; add exceptions; later adjust booking rules.
	•	Booking rules include (examples):
	•	Limit one upcoming booking per email.
	•	Buffer time before/after meetings.
	•	Restrict who can book (allow list of emails or domain suffixes; enterprise domain).
	•	Denylist emails/domains and country-based allow/deny rules.
	•	Password-protected calendars.
	•	Integrate Zoom/Teams/Meet/Webex. You may update/set the meeting link later; we email the Booker an update (ICS REQUEST) and respect free-tier email caps.
	•	Receive email and push notifications for new bookings/cancellations.
	•	Manage bookings and (where enabled) send one reminder email per booking.

3.2 For Bookers (web/app/App Clip)
	•	Book via web/App Clip and optionally sign in with Apple/Google/GitHub/Slack/LINE/Yahoo Japan.
	•	You can cancel anytime using the link or by logging in.
	•	Choose preferred meeting software if the Host offers options.
	•	Your avatar may appear via Gravatar or your customization.

3.3 Security & Abuse-Defense (Overview)
	•	Ed25519-signed host actions; device attestation for certain device-bound operations.
	•	CAPTCHA (e.g., Cloudflare Turnstile) on booking pages.
	•	Viewer-secret/passcode protections on detail/cancel links.
	•	Network-level and policy-level measures (e.g., IP/country/ASN-aware controls).
	•	Credentials are encrypted; the Host app avoids a traditional username/password sign-up by design.
	•	We may rate-limit, throttle, or suspend activity to protect the Service.

We are a software platform. We do not host your meetings and are not a party to the agreements between Hosts and Bookers.

⸻

4) Accounts & Authentication
	•	Hosts use the iOS app; core host operations are signed with per-calendar keys and may require device attestation. Keep your device and keys secure—loss or compromise is your responsibility.
	•	Bookers may sign in with a third-party identity provider. Your use of a provider is subject to that provider’s terms and privacy practices.
	•	We may refuse, reclaim, or change a Calendar slug if it causes confusion, violates rights, or is abusive.

Age. You must be at least 13 (or the age of digital consent where you live—e.g., 16 in parts of the EU). If you use the Service for a company, you confirm you’re authorized to do so.

⸻

5) Plans, Billing, and In-App Purchases
	•	Free Tier: 1 calendar, email-sending caps, and other limits may apply.
	•	Paid Tiers: Up to 10 calendars and additional limits/quotas as described in-app.
	•	Billing: Subscriptions (if offered) are typically handled via Apple In-App Purchase (IAP). Billing, renewals, cancellations, and refunds are governed by Apple’s terms and the App Store’s rules. Manage or cancel your subscription through your Apple ID settings. We do not directly process or store IAP payment card data.
	•	We may change prices or plan features with notice as required by law or platform policy. Changes usually take effect on your next billing cycle.

⸻

6) Booking Relationship & Host Responsibilities
	•	No Service Guarantee to Attend: We provide scheduling tools. We do not guarantee attendance, outcome, or quality of meetings.
	•	Host Content: You’re responsible for the accuracy of your calendar details (availability, descriptions), booking rules, and meeting links (including replacements/updates).
	•	Compliance: Hosts must comply with applicable laws, including data protection, marketing, and consumer rules.
	•	Reminders/Emails: Hosts may send limited reminders through the Service; free-tier caps apply. Do not use the Service to send spam or unlawful communications.
	•	Booking Rules: Rules like “one upcoming booking per email,” allow/deny lists, country limits, and password protection are implemented by you. You are responsible for the consequences of the rules you configure.

⸻

7) Acceptable Use

You agree not to:
	•	Use the Service for unlawful, harmful, fraudulent, or deceptive purposes.
	•	Harass, threaten, or defame others; post or transmit hateful or obscene material.
	•	Attempt to bypass security, rate limits, or access controls (e.g., viewer secrets, passcodes).
	•	Interfere with or disrupt the Service, including via scraping that degrades performance.
	•	Misrepresent your identity or affiliation.
	•	Upload or link malicious code, perform XSS/SQLi attacks, or exploit injection vectors.
	•	Abuse email or notification features (spam, deceptive content, or prohibited marketing).
	•	Infringe or misappropriate any intellectual property or privacy rights.

We may investigate and take action—including removal, throttling, suspension, or termination.

⸻

8) Third-Party Services & Integrations

The Service can interoperate with third parties you choose (e.g., Zoom, Microsoft Teams, Google Meet, Webex; identity providers like Apple, Google, GitHub, Slack, LINE, Yahoo Japan; avatar services like Gravatar). Your use of any third-party service is subject to that service’s terms and privacy policies. We do not control or assume responsibility for them.

If a third-party service becomes unavailable or changes functionality, the related feature in our Service may stop working or change. We are not liable for third-party downtime, data loss, or changes.

⸻

9) Privacy, Data, and Security
	•	Privacy Policy: Our separate Privacy Policy explains what we collect and why (e.g., emails, IP, country, ASN for abuse prevention; booking details; optional avatars), how we use it (e.g., to send confirmation/updates and protect the Service), and your choices.
	•	Gravatar: If enabled, we may compute a hash of a provided email to retrieve an avatar. You can customize or opt out by adjusting your account settings or using a different email.
	•	Security: We employ measures such as per-calendar key signing, device attestation, encrypted credentials, CAPTCHAs, passcodes for sensitive links, and abuse signals. No system is 100% secure—use strong device protections and safeguard secrets.
	•	Email Delivery: We send confirmations, updates (including ICS meeting updates), and limited reminders. Delivery depends on third-party mail systems and may be rate-limited.

⸻

10) Intellectual Property

The Service, including software, design, logos, mascots, and content we provide, is owned by the Company or its licensors and protected by law. Except for your own content and rights expressly granted to you, we reserve all rights. You may not copy, modify, reverse-engineer, or distribute our software except as allowed by law.

You retain rights in your content (calendar names/descriptions, branding you supply). By providing content through the Service, you grant us a non-exclusive, worldwide license to host, process, transmit, display, and otherwise use it solely to operate and improve the Service.

⸻

11) Feedback

If you send ideas or feedback, you grant us a royalty-free, perpetual license to use them without restriction or obligation.

⸻

12) Beta & Changes to the Service

Some features may be pre-release or beta. They might change, break, or be withdrawn. We may modify or discontinue the Service (or any part) at any time. When required by law or platform rules, we will provide notice.

⸻

13) Disclaimers

To the fullest extent permitted by law, the Service is provided “as is” and “as available.” We disclaim all warranties, express or implied, including merchantability, fitness for a particular purpose, and non-infringement. We do not warrant that the Service will be uninterrupted, error-free, secure, or that data will not be lost.

⸻

14) Limitation of Liability

To the fullest extent permitted by law:
	•	We are not liable for indirect, incidental, special, consequential, exemplary, or punitive damages, or lost profits, revenues, or data, even if advised of the possibility.
	•	Our total liability for any claim arising out of or relating to the Service is limited to the greater of (a) the amount you paid to us for the Service in the 12 months before the event giving rise to liability, or (b) JPY 10,000.

Some jurisdictions do not allow certain limitations—these limits apply to the maximum extent permitted.

⸻

15) Indemnification

You will defend, indemnify, and hold harmless the Company and its affiliates, officers, directors, employees, and agents from any claims, losses, liabilities, damages, costs, and expenses (including reasonable attorneys’ fees) arising from or related to: (a) your use of the Service; (b) your content; (c) your breach of these Terms; or (d) your violation of any law or third-party right.

⸻

16) Suspension & Termination

We may suspend or terminate your access if we believe you violated these Terms, pose a risk to the Service or others, or if required by law. You may stop using the Service at any time; for IAP subscriptions, manage cancellation through your Apple ID. Certain sections survive termination (e.g., IP, disclaimers, limitations, indemnity, governing law).

⸻

17) Export & Sanctions

You must comply with all applicable export control and sanctions laws. You may not use the Service if you are located in an embargoed country or are on a sanctions list.

⸻

18) Governing Law & Venue

These Terms are governed by the laws of Japan, without regard to its conflict of laws principles. You agree to the exclusive jurisdiction of the courts located in Kyoto, Japan for any disputes, unless another venue is required by mandatory law.

Optional alternative: Insert arbitration clause or your preferred jurisdiction here if different.

⸻

19) Changes to These Terms

We may update these Terms from time to time. If changes are material, we will provide notice as required (e.g., in-app notice or email). Your continued use of the Service after changes take effect constitutes acceptance.

⸻

20) Contact

Questions about these Terms can be sent to: legal or support email
Mailing address: Company address

⸻

21) Apple & Platform Terms (Additional)

When you download or use our iOS app/App Clip, you also agree to Apple’s applicable terms (including the App Store Terms and Licensed Application End User License Agreement). To the extent these Terms conflict with Apple’s mandatory terms, Apple’s terms control for the iOS distribution context.

⸻

22) Service-Specific Notes
	•	Email & ICS Updates: If a Host updates a Meeting Link, we may send an email update with an ICS REQUEST. Free-tier sending caps may apply. Delivery is best-effort.
	•	Abuse-Prevention Signals: We may process country/ASN indicators derived from network requests to detect fraud and enforce booking rules (e.g., country allow/deny lists).
	•	Security Controls: Booking details and cancel links can be protected by passcodes; Host management actions require signed requests and may require device attestation.
	•	Gravatar & Avatars: If enabled, we may derive a Gravatar using a hashed email. Bookers can customize their avatar; Hosts may display it to identify participants.
	•	Calendar Slug: Slugs are generated by the system and cannot be manually entered to avoid impersonation or namespace abuse.
	•	Integrations: Meeting provider integrations are optional and controlled by the Host. Availability or quality of third-party integrations is not guaranteed.

⸻

23) Entire Agreement; Miscellaneous

These Terms (and documents referenced, like the Privacy Policy) are the entire agreement between you and us regarding the Service and supersede all prior or contemporaneous agreements. If any provision is unenforceable, the remainder remains in effect. Our failure to enforce a provision is not a waiver. You may not assign these Terms without our consent; we may assign them as part of a merger, acquisition, or sale of assets.

⸻

Legal Notice & Disclaimer

This document is provided for general informational purposes and product fit; it is not legal advice. Laws vary by jurisdiction and product specifics. Please have a qualified attorney review and adapt this ToS for your circumstances (e.g., your exact company name, address, governing law, consumer disclosures, and App Store/IAP terms).


(Attached) Apple Standard EULA:
Apps made available through the App Store are licensed, not sold, to you. Your license to each App is subject to your prior acceptance of either this Licensed Application End User License Agreement (“Standard EULA”), or a custom end user license agreement between you and the Application Provider (“Custom EULA”), if one is provided. Your license to any Apple App under this Standard EULA or Custom EULA is granted by Apple, and your license to any Third Party App under this Standard EULA or Custom EULA is granted by the Application Provider of that Third Party App. Any App that is subject to this Standard EULA is referred to herein as the “Licensed Application.” The Application Provider or Apple as applicable (“Licensor”) reserves all rights in and to the Licensed Application not expressly granted to you under this Standard EULA.
a. Scope of License: Licensor grants to you a nontransferable license to use the Licensed Application on any Apple-branded products that you own or control and as permitted by the Usage Rules. The terms of this Standard EULA will govern any content, materials, or services accessible from or purchased within the Licensed Application as well as upgrades provided by Licensor that replace or supplement the original Licensed Application, unless such upgrade is accompanied by a Custom EULA. Except as provided in the Usage Rules, you may not distribute or make the Licensed Application available over a network where it could be used by multiple devices at the same time. You may not transfer, redistribute or sublicense the Licensed Application and, if you sell your Apple Device to a third party, you must remove the Licensed Application from the Apple Device before doing so. You may not copy (except as permitted by this license and the Usage Rules), reverse-engineer, disassemble, attempt to derive the source code of, modify, or create derivative works of the Licensed Application, any updates, or any part thereof (except as and only to the extent that any foregoing restriction is prohibited by applicable law or to the extent as may be permitted by the licensing terms governing use of any open-sourced components included with the Licensed Application).
b. Consent to Use of Data: You agree that Licensor may collect and use technical data and related information—including but not limited to technical information about your device, system and application software, and peripherals—that is gathered periodically to facilitate the provision of software updates, product support, and other services to you (if any) related to the Licensed Application. Licensor may use this information, as long as it is in a form that does not personally identify you, to improve its products or to provide services or technologies to you.
c. Termination. This Standard EULA is effective until terminated by you or Licensor. Your rights under this Standard EULA will terminate automatically if you fail to comply with any of its terms.
d. External Services. The Licensed Application may enable access to Licensor’s and/or third-party services and websites (collectively and individually, "External Services"). You agree to use the External Services at your sole risk. Licensor is not responsible for examining or evaluating the content or accuracy of any third-party External Services, and shall not be liable for any such third-party External Services. Data displayed by any Licensed Application or External Service, including but not limited to financial, medical and location information, is for general informational purposes only and is not guaranteed by Licensor or its agents. You will not use the External Services in any manner that is inconsistent with the terms of this Standard EULA or that infringes the intellectual property rights of Licensor or any third party. You agree not to use the External Services to harass, abuse, stalk, threaten or defame any person or entity, and that Licensor is not responsible for any such use. External Services may not be available in all languages or in your Home Country, and may not be appropriate or available for use in any particular location. To the extent you choose to use such External Services, you are solely responsible for compliance with any applicable laws. Licensor reserves the right to change, suspend, remove, disable or impose access restrictions or limits on any External Services at any time without notice or liability to you.
e. NO WARRANTY: YOU EXPRESSLY ACKNOWLEDGE AND AGREE THAT USE OF THE LICENSED APPLICATION IS AT YOUR SOLE RISK. TO THE MAXIMUM EXTENT PERMITTED BY APPLICABLE LAW, THE LICENSED APPLICATION AND ANY SERVICES PERFORMED OR PROVIDED BY THE LICENSED APPLICATION ARE PROVIDED "AS IS" AND “AS AVAILABLE,” WITH ALL FAULTS AND WITHOUT WARRANTY OF ANY KIND, AND LICENSOR HEREBY DISCLAIMS ALL WARRANTIES AND CONDITIONS WITH RESPECT TO THE LICENSED APPLICATION AND ANY SERVICES, EITHER EXPRESS, IMPLIED, OR STATUTORY, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES AND/OR CONDITIONS OF MERCHANTABILITY, OF SATISFACTORY QUALITY, OF FITNESS FOR A PARTICULAR PURPOSE, OF ACCURACY, OF QUIET ENJOYMENT, AND OF NONINFRINGEMENT OF THIRD-PARTY RIGHTS. NO ORAL OR WRITTEN INFORMATION OR ADVICE GIVEN BY LICENSOR OR ITS AUTHORIZED REPRESENTATIVE SHALL CREATE A WARRANTY. SHOULD THE LICENSED APPLICATION OR SERVICES PROVE DEFECTIVE, YOU ASSUME THE ENTIRE COST OF ALL NECESSARY SERVICING, REPAIR, OR CORRECTION. SOME JURISDICTIONS DO NOT ALLOW THE EXCLUSION OF IMPLIED WARRANTIES OR LIMITATIONS ON APPLICABLE STATUTORY RIGHTS OF A CONSUMER, SO THE ABOVE EXCLUSION AND LIMITATIONS MAY NOT APPLY TO YOU.
f. Limitation of Liability. TO THE EXTENT NOT PROHIBITED BY LAW, IN NO EVENT SHALL LICENSOR BE LIABLE FOR PERSONAL INJURY OR ANY INCIDENTAL, SPECIAL, INDIRECT, OR CONSEQUENTIAL DAMAGES WHATSOEVER, INCLUDING, WITHOUT LIMITATION, DAMAGES FOR LOSS OF PROFITS, LOSS OF DATA, BUSINESS INTERRUPTION, OR ANY OTHER COMMERCIAL DAMAGES OR LOSSES, ARISING OUT OF OR RELATED TO YOUR USE OF OR INABILITY TO USE THE LICENSED APPLICATION, HOWEVER CAUSED, REGARDLESS OF THE THEORY OF LIABILITY (CONTRACT, TORT, OR OTHERWISE) AND EVEN IF LICENSOR HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES. SOME JURISDICTIONS DO NOT ALLOW THE LIMITATION OF LIABILITY FOR PERSONAL INJURY, OR OF INCIDENTAL OR CONSEQUENTIAL DAMAGES, SO THIS LIMITATION MAY NOT APPLY TO YOU. In no event shall Licensor’s total liability to you for all damages (other than as may be required by applicable law in cases involving personal injury) exceed the amount of fifty dollars ($50.00). The foregoing limitations will apply even if the above stated remedy fails of its essential purpose.
g. You may not use or otherwise export or re-export the Licensed Application except as authorized by United States law and the laws of the jurisdiction in which the Licensed Application was obtained. In particular, but without limitation, the Licensed Application may not be exported or re-exported (a) into any U.S.-embargoed countries or (b) to anyone on the U.S. Treasury Department's Specially Designated Nationals List or the U.S. Department of Commerce Denied Persons List or Entity List. By using the Licensed Application, you represent and warrant that you are not located in any such country or on any such list. You also agree that you will not use these products for any purposes prohibited by United States law, including, without limitation, the development, design, manufacture, or production of nuclear, missile, or chemical or biological weapons.
h. The Licensed Application and related documentation are "Commercial Items", as that term is defined at 48 C.F.R. §2.101, consisting of "Commercial Computer Software" and "Commercial Computer Software Documentation", as such terms are used in 48 C.F.R. §12.212 or 48 C.F.R. §227.7202, as applicable. Consistent with 48 C.F.R. §12.212 or 48 C.F.R. §227.7202-1 through 227.7202-4, as applicable, the Commercial Computer Software and Commercial Computer Software Documentation are being licensed to U.S. Government end users (a) only as Commercial Items and (b) with only those rights as are granted to all other end users pursuant to the terms and conditions herein. Unpublished-rights reserved under the copyright laws of the United States.
i. Except to the extent expressly provided in the following paragraph, this Agreement and the relationship between you and Apple shall be governed by the laws of the State of California, excluding its conflicts of law provisions. You and Apple agree to submit to the personal and exclusive jurisdiction of the courts located within the county of Santa Clara, California, to resolve any dispute or claim arising from this Agreement. If (a) you are not a U.S. citizen; (b) you do not reside in the U.S.; (c) you are not accessing the Service from the U.S.; and (d) you are a citizen of one of the countries identified below, you hereby agree that any dispute or claim arising from this Agreement shall be governed by the applicable law set forth below, without regard to any conflict of law provisions, and you hereby irrevocably submit to the non-exclusive jurisdiction of the courts located in the state, province or country identified below whose law governs:
If you are a citizen of any European Union country or Switzerland, Norway or Iceland, the governing law and forum shall be the laws and courts of your usual place of residence.
Specifically excluded from application to this Agreement is that law known as the United Nations Convention on the International Sale of Goods.

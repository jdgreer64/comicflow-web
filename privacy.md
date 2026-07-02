---
title: Privacy Policy
layout: default
---

# ComicFlow Privacy Policy

**Effective date:** 2026-06-20
**Operator:** David Greer, doing business as Force Nebula (the "Operator", "we", "us")
**App:** ComicFlow for iOS ("the App")
**Contact:** support@forcenebula.com

This policy describes the personal information that ComicFlow collects, how we use it, who we share it with, and the rights you have over it. By using ComicFlow you agree to the practices described here.

## 1. Information we collect

### 1.1 Account information
When you sign in with **Apple**, we receive:

- Your Apple user identifier (an opaque string Apple provides). We use this as your account ID.
- Your email address, **only if you choose to share it** during Sign in with Apple. If you choose Apple's "Hide My Email" option, we never see your real email.
- A username you create the first time you sign in. We use it for display on community contributions (e.g. who contributed a cover).

We do **not** collect your real name, address, phone number, or social profile information.

### 1.2 Purchase and balance information
When you purchase In-App credit packs or a ComicFlow+ subscription:

- Apple processes the payment. We never receive your card number, billing address, or Apple ID password.
- Apple sends us a receipt token and the SKU you purchased.
- We record the credit balance and subscription state on our servers so the App can enforce the entitlements you purchased.

### 1.3 Library and collection data
Books you scan or import become entries in your collection. These entries can include:

- Series title, issue number, variant designation, publication year, publisher
- Grade, location, quantity, notes
- A photo of the cover (taken by you or imported from your photo library)
- Pricing data sourced from public marketplaces

This data is stored locally on your device. It is also sent to our servers **only if you opt in to sync, or if you choose to contribute a cover to the community library** (see Section 4).

### 1.4 Cover contributions (opt-in)
If you tap "Contribute to library" on a book, the cover photo and tuple (`series, issue, variant, year`) are uploaded to our server and stored alongside other users' contributions so all ComicFlow users can browse them. Cover contributions are linked to your account ID so we can show your stats and allow you to delete a contribution you made.

### 1.5 Automatic data
The App does **not** collect:

- Your location
- Your contacts, calendar, or photo library contents (beyond images you explicitly import)
- Cross-app tracking identifiers (IDFA)
- Crash dumps with personal content

We do log non-identifying technical events on the server side (request timestamp, endpoint, response code) for operational debugging. These logs are retained ≤30 days.

## 2. How we use information

We use the information described above to:

- Provide the App's core functions (identify books, look up prices, render your collection)
- Maintain your account, sessions, and credit balance
- Power optional features like sync and the community cover library
- Enforce purchases (verify you have credits, verify your subscription is active)
- Improve the App by identifying breakage patterns in non-identifying server logs

We do **not** use your data to build advertising profiles, sell to data brokers, or train machine learning models on your collection.

## 3. AI identification

When you photograph a book that the on-device identification path can't resolve, the App may send the photo to **xAI** (operator of the Grok vision API) for identification. This counts against your AI credit balance.

- The photo is sent through our server as a proxy; your Apple identifier travels with the request so we can deduct one credit on success.
- xAI's privacy practices apply to that submission. See [xAI's privacy notice](https://x.ai/legal/privacy-policy).
- We do not retain the photo on our server after the identification completes. We do log the request shape (size, response code) for cost monitoring.

You can disable AI fallback in **Settings → IDENTIFICATION → AI fallback**. With it off, no photos are sent to xAI.

## 4. Sharing with third parties

ComicFlow shares data with these third parties as part of providing the App's functions:

| Third party | What we send | Why |
|---|---|---|
| **Apple Inc.** | Sign in with Apple credential, IAP receipts | Authentication, payments |
| **RevenueCat, Inc.** | Apple subscription state, App User ID (your Apple identifier) | Subscription state tracking |
| **xAI Corp.** | A photo of a book you took, when AI fallback is on | AI book identification (Grok vision) |
| **eBay Inc.** | None directly — we read public sold-listing data | Price comp data |
| **Cloudflare, Inc.** | All server-bound requests including session tokens | Hosting our server (Workers + D1 database + R2 storage) |
| **Supabase, Inc.** | Cover library tuples + your contribution metadata | Database hosting for the community library |

We do not sell or share your data with any party for advertising or for any purpose not listed above.

## 5. Data retention

- **Session tokens:** 90 days, then automatically expired.
- **Account record:** Indefinite, until you delete your account.
- **Credit balance and purchase records:** Indefinite. Required for IAP compliance and for resolving billing disputes.
- **Community cover contributions:** Indefinite, until you delete the contribution or your account. When you delete a contribution, the cover image and your attribution are removed; the underlying book entry survives if other users have also contributed.
- **Server operational logs:** ≤30 days.

## 6. Your rights

- **Delete your account.** Settings → ACCOUNT → "Delete account…" permanently removes your account, all session tokens, all credits, and all community contributions you made. Subscription billing through Apple continues until your current period ends; cancel via the App Store before deleting if you want to stop billing.
- **Access your data.** Email support@forcenebula.com and we'll send a copy of all server-side records associated with your account within 30 days.
- **Correct your data.** Most data (username, collection entries) is editable in-app. For anything else, email support.
- **Opt out of AI fallback.** Settings → IDENTIFICATION → AI fallback off. No book photos are sent to xAI.
- **Opt out of cover contributions.** Don't tap "Contribute to library" on a book. You can also revoke past contributions from the admin / contributions view.

## 7. Children's privacy

ComicFlow is rated 12+ and is not directed at users under 13. We do not knowingly collect information from children under 13. If you believe a child under 13 has created an account, contact support@forcenebula.com and we will delete it.

## 8. Security

Account credentials are stored in your iOS Keychain. Server-side data is protected in transit by TLS and at rest by the storage providers' default encryption (Apple iCloud Keychain, Cloudflare D1 + R2, Supabase Postgres). No system is perfectly secure; we use industry-standard practices but cannot guarantee absolute security.

## 9. International use

ComicFlow is operated from the United States. By using the App you consent to your information being processed in the United States, which may have different privacy protections than your country of residence.

## 10. Changes to this policy

We will post material changes to this URL with an updated effective date. Continued use of the App after a change indicates acceptance.

## 11. Contact

Questions or requests about this policy:

**support@forcenebula.com**
David Greer, doing business as Force Nebula

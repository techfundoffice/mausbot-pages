---
layout: default
title: "Privacy Policy · MausBot"
description: "How the MausBot app, its iOS and Android companions and this website handle data: conversations stay on your computer, the hosted connection is optional."
permalink: "/privacy/"
---

Skip to content MausBot Get started Pricing Solutions Blog Partner 9.3k Get your team Get your 24/7 working team

Get started

FAQ

Pricing

Solutions

Enterprise

Blog

Community

Partner

Post about us

Discord

Theme

Privacy Policy

Last updated 18 October 2026

The short version: MausBot runs on your machine, and your conversations stay there. The phone app is a remote control for your own computer, not a service that holds your data. This website uses analytics, which you can switch off.

Who we are

MausBot is an open-source project published by Supamaus Software Private Limited. This policy covers the MausBot desktop app for macOS, Windows, and Linux, the MausBot companion apps for iOS and Android, and this website, openmausbot.com.

The companion apps are remote controls for an MausBot installation that you run and operate. Your bots, conversations, files, and credentials live on your own computer. We do not hold a copy of them.

This website: analytics and cookies

This section is about openmausbot.com only; the apps are covered below. We use two analytics services to understand which pages people read and how they found us:

Google Analytics 4, from Google, which sends the same page views to two Google Analytics properties we run.

PostHog, which records the pages you view and the links and buttons you click.

Both receive your IP address, browser and device details, the pages you visit, and the page that sent you here. We use them only to understand and improve this site. Neither receives what you type into the waitlist form. Both are US companies and may process this data in the United States; we use PostHog's US cloud.

Cookies and browser storage this site uses:

_ga and _ga_<property ID> (Google Analytics): tell repeat visits apart. Set only when analytics are on.

ph_<project key>_posthog (PostHog): tells repeat visits apart and holds the current session. Set only when analytics are on.

omb-analytics-consent (browser storage): remembers your analytics choice.

theme (browser storage): remembers light or dark mode.

Legal basis: if your browser's time zone is in Europe, including the UK, we ask before loading either service and load neither unless you accept; the basis is your consent. Elsewhere, analytics load by default, on the basis of our legitimate interest in understanding how the site is used. Wherever you are, you can switch them off here, and the choice is remembered in this browser:

Questions about the website or its analytics: omkar@supamaus.com .

MausBot Cloud launch waitlist

If you joined the waitlist on our website before MausBot Cloud launched, we stored your email address and the date you joined in our Cloud database so we could tell you when it launched. We also used hashed IP addresses to limit automated submissions. Joining did not create an account, start a subscription, or grant access to your app data.

We keep the waitlist only for that launch notification. You can ask us to remove your entry at any time by emailing omkar@supamaus.com. The email entered in the form was never sent to website analytics.

MausBox waitlist

If you join the MausBox waitlist at mausbot.com/mausbox, we keep the email address you enter, your name and what you would use MausBox for if you give them, the date you joined and the page you joined from. The entry is stored in our database, hosted by Upstash, and posted to a private Discord channel our team reads. Both may process it in the United States. To limit automated signups we count signups per connection for one hour, under a hashed form of your IP address.

We use the list only to write to you about MausBox: its specs, price and availability. Joining is free, does not create an account and does not commit you to buy. You can ask us to remove your entry at any time by emailing omkar@supamaus.com. Website analytics record only that someone joined and which use they picked, never the email or name.

What stays on your device

The companion app stores the address of the computer you selected, in the operating system's app preferences.

It stores the pairing token for that computer in the platform's encrypted credential store — the iOS Keychain, or the Android Keystore-backed encrypted store.

On iOS, the Share extension reads that same computer address and pairing token through a private App Group and a shared Keychain access group. No other app can read them.

Unpairing removes the address and the token from the phone.

Your computer remains the source of bots, transcripts, approvals, credentials, and screen images. Our hosted service does not store a copy of that content.

Permissions the apps ask for, and why

Camera — only to scan the pairing QR code shown by your computer. Nothing is recorded, stored, or uploaded; the frames are read for a code and discarded.

Microphone — only while you are speaking to a bot in voice or call mode, and only after you start it. Audio goes to the computer you paired with, and to the speech provider you configured there.

Notifications — to tell you when a bot replies, needs an approval, or finishes work.

Network and Wi-Fi state — to find your computer on the local network and to know when a connection has dropped.

Foreground service and battery optimisation — to hold the connection to your computer open while a session is running, so a reply is not lost when the screen turns off.

How your phone reaches your computer

On a local Wi-Fi network or over Tailscale, phone traffic goes directly to your computer, and nothing passes through us. Tailscale is a separate service with its own privacy terms. Plain local network connections should only be used on a network you trust.

If you enable the optional "use your phone anywhere" connection on the desktop, traffic is proxied by Cloudflare to an outbound-only connector on your computer. Messages, approvals, transcript responses, and screen frames pass through Cloudflare in transit, but are not written to our database. Cloudflare may process IP addresses and connection metadata as our service provider, under Cloudflare's own terms.

Neither route makes a sleeping or powered-off computer reachable.

What the optional hosted service stores

If, and only if, you sign in on the desktop to enable hosted access, we store: your account email address, an internal account ID, and metadata about the installation — an opaque installation ID, an opaque client ID, the computer's display name, operating system, app version, status, and security timestamps. We also store opaque Cloudflare tunnel and DNS resource IDs, and redacted operational errors.

Those records are used only to sign you in, establish ownership, prevent abuse, provision and revoke access, provide support, and keep the service reliable. Pairing tokens and device tokens are not stored in that database, and connector tokens stay in your desktop operating system's encrypted credential store.

Credentials you type on the phone

When you complete a credential request on your phone, the value exists in the secure text field only long enough to be encrypted with the public key pinned by that computer's pairing QR code, and the field is cleared immediately afterwards. Only your paired desktop app holds the private key. We receive ciphertext, never the value, and it is not written to phone preferences, the chat transcript, logs, or our database. Submission is available only over an encrypted connection, never plain local HTTP.

If you use a password manager to fill the field, that manager stores the value under its own settings and privacy terms.

Files and things you share

When you choose MausBot from another app's share sheet, or attach something in a chat, the text, link, image, or document you confirmed is sent to the bot you picked. Attachments are stored on your computer, with generated names and owner-only file permissions. Temporary copies made during a share are removed once the send completes or is cancelled.

Opening a file a bot sent you requests that exact file from your paired computer over the authenticated connection. The preview is kept on the phone only while it is open, then removed. Neither the file nor the preview is stored by our hosted service.

What we do not do

The desktop and companion apps contain no advertising SDKs and no third-party analytics SDKs. (This website does use analytics; see the website section above.)

The apps do not track you across other companies' apps or websites.

We do not sell or rent personal data, and we do not share it for advertising.

We do not read your conversations. They are on your computer.

Children

MausBot is a developer and productivity tool and is not directed at children. We do not knowingly collect personal information from children under 13, or under the minimum age set by local law.

Keeping, controlling, and deleting your data

Unpairing on the phone removes the stored computer address and pairing token from the device.

Revoking a phone in the desktop app's Companion settings invalidates that device's credential immediately.

Deleting the app removes its local data from the device.

Transcripts are deleted by the MausBot installation that stores them — that is, by you, on your computer.

Signing out of hosted access stops advertising the hosted address, revokes the installation credential, and schedules deletion of its Cloudflare tunnel and DNS record.

To request a copy of your hosted account data, or its deletion, email omkar@supamaus.com from the address on the account, or open a support request. Never include a one-time code, pairing code, device token, or any other secret in a public request. We will provide a private way to verify that you control the email address. Hosted account data is kept while it is needed to operate and protect the service, and otherwise until you ask us to delete it; a minimal record may be retained where security, fraud prevention, dispute resolution, or law requires it. Deleting hosted account data does not delete transcripts stored on your own computer.

Changes to this policy

If this policy changes in a way that materially affects how your data is handled, we will update the date at the top of this page and note the change in the app's release notes.

Contact

Supamaus Software Private Limited — privacy questions, data requests, and deletion requests: omkar@supamaus.com . You can also open a support request , without posting any secret in it. Company details are on the contact page .

MausBot

Your own team of AI bots, in a chat app. Free, open source, and running on your own machine.

Creators

Omkar Satpute

Milind Soni

Product

Download

Mac with Apple silicon

Mac with Intel

Windows

Ubuntu

Phone apps (Discord)

Scripted preview

Features

Ready-made bots

Cloud

Sign in to your Cloud plan

Become a partner

Project

Alternatives

GitHub

Docs

Contributing

Releases

Talk to us

Book a demo

Report an issue

Apache 2.0 License

Terms of Service

Refund Policy

No affiliation with any cryptocurrency. MausBot has no token. Any coin using the MausBot, Maus, or SupaMaus name is not created, endorsed, or affiliated with this project or its maintainer.

© 2026 NVIDIA, the NVIDIA logo, and NVIDIA Inception are trademarks and/or registered trademarks of NVIDIA Corporation in the U.S. and other countries. Google Cloud is a trademark of Google LLC. Claude is a trademark of Anthropic, PBC.

Apache 2.0 licensed · Built by the MausBot community

© 2026 Supamaus Software Private Limited . All rights reserved.

MAUS

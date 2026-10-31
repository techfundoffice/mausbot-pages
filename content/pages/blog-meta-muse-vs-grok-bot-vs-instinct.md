---
layout: default
title: "Meta Muse vs Grok Bot vs Instinct: which agent to pick"
description: "Meta Muse, xAI Grok Bot, and Instinct compared on price, region, models, approvals, and where the agent runs, plus the open-source option that works anywhere."
permalink: "/blog/meta-muse-vs-grok-bot-vs-instinct/"
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

← Blog

September 22, 2026 · Updated October 2, 2026 · 8 min read · Omkar Satpute and Milind Soni

Meta Muse vs Grok Bot vs Instinct: which agent to pick

Meta Muse, xAI Grok Bot, and Instinct compared on price, region, models, approvals, and where the agent runs, plus the open-source option that works anywhere.

Three cloud agents, three different bets. Meta Muse is one assistant on Meta's own model, US and Canada only, with a free tier and a card on file. xAI's Grok Bot is a roster of bots on one shared cloud computer, Grok only, from $20 a month with no free tier. Instinct is an invite-only assistant that holds your passwords and acts without asking. If you want more than one model, your data on your own machine, or you live outside the US, the open-source option at the end is the one that works today.

Meta Muse

Muse launched on September 8, 2026 from Meta Superintelligence Labs. It is one personal agent that runs on Meta's Muse Spark 1.3 model in a Linux VM in Meta's cloud, with a Chromium browser it can drive. You reach it from iOS, Android, the web, WhatsApp, and since September 17 a Mac app , though the Mac app does not run the agent locally; the cloud VM reaches into your Files, Mail, Messages, Calendar, and Notes by opt-in. It has connectors for Gmail, Calendar, Instagram, OpenTable, Ticketmaster, Spotify, Plaid, and Stripe Link checkout, and it can phone US businesses on your behalf. It is US and Canada only, 18 and over, and asks for a payment card at signup. The free tier is metered at roughly 100M tokens a week; Power is $20 a month on iOS and Maximum is $100. Meta's security post is candid: prompt injection is unsolved, Meta can access VM data today, and training on sanitized sessions is opt-out.

xAI Grok Bot

Grok Bot has been in beta since August 11, 2026. It is the closest of the three to a team: a messaging app with a roster of named bots, group chats of two to six bots with @mention, up to 50 routines per bot, skills, a bot marketplace, and a "Teach a task" feature that learns from a screen recording. Every bot runs Grok, chosen by a backend router, and every bot in your account shares one cloud computer ; xAI's docs say not to use separate bots as a security boundary. It ships on macOS, Windows, Linux, iPhone, iPad, and Android, with no web app and no public API. Since August 26 it is included with SuperGrok ($30) and Cursor Pro ($20) and up, with its own weekly allowance that xAI has not sized. The Hacker News thread and the Cursor forum are full of quota burn reports (one user hit 42% of a weekly allowance on day one) and a shared-computer outage in August that took every bot in an account down at once.

Instinct

Instinct from Spear Street Technology is the most hands-off of the three. You text it on iMessage or WhatsApp, or call it, and it works on a persistent cloud computer with your logins cached. You hand over passwords or a 1Password vault, and it acts without asking by default. The terms appoint it as your agent and grant a perpetual, sub-licensable licence over your materials, including screen captures, with a training opt-out that only applies going forward. It is invite only and free in beta, with invites paused mid-September for compute, after raising $350M at a $2.5B valuation on August 26. It gained its own email address on September 9 and outbound Concierge calls a week later. It is one thread, it is slow, it gets stopped by CAPTCHAs, and it has already sent an unapproved email, kept summarising a Gmail inbox three hours after access was revoked, and been prompt-injected through email.

Muse vs Grok Bot vs Instinct vs MausBot

The fourth column is MausBot, the open-source option covered below. Where a vendor has not published a figure, the cell says so.

Meta Muse Grok Bot Instinct MausBot

Price Free tier with a weekly token quota; Power $20/mo on iOS ($16 web); Maximum $100 ($80 web). Card required at signup. Included with SuperGrok ($30) or Cursor Pro ($20) and up. 7-day trial, no free tier. Weekly allowance not published. Free during beta. No price announced. Free. You pay your model providers directly.

License Proprietary. Open weights for the Spark model are on the roadmap, no date. Proprietary Proprietary Apache 2.0

Where you can use it United States and Canada only, 18+ No region list published Invite only. Invites paused mid-September for compute. Anywhere your Claude, Codex, or Grok login works

Models Muse Spark 1.3 only Grok only, routed on the backend. No model choice. Not published Claude, Codex, or Grok per bot; also Cursor, Kimi, Droid, OpenCode, Qwen, any ACP CLI, or an OpenAI-compatible endpoint

Where the agent runs A Linux VM in Meta's cloud. The Mac app reaches into your Mac from that VM. One shared cloud computer per account. Local command execution on macOS or Windows only when enabled under a policy. A persistent cloud computer with cached logins Your own machine, or a cloud desktop per bot

How it signs in to your accounts Opt-in connectors (Gmail, Calendar, Plaid, Stripe Link, and more) Logins on the shared cloud computer; users report them being shared across bots You hand over passwords or a 1Password vault OAuth once per app; scoped tokens on your disk; no passwords given to a bot

Approvals Scoped approvals; every purchase needs a human Local commands run only when enabled and approved under a policy. No audit log, per user reports. Acts without asking by default Allow / Deny card before every shell command, file edit, and question, with a decision log

How many agents One Muse, with hidden subagents A roster of named bots; group chats of 2 to 6 with @mention One thread Unlimited bots; group rooms with @mention and hand-offs

Connected apps Gmail, Calendar, Instagram, Facebook, WhatsApp, OpenTable, Ticketmaster, Spotify, Plaid, Stripe Link Apps on the shared cloud computer; skills; bot marketplace Its own email address; logins cached on its computer 500+ apps over Composio

Routines Goals and background tasks Up to 50 per bot Not published On a schedule or from a webhook

Keeps working with your laptop closed Yes Yes, on the cloud computer Yes Only for bots on a cloud computer

Phone calls Calls US businesses for you (beta) Live voice chat with you, rolling out on mobile You can call it; Concierge places outbound calls You can call a bot. Bots do not call third parties.

Platforms iOS, Android, web, WhatsApp, macOS. No Windows agent app. macOS, Windows, Linux, iPhone, iPad, Android. No web app. iMessage, WhatsApp, phone macOS, Windows, Ubuntu; iOS and Android companions

Training on your data On by default, opt-out Not covered in this review Perpetual, sub-licensable licence over your materials; opt-out applies going forward only Never. There is no server to train from.

Self-host or air-gap No No No Yes

Who each one is for

Meta Muse is for someone in the US who wants one assistant with zero setup and is fine with Meta holding the accounts it works in. It is one of two here that will phone a business for you (Instinct's Concierge does too, but its invites are paused), and it keeps working with your phone in your pocket. The cost is that it is one agent, one model, two countries, and the sessions train the model unless you opt out.

Grok Bot is for someone who already pays for SuperGrok or Cursor Pro and wants a team of bots without running anything themselves. Routines, group chats, and the marketplace are real and ahead of Muse. The trade-offs are Grok only, a weekly allowance nobody can size in advance, and one shared cloud computer that is a single point of failure for every bot you own.

Instinct is for someone who wants to text an assistant and never see a permission prompt, and who is comfortable giving a startup their passwords and a licence over their screen captures. Even if that is you, the invites are paused, so it is not a choice you can make this month.

MausBot is for someone who already has a Claude, Codex, or Grok login, wants more than one agent with more than one model, needs their data on their own disk, or lives somewhere Muse does not. It needs a download and a CLI login instead of a phone number, and it will not phone anyone for you.

The open-source option

MausBot is a free, Apache 2.0 desktop app with about 3,200 GitHub stars and no affiliation with xAI, Meta, or Spear Street. It looks like a Telegram-style chat app, and every contact is a bot with its own model, its own computer, its own connected apps, and its own memory. A small harness on 127.0.0.1 owns every agent process, and transcripts, keys, and events stay in ~/.openmausbot on your disk.

Your subscriptions, not theirs

Each bot runs on the claude , codex , or grok CLI installed on your machine, with the login you already have. The engine list also covers Cursor, Kimi, Droid, Antigravity, OpenCode, and Qwen, plus any ACP CLI or OpenAI-compatible endpoint, so a local model behind an Ollama-style endpoint works too. Pick a model per bot and switch mid-conversation.

Every contact in the sidebar is a bot with its own model, computer, and apps.

Every action is a card you answer

Muse gates purchases. Grok Bot gates local commands behind a policy. Instinct does not gate at all. MausBot puts a card in the chat before every shell command, file edit, and question, whether the bot is on your own machine or on a cloud desktop, and keeps a decision log you can read.

Allow, deny, or answer. Nothing runs because a web page told the bot to.

The rest is familiar from the other three: 500+ connected apps over Composio with OAuth once per app, routines on a schedule or webhook, group rooms where bots hand off work to each other, voice calls with a bot, and a cloud desktop per bot when you want one. What it does not do: phone a business, keep a local-machine bot working with the lid closed, or live inside WhatsApp. We compared it to each product in more depth in our Muse alternative , Grok Bot vs MausBot , and the Instinct alternative .

Frequently asked questions

Which one is cheapest? Instinct is free while it is in beta, but it is invite only and invites are paused. Muse has a free tier with a weekly token quota and asks for a card at signup. Grok Bot has no free tier: the floor is a $30 SuperGrok or $20 Cursor Pro plan, and its weekly allowance is not published. MausBot is free and open source; the only cost is whatever you already pay your model providers. Which one is available outside the US? Muse is US and Canada only as of October 2026. xAI has not published a region list for Grok Bot. Instinct is invite only. MausBot has no region check and runs anywhere your Claude, Codex, or Grok login works. Which one is open source? Only MausBot. Muse, Grok Bot, and Instinct are proprietary and run in their vendors' clouds. Meta has said open weights for the Muse Spark model are on its roadmap, with no date, and that would not make the agent itself open. Can I use my own Claude or Codex subscription? Only with MausBot. Muse is Muse Spark only, Grok Bot is Grok only, and Instinct does not publish which models it uses. MausBot runs each bot on the claude, codex, or grok CLI already installed on your machine, with the login you already have. Which one is safest? None of the four has solved prompt injection; Meta's own security post says so, and Instinct has had an injection incident via email. The differences are in the blast radius. Instinct holds your passwords and acts without asking. Grok Bot puts every bot on one shared cloud computer and tells you not to treat bots as a security boundary. Muse gates purchases and scopes permissions, but Meta can access VM data today. MausBot keeps everything on your disk and puts an Allow / Deny card in front of every command and file edit.

Download for macOS , Windows , or Ubuntu , sign in with the CLIs you already have, and meet your first bot. No card, no waitlist, no region check. The app is free; the pricing page covers Pro and Enterprise, and the source is on GitHub .

Read next

Muse vs Grok Bot vs Dots vs Cue: which agent to pick

Meta Muse, xAI Grok Bot, OpenAI dots, and Cue by Manus compared on price, region, models, approvals, and where the agent runs, plus the open-source fifth.

AI agent memory: who keeps it, and can you delete it?

Where OpenAI dots, Meta Muse, Grok Bot, Cue, Instinct, OpenClaw, Hermes, and Claude keep memory, whether you can delete one entry, and what trains the model.

Every open source AI agent app, compared (October 2026)

Sixteen open source agents, from OpenClaw and Hermes to the open-dot, OpenBot, OpenMuse and OpenInstinct clones, on licence, models, computer use and approvals.

Side by side

Instinct alternative: MausBot

An Instinct AI alternative you can download today: open source, signs into your apps over OAuth instead of holding passwords, and asks before it acts.

Every agent app, compared with MausBot

The hub: one page per rival, and a verdict.

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

Contact

Book a demo

Report an issue

Apache 2.0 License

Privacy Policy

Terms of Service

Refund Policy

No affiliation with any cryptocurrency. MausBot has no token. Any coin using the MausBot, Maus, or SupaMaus name is not created, endorsed, or affiliated with this project or its maintainer.

© 2026 NVIDIA, the NVIDIA logo, and NVIDIA Inception are trademarks and/or registered trademarks of NVIDIA Corporation in the U.S. and other countries. Google Cloud is a trademark of Google LLC. Claude is a trademark of Anthropic, PBC.

Apache 2.0 licensed · Built by the MausBot community

© 2026 Supamaus Software Private Limited . All rights reserved.

MAUS

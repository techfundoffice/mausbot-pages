---
layout: default
title: "Open Dots vs MausBot: the open source dots, compared"
description: "Three projects call themselves the open source OpenAI dots: Composio's open-dot, Anil Matcha's Open Dots, CopilotKit's OpenDots. Each vs MausBot, from GitHub."
permalink: "/alternatives/open-dots/"
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

← All alternatives

Facts checked October 8, 2026 · Composio, Anil Matcha, CopilotKit · open source

Open Dots vs MausBot

Three projects call themselves the open source OpenAI dots: Composio's open-dot, Anil Matcha's Open Dots, CopilotKit's OpenDots. Each vs MausBot, from GitHub.

Open Dots is three GitHub projects that appeared within a day of OpenAI's dots launch: Composio's open-dot, a Mac app with no licence and no commits since September 30; Anil Matcha's Open Dots, a renamed 2023 repo now a Telegram coding bot; and CopilotKit's OpenDots, a web template tied to CopilotKit's cloud. MausBot is the open source dots that is a finished app: bots on any model, Apache 2.0.

What Open Dots is

OpenAI launched dots on September 29, 2026 for ChatGPT Pro and Business Premium. Within 26 hours four repositories had taken the name. Composio's open-dot (600 stars) is an Electron app you build yourself for an Apple Silicon Mac, on an OpenAI or OpenRouter key, with Composio integrations, a per-dot Chrome profile and approval cards; it has four commits, all from September 29 and 30, and no licence file. Anil Matcha's Open Dots (5,517 stars) was created in May 2023 under another name, had its history replaced on October 7 and now describes itself as a Telegram and web front end for Claude Code running in Boat cloud sandboxes. CopilotKit's OpenDots (4,270 stars, MIT) is a web template whose conversations go through CopilotKit Intelligence, a hosted service outside the MIT licence.

Launched: September 29 and 30, 2026, all three within a day of OpenAI's dots . Sources: composio-community/open-dot on GitHub ; Anil-matcha/open-dots on GitHub ; CopilotKit/OpenDots on GitHub ; The Register: OpenAI dots inspire open source imitators .

Why people compare Open Dots with MausBot

None of the three is an app you can install: open-dot must be built from source on a Mac, Open Dots is a Docker stack plus a Telegram bot, and OpenDots is a web template.

Two of the three have no licence file as of October 8, 2026, which in law means all rights reserved, whatever the README says.

Composio's open-dot has had no commit since September 30; Anil Matcha's repo was force-replaced on October 7 and is now a different product from the one that launched.

CopilotKit's OpenDots cannot start without a CopilotKit Intelligence key, and the hosted setup sends conversations to CopilotKit's cloud with telemetry on by default.

One model vendor each: OpenAI or OpenRouter keys for open-dot, Claude via OAuth for Open Dots, OpenAI-compatible keys for OpenDots. No one lets a Claude bot and a Codex bot share a room.

The Open Dots column comes from the vendor's own pages and the press cited above, checked on October 8, 2026 . Where the vendor has not said, the cell says so.

Open Dots MausBot

License, stars open-dot: none, 600. Open Dots: none on disk, 5,517 on a 2023 repo. OpenDots: MIT, 4,270 Apache 2.0, about 4.2k

Shape A Mac app you build; a Telegram bot plus web UI; a web template A desktop chat app of bots; iOS and Android companions

Models OpenAI or OpenRouter keys; Claude by OAuth only; any OpenAI-compatible key Claude, Codex, Grok, and other CLIs, chosen per bot; switch mid-conversation

Before a shell command runs open-dot: rules plus a review model, cards in chat. Open Dots: a PermissionRequest hook, deny on timeout. OpenDots: approve-and-run cards for non-read-only tools Allow / Deny cards for shell commands and file edits; answer cards for questions

Agents open-dot: several dots with hand-off. Open Dots: one. OpenDots: one owner, group chat listed as further work As many bots as you like, in group rooms

Where it runs Your Mac; Boat cloud sandboxes at $20 a month after a trial; your server plus CopilotKit's cloud Your own machine; or a cloud desktop per bot

Platforms macOS arm64 only; anything with Docker; any Node 24 host macOS, Windows, Ubuntu; iOS and Android companions

Installers None of the three ships a binary Signed installers for macOS, Windows and Ubuntu; App Store and Play Store apps

Last commit September 30; October 7; October 6, 2026 Daily

What MausBot is

MausBot is a free, open-source chat app where every contact is an AI bot with its own model, its own computer, and its own connected apps. Bots run on the claude , codex , and grok CLIs installed on your own machine, with your existing logins, so one bot can be on Claude and the next on ChatGPT. Shell commands and file edits surface as Allow / Deny cards before they run, bots share group rooms and hand work to each other, and your data stays in ~/.openmausbot on your disk. It is published on GitHub under Apache 2.0, with iOS and Android companions, and paid Cloud plans from $15 a month keep bots working with the laptop closed.

What Open Dots still does better

open-dot: Composio's 1,500-app OAuth catalogue with event triggers, a Keychain-encrypted password vault that types credentials into the page, and voice calls, all in a very small readable codebase.

Open Dots: control of a Claude Code session from Telegram, with Allow once, Always allow and Deny buttons in the chat, on a Claude subscription rather than an API key.

OpenDots: WebRTC calls, Slack over the Channels SDK, and the largest community of the three, with 53 commits in the last 30 days.

Other Open Dots alternatives

The other open-source clones first, then the big agent apps, each with its own comparison page:

OpenBot by CopilotKit : OpenBot (6,182 stars, 841 forks, MIT) is the most-starred of the open source Grok Bot clones .

Rakazo by Inbox Zero Inc. (Elie Steinbock) : Rakazo (3,418 stars, 599 forks, Apache 2.0) was created two days after Grok Bot launched and is the closest of the clones to MausBot in shape: persistent bots with their own memory, routines and group channels, each on a model you choose through the Pi harness, including Claude Pro or Max and ChatGPT Plus or Pro sign-in, API keys, and Ollama .

OpenMuse by CopilotKit, nanoMuse and twelve smaller repos : Meta's Muse arrived on September 8, 2026 as a single proactive agent in a secure VM .

OpenInstinct by Merit Systems, Maria Gorskikh (Maritime) and others : Instinct opened its invite-only beta on August 26, 2026 and raised at a $10 billion valuation a month later .

Every other comparison page: Bops , Hark Pro , Grok Bot , Meta Muse , OpenAI dots , Cue by Manus , Instinct , OpenBot , Rakazo , OpenMuse , OpenInstinct , OpenClaw , Hermes Agent , Claude Cowork .

Frequently asked questions

Is there an open source OpenAI dots? Several projects claim the name. As of October 8, 2026, Composio's open-dot and Anil Matcha's Open Dots have no licence file, and CopilotKit's OpenDots is MIT but needs CopilotKit's hosted Intelligence service to run. MausBot is Apache 2.0, app and harness, and runs with no vendor service. What is open dot vs Open Dots vs OpenDots? open-dot is Composio's Mac app, launched by Karan Vaidya on September 30. Open Dots is Anil Matcha's repository, launched September 29. OpenDots is CopilotKit's web template, launched the same day. They share nothing but the name. Which Open Dots runs on Windows? Only Anil Matcha's, as a Docker stack with a Telegram bot; it has no desktop app. open-dot is macOS only and OpenDots is a web template. MausBot ships a native Windows installer. Does MausBot use any Open Dots code? No. MausBot started on August 11, 2026, seven weeks before dots, and is an independent codebase under Apache 2.0.

Read more

Open Dots vs MausBot: three open source dots, one app : the full comparison this page summarises.

OpenAI Dots alternative: free, open source, any model

Meta Muse vs OpenAI dots: the two one-agent products

Every open source AI agent app, compared (October 2026)

Meet your first bot

Free and open source. Connect one supported provider and start with a useful task. Provider fees and limits apply.

Download free Explore optional Cloud Installation help Discord support Report an issue

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

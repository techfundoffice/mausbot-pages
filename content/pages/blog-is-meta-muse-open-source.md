---
layout: default
title: "Is Meta Muse open source? No. Here is what is"
description: "Meta Muse is not open source: the app, the agent VM, and the Muse Spark model are all proprietary. Open weights have no date. Here is what is open instead."
permalink: "/blog/is-meta-muse-open-source/"
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

September 22, 2026 · 5 min read · Omkar Satpute and Milind Soni

Is Meta Muse open source? No. Here is what is

Meta Muse is not open source: the app, the agent VM, and the Muse Spark model are all proprietary. Open weights have no date. Here is what is open instead.

No. Meta Muse is not open source. The Muse app, the agent harness and the cloud VM it runs in, and the Muse Spark model are all proprietary. Meta has said open weights for the Spark model are "on the roadmap" with no date. Even if those weights ship, the Muse agent itself will still run only in Meta's cloud. If you want an agent you can read, run, and host yourself, the options are further down.

The three layers of Muse, and what is open

Muse launched on September 8, 2026, and the question "is it open source" has a different answer for each of the three things people mean by it.

The app. iOS, Android, web, WhatsApp, and since September 17 a Mac app . All closed. The Mac app is worth a second look because it sounds local and is not: the agent stays in Meta's cloud and reaches into your Files, Mail, Messages, Calendar, and Notes over an opt-in connection.

The agent harness and VM. Muse does its work in a Linux virtual machine in Meta's data centers, with a Chromium browser, a runtime cell, surrogate tokens for your credentials, and an egress authority Meta calls Sentinel. Meta's security post describes this design in detail, and none of it is published as code. The same post says Meta can access VM data today under its operational policy, with a "Confidential VM" planned for later.

The model. Muse runs on Muse Spark 1.3 , a proprietary model from Meta Superintelligence Labs. This is the only layer where Meta has said anything about openness: open weights are on the roadmap. No date has been given.

So the honest scorecard is: zero of three layers open today, one of three possibly open later, and the agent you actually use cloud only either way.

Where the confusion comes from

The Muse Spark 1.3 announcement is a research post. It names the model, describes it, and mentions that open weights are on the roadmap. Read quickly, or through a headline, that sounds like a release. It is not one. There is no published licence, no download, and no way to run Spark outside Muse, and Meta has given no date for when that changes.

The second source of confusion is the Mac app. A native app on your laptop that edits your files feels like software you run. In Muse's case the app is a window onto a cloud VM; close the lid and the agent keeps going in Meta's data center because it was never on your Mac. That is a feature if you want background work and a problem if you wanted your data to stay home.

What is open source in this category

Personal agents that do things for you, rather than frameworks you build with, are a young category, and most of the open projects in it are less than a year old. Here are the ones worth knowing, with what each is honest about.

OpenClaw (MIT, TypeScript, ~390k stars) is the biggest by far. A gateway daemon on your machine talks to WhatsApp, Telegram, Discord, Slack, Signal, iMessage, Teams, and 20-plus other channels, with a skills hub and MCP support, and it runs Claude, OpenAI via a ChatGPT subscription, DeepSeek, or Ollama. Version 2.0 on August 30 added a rebuilt Control Center with approvals, native apps with voice, and Computer Use on paired Macs and Windows PCs. The caveats are serious: The Register's review of 2.0 called it "not bringing security by default," the year opened with a CVSS 8.8 one-click RCE and more than 1,100 malicious skills on ClawHub, and the exec approvals default to full , meaning no prompt, on gateway hosts.

Hermes Agent from Nous Research (MIT, Python, ~248k stars, launched February 25, 2026) is a single self-improving assistant: it writes its own skills, keeps FTS5 memory, runs cron jobs and subagents, and speaks MCP. The "$5 VPS" positioning is real, and Hermes Desktop has been in public preview since June 2. It has Codex-style command approval. Users complain that its self-evaluation always reports success, that it overwrites hand-edited skills, and that it is one agent only.

NanoClaw (MIT, ~31k stars) takes the opposite approach to safety: no approval UI, but every chat runs inside its own Docker container on the Claude Agent SDK. macOS, Linux, and WSL2.

OpenWork (MIT, ~24k stars, from different-ai, a YC company) is an Electron desktop app built on OpenCode, positioned as a Claude Cowork clone for macOS, Windows, and Linux.

Rakazo (Apache 2.0, ~2.8k stars, by elie222) describes itself as an open-source Grok Bot alternative. It has been in beta since August 2026, deploys as a Docker Compose stack with Postgres, and runs agents in local Docker, E2B, Daytona, or Box sandboxes. No approval gate is documented.

MausBot (Apache 2.0, ~3.2k stars) is a desktop chat app where every contact is a bot with its own model, computer, connected apps, and memory. Bots run on the claude , codex , or grok CLI on your machine with your existing login, or on any OpenAI-compatible endpoint. A local harness on 127.0.0.1 owns every process and keeps everything in ~/.openmausbot . Every shell command, file edit, and question surfaces as an Allow / Deny card before it runs. It is one of the youngest and smallest projects on this list, and it does not phone businesses or live inside WhatsApp. The full comparison with Muse is in Meta Muse alternative: open source, runs on your machine .

In MausBot, the bot asks before it acts. The approval lands in the chat as a card.

Side by side

Project License Stars GUI Approval gate Platforms

OpenClaw MIT ~390k Control UI plus native apps; config-file heavy Ask mode exists; default is full (no prompt) on gateway hosts Gateway on macOS, Linux, Windows; apps for macOS, iOS, Android, Windows, Linux

Hermes Agent MIT ~248k Hermes Desktop, public preview Codex-style command approval Linux, macOS, WSL2, Windows (experimental), Termux

NanoClaw MIT ~31k Chat channels; no approve UI None; every chat runs in a Docker container instead macOS, Linux, WSL2

OpenWork MIT ~24k Electron desktop app Not covered in this review macOS, Windows, Linux

Rakazo Apache 2.0 ~2.8k Docker Compose stack with Postgres No approval gate documented Wherever Docker Compose runs; sandboxes on local Docker, E2B, Daytona, or Box

MausBot Apache 2.0 ~3.2k Desktop chat app Allow / Deny card before every command, file edit, and question macOS, Windows, Ubuntu; iOS and Android companions

Two distinctions matter more than the star counts. First, whether there is a per-action approval gate at all, and whether it is on by default: OpenClaw has one but ships with it off on gateway hosts, NanoClaw and Rakazo rely on sandboxes instead, Hermes and MausBot prompt. Second, where the agent runs: on your own machine, in a container you own, or in a cloud you rent. Muse is none of these; it is a cloud Meta owns.

Frequently asked questions

Can I self-host Meta Muse? No. Muse runs only in Meta's cloud, in a Linux VM Meta calls the Muse Secure VM. There is no download of the agent and no container image. The Mac app is a client for that cloud VM, not a local runtime. Is Muse Spark open source? Not today. Muse Spark 1.3 is a proprietary model that Meta serves from its own infrastructure. Meta has said that open weights are on the roadmap, without a date. If they ship, you would get model weights, not the Muse product; the harness, the VM, the connectors, and the app would still be Meta's and cloud only. Will Muse work with Ollama or a local model? No. Muse is Muse Spark only, with no model picker and no way to point it at a local endpoint. Of the open-source options here, OpenClaw and Hermes both support Ollama and local models, and MausBot accepts any OpenAI-compatible endpoint, which is how Ollama-style servers plug in. What is the closest open-source Muse? It depends on which part of Muse you want. For the messaging-app surface (WhatsApp, Telegram, iMessage), OpenClaw has the most channels and the most stars. For a single self-improving assistant on a cheap VPS, Hermes Agent. For a desktop app with a per-action approval gate, more than one agent, and your choice of Claude, Codex, or Grok, MausBot. We wrote up that last case in the open-source alternative to Meta Muse .

Try the open one

MausBot is free and runs on the CLIs you already have. Download for macOS , Windows , or Ubuntu , sign in with the CLIs you already have, and read the source on GitHub first if you like. No card, no waitlist, no region check.

Read next

OpenMuse vs MausBot: every open source Muse, compared

Fifteen GitHub repos call themselves OpenMuse. CopilotKit’s template and nanoMuse are the two that matter. What each is, and how the open source Muse compares.

Muse for Small Business vs a team of bots you own

What Meta's Muse for Small Business is, what it is not, the trust questions a business has to ask, and how the same five jobs run on a team of bots you own.

Meta Muse vs OpenAI dots: the two one-agent products

Meta Muse and OpenAI dots compared on price, region, model, where the agent runs, memory, training, and phone calls, plus the open-source third option.

Meta Muse alternative: MausBot

A Meta Muse alternative that is open source, works outside the US and Canada, and keeps your data off Meta's servers: a team of agents on your own machine.

OpenMuse vs MausBot

Fifteen GitHub repos call themselves OpenMuse. The two that matter, CopilotKit's template and nanoMuse, compared with MausBot on licence, models and approvals.

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

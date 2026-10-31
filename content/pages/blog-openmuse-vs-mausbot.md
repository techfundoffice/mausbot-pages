---
layout: default
title: "OpenMuse vs MausBot: every open source Muse, compared"
description: "Fifteen GitHub repos call themselves OpenMuse. CopilotKit’s template and nanoMuse are the two that matter. What each is, and how the open source Muse compares."
permalink: "/blog/openmuse-vs-mausbot/"
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

October 8, 2026 · 11 min read · Omkar Satpute and Milind Soni

OpenMuse vs MausBot: every open source Muse, compared

Fifteen GitHub repos call themselves OpenMuse. CopilotKit’s template and nanoMuse are the two that matter. What each is, and how the open source Muse compares.

OpenMuse is a name, not a project, and MausBot is the app. Fifteen GitHub repositories took the name after Meta launched Muse on September 8, 2026. Two matter. CopilotKit’s OpenMuse, 4,209 stars and MIT, is a phone-first template that needs CopilotKit’s hosted Intelligence service to run and cannot operate your own computer. nanoMuse, 267 stars and GPL, ships installers for five platforms and screen-driven hands, and calls itself a preview whose hands fail on grounding. Both are one agent. MausBot is the open source Muse alternative that is a team of bots on any model, on your own machine, Apache 2.0, with no vendor service.

What “open muse” means on GitHub

Meta’s Muse is a single proactive agent in a secure VM, on iOS, Android, muse.ai and since September 17 a Mac app, free for most use with $20 and $100 tiers, in the US and Canada only. Nat Friedman told TechCrunch it was “heavily inspired as a product by OpenClaw”, down to the workspace file names. The open-source response was immediate and scattered: a GitHub search for openmuse returns 138 repositories, of which fifteen position themselves as the open Muse. Here are the four with code worth reading, from their own repositories on October 8, and then the long tail.

OpenMuse, by CopilotKit

CopilotKit/openmuse launched on September 22 with a tweet seen 1.15 million times and was the number one TypeScript repository on GitHub the next day. It is a monorepo: an Expo app for iOS, Android and web, a Hono API with a task worker, a Playwright Chromium worker, and a nonroot Linux container with no network and a 30-second command limit, deployable to Render as three services. It has a durable task engine with signed receipts for every external write, a stored review before every send or calendar change, goals, page watches and “Ideas”. The README is candid: “Alpha, for self-hosting and building on”, demos use fictional data, and “every deployment requires CPK_INTELLIGENCE_API_KEY … Intelligence is a separate service and is not included in this repository’s MIT license”. An open issue asks to make that optional. Telemetry defaults to full capture. The agent reads pages in its own browser; another open issue asks for it to “click, type and fill forms on web pages”, and it has no way to touch the apps on your Mac or PC. No binaries are produced; it is API keys only. It is the best-engineered template in this group and a developer’s starting point.

nanoMuse

nano-muse/nanoMuse began life as OpenMuseAgent/OpenMuse and was renamed. It is the most product-like of the clones: forty releases since September 25 with an Android APK, a macOS DMG, a Windows EXE, Linux builds and TestFlight, all unsigned. Each device runs its own agent, an Alpine Linux under proot inside the phone app and DeepSeek Harness on the desktop, with screenshot-driven “hands” that operate apps on Android and on desktop screens, approvals that stop before deleting, sending or paying, Markdown memory files, routines that run while the app is closed, a morning feed, eighteen model providers plus Ollama and ChatGPT, Claude and Kimi plan sign-in, a free model allowance on a community relay, and no telemetry. Its Show HN on October 7 drew 56 points and 20 comments, mostly about the name and security, and there is an arXiv paper . The roadmap is equally candid: the 0.1 versions are a preview, the hands “fail on grounding” and on recovery after an unexpected dialog, memory is per device, and voice is input only. It is GPL-3.0, not Apache, which matters if you want to build on it.

Digger’s openmuse and chyroc’s open-muse

diggerhq/openmuse was first to the name on September 10: a web app over Digger’s own OpenComputer cloud, five commits in two days, a Show HN with one point, nothing since, and no licence. chyroc/open-muse is one developer’s 489 commits in ten days: an iPhone and Mac client for Volcano Engine’s Managed Agents service, with real Mac computer use behind an allow once, this chat or always ladder and app blocklists, Apple Health and Calendar, and no licence file, which means all rights reserved. The remaining eleven are a Manus API skin, a one-weekend build, an NVIDIA NIM hackathon entry, a security-runtime library with zero stars, and stubs.

OpenMuse vs MausBot, side by side

CopilotKit OpenMuse nanoMuse MausBot

Made by CopilotKit, a VC-backed company A team behind nanomuse.cn; main author Guangyi Liu Supamaus Software, an independent open-source project

Launched September 22, 2026 September 25, 2026 August 11, 2026

Stars, forks 4,209, 573 267, 28 About 4,200, 716

License MIT, but every deployment needs CopilotKit Intelligence, a separate service outside the licence GPL-3.0-or-later Apache 2.0, app and harness; no vendor service

Status Alpha, for self-hosting and building on; demos use fictional data 0.1.x preview, about three releases a day Shipping releases since August

Shape One agent: an Expo app for iOS, Android and web over a Hono server, a Playwright browser worker and a Linux container One agent per device: phone app, desktop app, web console and a relay, all in one repository A team of bots in a desktop chat app; iOS and Android companions

Installers None; build scripts do not produce signed app binaries Android APK, macOS DMG, Windows EXE, Linux AppImage and deb, TestFlight; unsigned Signed macOS, Windows and Ubuntu installers; App Store and Play Store apps

Models OpenAI, Anthropic or Google by API key; an OpenAI-compatible base URL; no plan sign-in Eighteen providers, Ollama and vLLM, or ChatGPT, Claude and Kimi plan sign-in; a free ¥10 relay allowance Claude, Codex, Grok and other CLIs, chosen per bot, on your existing logins

Controls your own computer No; its own browser and container only. An open issue asks for it to click and fill forms at all Yes, by screenshots, on Android and desktop; the roadmap says the hands fail on grounding Yes: the claude, codex and grok CLIs on your machine, plus a browser; or a cloud desktop per bot

Before it acts Every send or calendar change requires its own stored review; Take control hands you the browser A stop before deleting, sending or paying, remembered for once, this chat or always Allow / Deny cards for shell commands and file edits, by default

Memory Editable name, tone, avatar and memories SOUL.md, USER.md, MEMORY.md you can read and edit; per device, not yet synced Per bot, on your disk

Proactive Ideas, goals and page watches Goals on a schedule, routines while the app is closed, a morning feed Routines; always-on with a Cloud plan

Where it runs Your server, plus CopilotKit’s cloud for conversations Inside each device, with a relay in mainland China or one you host Your own machine, or a cloud desktop per bot

Telemetry Full capture to PostHog by default None; the community relay keeps request logs None sent

Voice Roadmap Input only; calls were removed in 0.1.22 In-app calls

Launch reception A tweet seen 1.15 million times; no HN thread Show HN, 56 points and 20 comments; an arXiv paper n/a

What MausBot is, in the same terms

MausBot is not a Muse clone; it is the other shape. Where Muse and every OpenMuse give you one assistant, MausBot is a chat app where every contact is a bot, each on the claude , codex or grok CLI installed on your own machine with the login you already have, so a Claude bot and a Codex bot share a room and hand work to each other. Shell commands and file edits surface as Allow / Deny cards before they run, by default. Data stays in ~/.openmausbot ; the harness listens on 127.0.0.1 only; nothing is sent to us. It installs from a signed DMG, EXE or deb, the iOS and Android apps are in the stores, and it is on GitHub under Apache 2.0, app and harness. Cloud plans from $15 a month keep bots working with the laptop closed. There is no region list.

What the OpenMuse projects still do better

CopilotKit OpenMuse has a phone-native UI with rich cards for email, browser previews, PDFs and plans; a durable task engine with signed receipts for every external write; and the largest community of the group, with 105 merged pull requests in three weeks.

nanoMuse drives the apps on an Android phone’s screen, which MausBot’s phone apps do not do; routes approvals to whichever device is in your hand; supports eighteen providers; and needs no key for a first run.

chyroc’s Open Muse operates your Mac apps by screen with per-app blocklists and reads Apple Health, and offers a Quick Chat overlay over any app.

All of them are proactive by design, with goals, ideas and a morning feed; MausBot’s routines are a schedule you set.

The verdict

An open-source Muse has to clear three bars: a licence that lets you use it, a build you can install, and an agent that can act on your computer under your control. CopilotKit’s clears the first on paper and fails the second and third, and adds a vendor service the licence does not cover. nanoMuse clears the second, half-clears the third by its own account, and is GPL and a preview. Two others have no licence at all. MausBot clears all three, and adds the thing none of them has: more than one agent, on more than one model, in one room. Measured against Muse itself, MausBot is also the only option here with no region list and no usage tiers. For the searcher typing “open muse”, it is the one to install.

Frequently asked questions

Is there an open source Meta Muse? Several projects claim it and Meta has not released one. CopilotKit’s OpenMuse is MIT but depends on CopilotKit’s hosted Intelligence service in every mode; nanoMuse is GPL-3.0 and fully self-hostable; Digger’s and chyroc’s open-muse have no licence file at all. MausBot is Apache 2.0, app and harness, and runs with no vendor service. Which OpenMuse is the real one? None is official. CopilotKit’s is the most-starred, nanoMuse ships the most installers, and twelve smaller repositories use the name, several of them one-day builds. Unrelated projects called OpenMuse cover a text-to-image model, an EEG headband, a MuseNet reimplementation and a music downloader, and two more target Muse Code, Meta’s coding CLI. Does OpenMuse control my computer like Muse’s Mac app? CopilotKit’s does not: it drives its own browser and a no-network Linux container on your server, and an open issue asks for it to click and fill forms at all. nanoMuse and chyroc’s Open Muse do, by screenshots, on desktop. MausBot bots run the Claude, Codex and Grok CLIs on your own machine, so file edits and shell commands happen where you sit, behind an approval card. Can I run OpenMuse on my ChatGPT or Claude plan? nanoMuse can, by plan sign-in. CopilotKit’s OpenMuse takes API keys only. MausBot runs bots on the claude and codex CLIs with your existing logins. Is OpenMuse available outside the US? Yes, all of them, which is one reason people look: Muse itself is US and Canada only. nanoMuse defaults to Chinese providers and a relay in mainland China, with your own key or self-hosted relay as the alternative. MausBot has no region list.

Read next

OpenMuse vs MausBot , the one-page summary.

The open source alternative to Meta Muse , MausBot against Muse itself.

Is Meta Muse open source?

Muse for Small Business vs a team of bots you own

What Meta's Muse for Small Business is, what it is not, the trust questions a business has to ask, and how the same five jobs run on a team of bots you own.

Meta Muse vs OpenAI dots: the two one-agent products

Meta Muse and OpenAI dots compared on price, region, model, where the agent runs, memory, training, and phone calls, plus the open-source third option.

Muse vs Grok Bot vs Dots vs Cue: which agent to pick

Meta Muse, xAI Grok Bot, OpenAI dots, and Cue by Manus compared on price, region, models, approvals, and where the agent runs, plus the open-source fifth.

Side by side

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

---
layout: default
title: "Every open source AI agent app, compared (October 2026)"
description: "Sixteen open source agents, from OpenClaw and Hermes to the open-dot, OpenBot, OpenMuse and OpenInstinct clones, on licence, models, computer use and approvals."
permalink: "/blog/open-source-ai-agent-apps-compared/"
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

October 8, 2026 · 14 min read · Omkar Satpute and Milind Soni

Every open source AI agent app, compared (October 2026)

Sixteen open source agents, from OpenClaw and Hermes to the open-dot, OpenBot, OpenMuse and OpenInstinct clones, on licence, models, computer use and approvals.

Sixteen open source AI agents, one table, one verdict. The field in October 2026 splits three ways: the self-hosted giants (OpenClaw, Hermes, Paperclip, LobeHub), the desktop agents with real installers (goose, Eigent, QwenPaw, Agent Zero), and the “open X” clones that appeared within days of each closed launch (OpenBot, Open Dots, OpenMuse, OpenInstinct, Rakazo). Judged on licence, models, where the agent runs, what happens before a command, and whether you can install it, MausBot is the only one that is Apache 2.0 with no vendor service, a team of bots on any model including the plan you already pay for, gated by default, and shipped as signed installers with store phone apps.

How to read the table

Every star count is from the GitHub API on October 8, 2026. Every other cell is from the project’s own README, docs or licence file on that date, or from the per-project page linked in the first column, each of which cites its sources and says what that project does better than MausBot. “Gate by default” is the one column people skip and should not: it says what happens before a shell command or an external write on a fresh install, before you have read the docs. Where a project does not document a gate, the cell says so rather than guessing.

Project Stars License Shape Models Its computer Gate by default Team of agents Install

MausBot 4.2k Apache 2.0 Desktop chat app of bots; iOS and Android Claude, Codex, Grok CLIs on your plan; any OpenAI-compatible endpoint Your machine, or a cloud desktop per bot Allow / Deny card, on by default Yes, in rooms Signed installers; store apps

OpenClaw 392k MIT Gateway daemon reached through chat apps; Control UI Claude, OpenAI, DeepSeek, Ollama The host it runs on None by default on gateway hosts (exec mode full) One gateway, many channels Install script; native apps

Hermes Agent 252k MIT One always-on agent through chat apps; Hermes Desktop Nous Portal, OpenAI, Anthropic, local A server, a VPS, or your PC Smart, manual or off; --yolo skips it Profiles, not a room Install script; desktop preview

Paperclip 98.5k MIT Node server and web UI; an org chart of agents Any CLI agent as an adapter: Claude Code, Codex, OpenClaw, Hermes The host, or sandbox providers Allowed, Ask first or Off per gateway action; budgets Yes, with reporting lines; chat is experimental npx; no binary

LobeHub 83k LobeHub Community License (Apache 2.0 plus conditions) Web, Electron desktop, iOS and Android API keys; wraps Claude Code and Codex as agents Their cloud for 24/7 runs; no local computer use found Approve tasks by reply in a Daily Brief Agent Groups Installers; store apps

Open Interpreter 68.5k Apache 2.0 Rust terminal agent, a Codex fork Low-cost models by key Native sandboxing on your machine Sandbox and approvals No Binary

goose 55k Apache 2.0 Native desktop and CLI, Linux Foundation 15+ providers; Claude Code and ChatGPT plans via ACP Your machine Autonomous, Manual, Smart Approval or Chat Only No Installers for Mac, Windows, Linux

QwenPaw 35.5k Apache 2.0 Local console, TUI, Tauri desktop; chat channels Its own 2B to 9B agent models, no key; Ollama; 14+ clouds Local or cloud; browser and computer use allow, deny, ask or sandbox; dangerous commands blocked Sub-agents pip; desktop zip and exe

Kortix (Suna) 20.3k Elastic License 2.0 (source-available) Self-hosted web, desktop, CLI; Slack and Teams API keys, or a ChatGPT plan A cloud sandbox per session; no local mode Allow, Ask or Block per tool argument; off until set Thousands in parallel; merge gate Docker Compose; desktop installers

Agent Zero 19.4k MIT Docker image with a Linux desktop; web UI; launcher Any provider; Codex plan by OAuth; local An XFCE desktop in the container; your browser by bridge Intervene with your mouse; no per-action gate documented Subordinate agents docker run; launcher app

Eigent 15.5k Apache 2.0 Electron desktop with a local backend Any key; vLLM, Ollama, LM Studio Your machine: browser and terminal toolkits Optional human in the loop A parallel workforce on one task Installers for Mac, Windows, Linux

OpenBot (CopilotKit) 6.2k MIT, plus a required CopilotKit Intelligence account Self-hosted web app for a company’s coworkers API keys; any AG-UI agent A container with Chromium and a shell per bot CEL policy at the gateway; shipped policy permissive Group chats, delegation Container images only

Open Dots (three repos) 0.6k, 5.5k, 4.3k None, none on disk, MIT A Mac app you build; a Telegram bot; a web template OpenAI or OpenRouter keys; Claude by OAuth; any key Your Mac; Boat cloud; CopilotKit containers Review model and rules; permission hook; approve-and-run cards Hand-off; no; further work None

OpenMuse (CopilotKit) 4.2k MIT, plus a required CopilotKit Intelligence key Expo phone app over your server OpenAI, Anthropic, Google keys Its own browser and container; not your computer Stored review for every external write No None

Rakazo 3.4k Apache 2.0 Self-hosted API with web, Electron and Expo clients Claude, ChatGPT, SuperGrok, Copilot plans; keys; Ollama Docker desktop per bot; E2B, Daytona, Box, or your Mac Approval rules per bot; audit log Yes, with group channels Mac DMG, Linux AppImage; no Windows

OpenInstinct (Merit) 0.4k MIT Vercel service you text on iMessage Any model through Vercel AI Gateway A Kernel cloud browser Prompt-level; Stripe Link for money No Deploy to Vercel Pro

nanoMuse 0.3k GPL-3.0 An agent per device: phone, desktop, relay 18 providers; Ollama; ChatGPT, Claude, Kimi plans Screen-driven hands on Android and desktop, a preview A stop before deleting, sending or paying One per device APK, DMG, EXE, Linux; unsigned

open-instinct (Gorskikh) 0.2k MIT Node service; a microVM per person on Maritime Claude default; any Pi provider incl. Ollama A Firecracker microVM desktop Policy guard before every tool; six trust tiers One per person; talks to friends’ agents CLI; beta

The self-hosted giants

OpenClaw (392,000 stars) and Hermes Agent (252,000) are the projects everyone else is measured against, including Meta, whose Muse borrowed OpenClaw’s workspace files by its own admission. Both are gateways you run on a server and reach through WhatsApp, Telegram or Discord, both support every model including local ones, and both put the safety decision on you: OpenClaw’s exec approvals default to full on gateway hosts, Hermes ships a yolo flag, and both have 2026 CVE lists. Paperclip (98,500 stars) is the biggest team-of-agents project of the year, an org chart with budgets and reporting lines that hires any CLI agent as an employee, and it is a task manager, not a chat app. LobeHub (83,000) is the closest in shape to MausBot, with Agent Groups, a chat-network gateway and store phone apps, under a licence that is Apache 2.0 with commercial conditions, and with its 24/7 runs on its own cloud.

The desktop agents with installers

goose (55,000 stars, Linux Foundation) is the most mature single agent on the desktop, with Claude Code and ChatGPT plan reuse over ACP and four permission modes; it has no roster and no phone. Eigent (15,500, Apache 2.0) runs a parallel workforce on one task, with local models first-class and no subscription reuse. QwenPaw (35,500) needs no API key at all, because it ships its own small agent models, and reaches you through seven chat apps, DingTalk and WeChat first. Agent Zero (19,400) gives every instance a full Linux desktop in Docker and lets you share the mouse, and relies on that isolation rather than a per-action gate. Open Interpreter (68,500) is now a Rust fork of Codex for cheap models, a coding agent in a terminal. All five are products with releases; none is a team of named bots in a chat.

The “open X” clones

The pattern of 2026 is that a closed agent launches on Monday and four repositories named after it exist by Tuesday. We checked each family on its own page:

OpenBot , CopilotKit’s Grok Bot for companies: the most-starred clone, MIT, policy and SSO, a template that needs a CopilotKit account to start and ships no installer.

Rakazo , Inbox Zero’s Grok Bot: Apache 2.0, the widest model menu, a server with Docker desktops per bot, no Windows build, a hosted waitlist.

Open Dots , three unrelated repositories: a Mac app with no licence and no commits since September 30, a renamed 2023 repo rebuilt as a Telegram coding bot, and a CopilotKit web template.

OpenMuse , fifteen repositories: CopilotKit’s phone-first template that cannot touch your computer, and nanoMuse, which ships installers and screen-driven hands as a preview under GPL.

OpenInstinct , two iMessage agents you deploy to Vercel or Maritime, one marked not for production and one five days old; and no open Cue at all.

What the clones share: one agent, one vendor or one gateway, a service to deploy rather than an app to open, and, in four cases, no licence file. What they do better than MausBot is listed on each page, and some of it is real: OpenBot’s policy engine, Rakazo’s provider matrix, nanoMuse’s phone-screen hands, open-instinct’s agent-to-agent protocol.

Where MausBot sits

MausBot started on August 11, 2026 as the open source Grok Bot and has been committed to daily since. It is a chat app where every contact is a bot, each on the claude , codex or grok CLI installed on your own machine with your existing login, which is why the models column reads “on your plan”: a bot costs nothing beyond the subscription you have. Bots share rooms and hand work to each other, run routines, connect to 500+ apps over Composio, and get a cloud desktop each when you want one. Shell commands and file edits become Allow / Deny cards before they run, by default, for every engine, which is a gate in code rather than a mode you remember to switch on. Data stays in ~/.openmausbot ; the harness listens on 127.0.0.1 only; there is no account, no telemetry and no vendor service in the path. It installs from a signed DMG, EXE or deb, the iOS and Android apps are in the stores with Live calls, Hermes can run inside it as an engine, and the code is on GitHub under Apache 2.0, app and harness. Cloud plans from $15 a month add always-on bots for the laptop-closed case.

The verdict

Run down the columns. Licence: eleven of the sixteen are MIT or Apache with no strings; the CopilotKit templates need a hosted service, Kortix and LobeHub carry conditions, four clones have no licence. Models on the plan you already pay for: seven, and among them only MausBot, Rakazo and LobeHub are a team of agents. A gate on by default: MausBot, goose, QwenPaw and the Instinct clones; the giants default to open. An app you install with a phone app in the stores: MausBot, LobeHub and Kortix. Put the four columns together and one row has every box ticked. The giants are more popular; the desktops are older; several clones are clever. MausBot is the one that is open source without a vendor in the path, runs any model on your own plan, puts a team of bots in a room, asks before every command, and installs in a minute on Mac, Windows, Ubuntu, iPhone and Android. On the evidence in this table, it is the best open source AI agent app you can run today. Each rival page says what we would borrow from them; this page says why we would still pick ours.

Frequently asked questions

What is the best open source AI agent app? For a person who wants an app: MausBot, the only project in the table that is Apache 2.0 with no vendor service, a team of agents on any model including the Claude, ChatGPT or Grok plan you already pay for, an approval card on by default, signed installers and store phone apps. For a company that wants policy and SSO: OpenBot or Kortix. For a tinkerer who wants the biggest community: OpenClaw or Hermes. Which open source agents can use my ChatGPT or Claude subscription instead of an API key? MausBot (through the claude, codex and grok CLIs), goose (through ACP), Rakazo (through Pi), nanoMuse (plan sign-in), Kortix (a ChatGPT plan), Agent Zero (a Codex plan by OAuth), and Anil Matcha’s Open Dots (Claude by OAuth). OpenClaw routes OpenAI through a ChatGPT subscription too. The CopilotKit templates, Eigent, OpenInstinct and Open Interpreter take keys. Which ones ask before running a shell command, by default? MausBot shows an Allow / Deny card by default for every engine. goose and QwenPaw ship approval modes you pick at setup. OpenClaw’s exec mode defaults to full on gateway hosts; Hermes has a --yolo flag; Kortix’s gates are off until you set them; nightly-labs/openbot runs with an approval policy of never. The CopilotKit templates review external writes but the shipped OpenBot policy allows everything until you write rules. Which “open X” projects are really open source? By licence file on October 8, 2026: OpenBot, CopilotKit OpenDots and OpenMuse, both OpenInstincts and Rakazo are MIT or Apache; nanoMuse is GPL. Composio’s open-dot, Digger’s openmuse and chyroc’s open-muse have no licence file, and Anil Matcha’s Open Dots lost its licence file in an October 7 rewrite. The CopilotKit templates are MIT but cannot start without CopilotKit’s hosted Intelligence service. Why does this page say MausBot wins? Because we wrote it, and because the table supports it. Each rival page on this site lists what that project does better than MausBot, and this page links to them. The claim is narrow: among open source agent apps a person can install today, MausBot is the one that clears every bar at once.

Read next

Every agent app compared with MausBot , the hub, with the closed products too.

The best self-hosted AI agents , the earlier round-up of OpenClaw, Hermes and friends.

Which AI agent should I use? , five questions to decide.

AI agent memory: who keeps it, and can you delete it?

Where OpenAI dots, Meta Muse, Grok Bot, Cue, Instinct, OpenClaw, Hermes, and Claude keep memory, whether you can delete one entry, and what trains the model.

Meta Muse vs Grok Bot vs Instinct: which agent to pick

Meta Muse, xAI Grok Bot, and Instinct compared on price, region, models, approvals, and where the agent runs, plus the open-source option that works anywhere.

OpenMuse vs MausBot: every open source Muse, compared

Fifteen GitHub repos call themselves OpenMuse. CopilotKit’s template and nanoMuse are the two that matter. What each is, and how the open source Muse compares.

Side by side

Open Dots vs MausBot

Three projects call themselves the open source OpenAI dots: Composio's open-dot, Anil Matcha's Open Dots, CopilotKit's OpenDots. Each vs MausBot, from GitHub.

OpenBot vs MausBot

OpenBot is CopilotKit's MIT template of AI coworkers for companies, and needs a CopilotKit account to start. MausBot is the open source Grok Bot for a person.

OpenMuse vs MausBot

Fifteen GitHub repos call themselves OpenMuse. The two that matter, CopilotKit's template and nanoMuse, compared with MausBot on licence, models and approvals.

OpenInstinct vs MausBot

Two serious OpenInstinct projects: Merit Systems' Vercel template and Maria Gorskikh's Maritime agent. Both are iMessage agents you deploy. MausBot is an app.

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

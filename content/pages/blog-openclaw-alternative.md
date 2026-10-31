---
layout: default
title: "OpenClaw alternative with an approval gate built in"
description: "An OpenClaw alternative that asks before every shell command, ships as a desktop app for Mac, Windows, and Ubuntu, and uses the Claude or Codex login you have."
permalink: "/blog/openclaw-alternative/"
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

September 22, 2026 · Updated September 29, 2026 · 9 min read · Omkar Satpute and Milind Soni

OpenClaw alternative with an approval gate built in

An OpenClaw alternative that asks before every shell command, ships as a desktop app for Mac, Windows, and Ubuntu, and uses the Claude or Codex login you have.

MausBot is an OpenClaw alternative with an approval gate on by default. OpenClaw is a gateway you run from the terminal and reach over WhatsApp or Telegram; out of the box it runs shell commands without asking. MausBot is a desktop chat app where every bot asks with an Allow / Deny card before it runs a command or edits a file. It is free, Apache 2.0 licensed, and works on the Claude, Codex, or Grok login you already have.

What OpenClaw is

OpenClaw is the most-starred self-hosted AI agent on GitHub, at roughly 390,000 stars. It started as Clawdbot in November 2025, became Moltbot on January 27, 2026, and took its current name three days later. It is the project that proved people want an agent that lives in their chat apps and does things on their machines.

A gateway daemon on port 18789 connects to 20+ channels: WhatsApp, Telegram, Discord, Slack, Signal, iMessage, Teams, and more.

Skills come from ClawHub, tools come over MCP, and models include Claude, OpenAI via a ChatGPT subscription, DeepSeek, and local models through Ollama.

MIT licensed, written in TypeScript, installed with a curl script or npm on Node 24.16 or newer.

v2.0 shipped on August 30, 2026 with a rebuilt Control Center that includes approvals, session permission modes, plugin trust review, memory recall, a Skill Workshop, and Computer Use on paired Macs and Windows machines.

The creator, Peter Steinberger, joined OpenAI in February 2026 , and the project now sits under the OpenClaw Foundation with OpenAI, NVIDIA, Microsoft, and Tencent as sponsors. It is not going anywhere. If you are comfortable at a terminal and you run it well, it is a lot of agent for free.

Why people look for an OpenClaw alternative

Four reasons, in the order they come up.

1. The security history

No other agent project has a timeline like this one.

February 1, 2026. Koi Security published ClawHavoc : 341 malicious skills on ClawHub, later revised to 1,184, shipping macOS credential stealers to people who installed them.

February 9 and 18, 2026. Scans found 135,000 OpenClaw gateways exposed to the internet, then more than 312,000 hosts answering on port 18789. Flare put the number of compromised instances above 30,000.

CVE-2026-25253. A CVSS 8.8 one-click remote code execution bug through the Control UI's gatewayUrl parameter, with around 17,500 exposed instances counted by runZero . CVE-2026-32922, a privilege escalation, followed.

Prompt injection. Giskard showed that any member of a group chat can chain tool calls through the bot. The MoltMatch incident made the same point in public.

Defaults. OpenClaw has an exec approval system with deny, allowlist, ask, auto, and full modes. The default on gateway hosts is full , which means no prompt. After v2.0, The Register wrote that the release was "not bringing security by default": secrets are unencrypted at rest and the sandbox is not enabled automatically.

2. Setup and operations

The Windows install script, gateway restarts, and config drift between machines are the recurring threads. OpenClaw is a daemon you operate, not an app you open.

3. Token cost

A heartbeat cron job that burned $20 overnight is the story people repeat. Heavy users report three to five million tokens a day. An always-on agent that polls is an always-on bill.

4. It is built for operators

A maintainer put it plainly: "if you can't understand how to run a command line, this is far too dangerous." That is honest, and it is the reason a lot of people search for something else.

What to look for in an OpenClaw alternative

A real GUI. Not a browser page bolted onto a daemon. Something you install and open.

Approval before action, by default. The gate should be the thing you have to turn off, not the thing you have to find.

OAuth, not passwords. An agent that holds scoped tokens on your disk is a smaller blast radius than one that holds your logins.

Local first. Transcripts and keys on your machine, a harness that listens on localhost, no gateway to expose by accident.

Your existing subscriptions. If you already pay for Claude or ChatGPT, the agent should use that login rather than a new API bill.

MausBot: the approval gate is the product

MausBot is a chat app, Telegram in shape, where every contact is an AI bot. Each bot runs on the claude , codex , or grok CLI installed on your machine with your existing login. A small harness on 127.0.0.1 owns every agent process and everything it produces lives in ~/.openmausbot . The code is on GitHub under Apache 2.0.

Every risky action is a card

Shell commands, file edits, and questions surface in the chat as cards. Allow, deny, or type an answer. The action does not run until you decide, whether the bot is on your own machine or on a cloud desktop, and every decision lands in a log you can read. This is the exact opposite of OpenClaw's full default.

No shell command or file edit runs because a web page or a group member told the bot to. You decide first.

An app, not a gateway

Download, sign in with the CLIs you already have, and meet your first bot. There is no daemon to keep alive, no port 18789, and no config file to hand-edit. Bots can go into group rooms, ask each other questions, and hand off work; a peer-comms card controls who talks to whom.

Every chat in the sidebar is a real agent with its own model, computer, and connected apps.

OAuth once, no passwords

Gmail, Slack, GitHub, Notion, Linear, and 500+ other apps connect over Composio. You approve each app once; every bot can use it; the scoped tokens stay on your disk. A bot never sees a password, which is the part of the ClawHavoc story that should worry you most.

Connect an app once. Every bot gets it. No password is ever handed to a bot.

Your subscriptions, any model per bot

Claude, Codex, and Grok sit side by side in a provider rail, with Cursor, Kimi, Droid, Antigravity, OpenCode, and Qwen alongside. Any ACP CLI or OpenAI-compatible endpoint also works, so a local model behind an Ollama-style endpoint is possible. Pick a model per bot and switch mid-conversation.

One bot, any model. Unavailable providers are dimmed with the reason.

Here is a live simulation of four bots working in parallel:

Search Inbox 2:21 AM Keeps the mail moving Inbox Release 1:04 AM Published. latest.yml is live, so anyone… Release Chief of Staff 9:12 AM One cause, not three: the mobile signup… Chief of Staff Weekly numbers 6:00 AM Monday's report is ready. Revenue up 4%… Weekly numbers Research Yesterday The split is about trust, not capability… Research Review Yesterday One real problem: the broker resolves an… Review MS Milind Soni Inbox Claude Sonnet 5 Message Inbox +

A simulation. Pick a bot, or type to it. The replies are scripted; the real thing runs on your own machine.

What OpenClaw still does better

Three things, and they matter. OpenClaw lives inside WhatsApp, Telegram, Signal, iMessage, and twenty other channels; MausBot bots live in the MausBot app and its phone companions, not in your existing messaging apps. OpenClaw has ClawHub, a skill catalogue MausBot has no equivalent of. And OpenClaw has 390,000 stars and a far larger contributor base behind it, while MausBot is a young project at roughly 3,200. If channel reach or skill count is the job, OpenClaw wins today.

Other OpenClaw alternatives

Hermes Agent from Nous Research is the closest thing to OpenClaw in scope: MIT, Python, about 248,000 stars since its February 2026 launch, 20+ chat gateways, cron, subagents, and a memory that writes its own skills. It uses Codex-style command approval and has a desktop app in public preview. Complaints: the self-evaluation always reports success, it overwrites hand-edited skills, the setup wizard can loop, and it is single-agent only.

ZeroClaw is a single Rust binary with 30+ channels, a supervised default, and sandboxes, at about 33,000 stars. The right pick if you want OpenClaw's shape with a smaller footprint and a safer default, and you are happy in a terminal.

NanoClaw puts every chat in its own Docker container on the Claude Agent SDK, about 31,000 stars, on Mac, Linux, and WSL2. Isolation is the safety story; there is no approve UI.

Goose from Block is Apache 2.0 with about 55,000 stars, a desktop app and a CLI, approval modes, native MCP, and 15+ model providers. Closer to a coding and task agent than a chat bot, and a solid choice if you want a GUI from a large company.

Claude Cowork from Anthropic is closed source, Claude only, and part of every paid Claude plan. It merged into the single Claude experience on September 16, 2026. Polished, but no local models and no other vendor. We wrote up the open-source options separately.

Grok Bot from xAI is a roster of named bots in a messaging app, in beta since August 11, 2026. Grok only, one shared cloud computer per account, bundled with SuperGrok and Cursor plans from $30 and $20. See Grok Bot vs MausBot .

OpenClaw vs Hermes vs ZeroClaw vs MausBot

Stars were read on September 22, 2026. Where a project does not publish a figure in the sources we used, the cell says so.

OpenClaw Hermes Agent ZeroClaw MausBot

License MIT MIT MIT / Apache Apache 2.0

GitHub stars ~390k ~248k ~33k ~3.2k

Interface Gateway daemon plus a browser Control UI, CLI/TUI, and native apps. Config-file heavy. CLI, plus Hermes Desktop in public preview since June 2026 A single Rust binary, driven from the terminal A desktop chat app. Every contact in the sidebar is a bot.

Default before running a shell command Runs it. Exec mode defaults to full on gateway hosts; ask mode must be switched on. Codex-style command approval Supervised mode An Allow / Deny card in the chat, before anything runs

Chat channels WhatsApp, Telegram, Discord, Slack, Signal, iMessage, Teams, 20+ in all 20+ chat gateways 30+ channels None. You talk to bots inside the app, or on the iOS and Android companions.

Models Claude, OpenAI via a ChatGPT subscription, DeepSeek, Ollama and local Nous Portal, OpenRouter, OpenAI, Anthropic, custom and Ollama See the project README Claude, Codex, and Grok CLIs with your existing login; Cursor, Kimi, Droid, OpenCode, Qwen; any OpenAI-compatible endpoint

Platforms Gateway on macOS, Linux, Windows; native apps for macOS, iOS, Android, Wear OS, Windows, Linux Linux, macOS, WSL2, native Windows (experimental), Termux See the project README macOS (Apple Silicon and Intel), Windows x64, Ubuntu

Which one should you choose?

Stay on OpenClaw if you need your agent inside WhatsApp or Signal, you want the biggest skill catalogue, and you are the kind of person who will set exec mode to ask , keep the gateway off the public internet, and read the release notes.

Choose Hermes if you want OpenClaw's reach with a command gate on by default and you like Python.

Choose ZeroClaw or NanoClaw if you want a smaller, sandboxed footprint and a terminal is home.

Choose MausBot if you want a desktop app on Mac, Windows, or Ubuntu, an approval card before every command as the default, OAuth instead of passwords, more than one bot with more than one job, and your existing Claude, Codex, or Grok login doing the work. It is the safer starting point for someone who does not want to operate a daemon.

Frequently asked questions

Is OpenClaw safe? It can be, if you run it carefully. The record says most people do not. CVE-2026-25253 allowed one-click remote code execution through the Control UI, and runZero counted around 17,500 exposed instances at the time. In February 2026 scans found 135,000 exposed gateways, then 312,000 on port 18789. The v2.0 release in August added approvals and plugin trust review, but The Register noted that secrets still sit unencrypted at rest and the sandbox is not enabled automatically. Does OpenClaw ask before running commands? Only if you configure it to. OpenClaw has exec approvals with deny, allowlist, ask, auto, and full modes, but the default on gateway hosts is full, which runs commands without a prompt. The docs also say approvals are not a per-user auth boundary. MausBot shows an Allow / Deny card by default for every shell command, file edit, and question. Can I use my ChatGPT or Claude subscription with the alternatives? With most of them. OpenClaw uses Claude and reaches OpenAI through a ChatGPT subscription via the Codex runtime. Hermes talks to Anthropic and OpenAI directly, or through Nous Portal and OpenRouter. MausBot runs bots on the claude, codex, and grok CLIs already installed on your machine, so the login you have is the login it uses. No extra API key is needed. Which OpenClaw alternative works on Windows? OpenClaw itself has a Windows gateway and a native Windows app, though the Windows install script is a common complaint. Hermes runs under WSL2 and has an experimental native Windows build plus a Windows desktop preview. MausBot ships a Windows x64 installer, and the bot can control the Windows machine it is installed on. Is there an OpenClaw alternative with a GUI? Yes. OpenClaw has a browser Control UI and native apps but is still configured through files. Hermes Desktop has been in public preview since June 2026. Goose from Block ships a desktop app alongside its CLI. MausBot is a desktop app first: there is no gateway to run and no config file to hand-edit before the first message.

Get started in two minutes

The harness is embedded, so there is nothing else to install. Download for macOS , Windows , or Ubuntu , sign in with the CLIs you already have, and meet your first bot. The iOS and Android companions are shared in our Discord . Or read the source on GitHub first. Everything on the features list is free; you pay your model providers, not us.

Read next

Managed OpenClaw hosting compared, and the no-server option

Nine hosts sell managed OpenClaw, from $5.99 to $499 a month. What you get, the renewal traps, what a managed workspace means, and a free option with no server.

OpenClaw on a VPS or a Mac mini? There is a third option

Where to run OpenClaw: a cheap VPS, a Mac mini in a cupboard, or a managed host. What each costs and breaks, and the desktop-app route that needs none of them.

Every open source AI agent app, compared (October 2026)

Sixteen open source agents, from OpenClaw and Hermes to the open-dot, OpenBot, OpenMuse and OpenInstinct clones, on licence, models, computer use and approvals.

Side by side

OpenClaw alternative: MausBot

An OpenClaw alternative that asks before shell commands run, ships as a desktop app for Mac, Windows and Ubuntu, and uses the Claude or ChatGPT login you have.

Hermes Agent alternative: MausBot

Hermes Agent is a built-in MausBot engine: run Hermes with a GUI, rooms, automations and phone apps beside Claude and Codex bots, or use MausBot instead.

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

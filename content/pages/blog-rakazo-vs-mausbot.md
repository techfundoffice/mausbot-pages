---
layout: default
title: "Rakazo vs MausBot: two open source Grok Bots, compared"
description: "Rakazo is Inbox Zero’s Apache 2.0 Grok Bot alternative: web, desktop and mobile clients on one self-hosted API with Docker. MausBot installs in a minute."
permalink: "/blog/rakazo-vs-mausbot/"
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

October 8, 2026 · 9 min read · Omkar Satpute and Milind Soni

Rakazo vs MausBot: two open source Grok Bots, compared

Rakazo is Inbox Zero’s Apache 2.0 Grok Bot alternative: web, desktop and mobile clients on one self-hosted API with Docker. MausBot installs in a minute.

Rakazo and MausBot are the two Apache 2.0 Grok Bots. Rakazo, launched by Elie Steinbock of Inbox Zero on August 13, 2026, is a server you host, with Postgres, a job worker and a Docker desktop per bot, and web, desktop and mobile clients on top; it has the widest model menu of any clone and no vendor in the path, and it is in beta with no Windows build. MausBot is the open source Grok Bot with no server at all: a desktop app of bots on your own machine, signed installers for Mac, Windows and Ubuntu, store phone apps, and an approval card before every command.

What is Rakazo?

elie222/rakazo appeared two days after Grok Bot, in a launch tweet that listed the recipe: any LLM through the Pi harness, any sandbox provider or Docker, web, desktop and mobile clients, Apache 2.0, built with Cursor and Grok 4.6. The follow-up article was titled “How I built an open source Grok Bot in a day”. Two months on it has 3,418 stars, 76 contributors, daily commits, and a site whose title tag reads “Open source Grok Bot alternative”. In its own words:

“An open source AI agent for persistent teammates, and a self-hosted AI assistant you can run on your own machine.”

“Available on the web, as an Electron desktop app, and through an Expo mobile app.” All three are clients of one self-hosted API.

“Once Rakazo is running, it is just chat, like Grok Bot: you set up a bot and manage it from that chat.”

“Rakazo is in beta.”

Sign in with Claude Pro or Max, ChatGPT Plus or Pro, or use an Anthropic or OpenAI key; OpenRouter, Grok, SuperGrok, Ollama and LM Studio work too, swapped per bot.

Bot computers from Docker, E2B, Daytona, CreateOS, Box or your own Mac, shared as Team computers or isolated as Private ones.

Approvals you set per bot, an audit log you own, and site logins stored encrypted so the model sees neither username nor password.

Routines as plain Markdown you can read, edit and commit.

Slack, WhatsApp, Telegram and iMessage bridges, and a voice mode.

A vision document that promises no hosted vendor ever becomes a hidden dependency of the self-hosted core, and keeps that promise.

The costs of that design are also on the record. The desktop app’s “This computer” option installs and starts the published images with Docker Compose, so Docker Desktop, OrbStack or Docker Engine must be present. A review measured about 2 GB and 2 CPUs per active bot, counted 815 commits in 28 days with 169 by a Cursor agent account, and noted no Windows desktop build and no hosted version. The last tagged release is 0.1.6 from September 8, a Mac DMG and a Linux AppImage, while main has moved daily since; the Windows build is skipped unless a signing certificate is configured. Open issues this week include bots unable to read PDF or Office documents, MCP OAuth failing, and the desktop tunnel not connecting. One launch-day write-up put it fairly: the Grok Bot framing describes an alternative architecture, not proven feature parity.

Rakazo vs MausBot

Rakazo MausBot

Launched August 13, 2026, two days after Grok Bot August 11, 2026

Made by Elie Steinbock; maintained by Inbox Zero Inc.; 76 contributors, 169 commits by a Cursor agent account Supamaus Software, an independent open-source project

Stars, forks 3,418, 599 About 4,200, 716

License Apache 2.0 Apache 2.0

Status Beta Shipping releases since August

Shape One self-hosted API (Hono, Postgres, a job worker) with web, Electron and Expo clients A desktop app with no server; iOS and Android companions

Setup Docker Desktop plus a published-images script, or the desktop app, which installs and starts that stack Download, sign in with your CLI, meet a bot

Installers Mac universal DMG and Linux AppImage in v0.1.6 (September 8); no Windows asset in any release; mobile from source Signed macOS, Windows and Ubuntu installers; App Store and Play Store apps

Models Claude Pro/Max, ChatGPT Plus/Pro, SuperGrok and Copilot sign-in; Anthropic, OpenAI, OpenRouter keys; Ollama, LM Studio; per bot, via Pi Claude, Codex, Grok and other CLIs, chosen per bot, on your existing logins

Each bot’s computer Docker by default (a Chromium desktop per bot), or E2B, Daytona, CreateOS, Box, or your Mac; Team or Private Your own machine; or a cloud desktop per bot

Resources About 2 GB and 2 CPUs per active bot, per one review The CLI’s own footprint

Before it acts Approval rules per bot; an audit log you own; site logins the model never sees Allow / Deny cards for shell commands and file edits, by default

Agents Persistent bots with memory, routines in Markdown, peers, subagents, group channels As many bots as you like, in rooms; routines

Reach it from Web, desktop, mobile; Slack, WhatsApp, Telegram, iMessage bridges; voice mode Desktop, iOS and Android apps, in-app calls

Always on Yes, wherever you host the stack A Cloud plan from $15 a month, or npx openmausbot serve

Hosted version A waitlist Cloud plans, today

Vendor dependency None; VISION.md commits to that None

What MausBot is, in the same terms

MausBot is the same idea with the server removed. It is a chat app where every contact is a bot on the claude , codex or grok CLI already installed on your machine, using the login you already have; the app talks to a harness on 127.0.0.1 and nothing else. Bots share rooms and hand work to each other, run routines, and connect to 500+ apps over Composio. Shell commands and file edits become Allow / Deny cards before they run, by default. Your data is in ~/.openmausbot . It installs from a signed DMG, EXE or deb in about a minute, the iOS and Android apps are in the stores, and the code is on GitHub under Apache 2.0. When you want bots working with the laptop closed, Cloud plans start at $15 a month, today, or you run npx openmausbot serve on a box of your own.

What Rakazo still does better

Three first-party surfaces on one API, plus Slack, WhatsApp, Telegram and iMessage bridges and a voice mode. MausBot has the desktop app, the phone apps and in-app calls, and no messaging bridges.

The widest provider matrix of any clone: Claude, ChatGPT, SuperGrok and Copilot subscriptions, API keys, OpenRouter, Bedrock, Ollama and LM Studio, per bot.

Pluggable sandboxes, with shared Team computers and isolated Private ones, and per-site encrypted logins the model never sees.

Always-on by construction, because it is a server; MausBot’s always-on is a Cloud plan or your own serve command.

A UI in nine languages.

The verdict

These two are closer than any other pair on this site, and the difference is where the weight sits. Rakazo puts it in a server: more surfaces, more providers, more bridges, and a Docker stack, two gigabytes a bot, a month-old installer and no Windows build to carry it. MausBot puts it in an app: install in a minute on any desktop, phone apps from the stores, an approval card before every command, and a Cloud plan you can buy today instead of a waitlist. Same licence, same shape, same refusal to put a vendor in the path. For the person who searched “open source Grok Bot” and wants to be talking to a bot in the next five minutes, MausBot is the one that gets them there, and on the evidence in the table it is the better app.

Frequently asked questions

Is Rakazo open source? Yes, Apache 2.0, the same licence as MausBot. One bundled tool source, Treg, is usage-metered and needs a written agreement for hosted resale, which matters only if you sell Rakazo as a service. Does Rakazo run on Windows? Not as a desktop app. No release has a Windows asset, and the build is skipped unless a signing certificate is configured. You can run the server stack on Windows with Docker and use the web client. MausBot ships a native Windows installer. Can I use my Claude or ChatGPT plan in Rakazo? Yes, through the Pi harness, with Claude Pro or Max, ChatGPT Plus or Pro, SuperGrok and Copilot sign-in. MausBot does the same through the claude, codex and grok CLIs. Neither bills you per token for those. Why does Rakazo rank for “open source Grok Bot”? Its home page title is that exact phrase, it has a dedicated page per rival, and it launched two days after Grok Bot. The ranking says something about SEO and nothing about which app is better; this page exists so you can judge that from the table. Rakazo or MausBot? Rakazo if you want to host one server that several surfaces and messaging bridges connect to, you run Docker happily, and Windows is not your desktop. MausBot if you want the Grok Bot shape as an app you install in a minute on Mac, Windows or Ubuntu, with phone apps from the stores and a Cloud plan when the laptop is closed.

Read next

Rakazo vs MausBot , the one-page summary.

OpenBot vs MausBot , CopilotKit’s Grok Bot for companies.

The open source alternative to Grok Bot , against Grok Bot itself.

OpenBot by CopilotKit vs MausBot: open source Grok Bots

Open Bot, CopilotKit’s MIT template of AI coworkers, is built for companies and needs a CopilotKit account. MausBot is the open source Grok Bot for a person.

Grok Bot Team Bots vs MausBot teams: shared agents compared

xAI's Grok Bot Team Bots, in public beta since Sept 28, against MausBot's Team plan and free rooms: price for five people, who runs the bot, chats, approvals.

Muse vs Grok Bot vs Dots vs Cue: which agent to pick

Meta Muse, xAI Grok Bot, OpenAI dots, and Cue by Manus compared on price, region, models, approvals, and where the agent runs, plus the open-source fifth.

Side by side

OpenBot vs MausBot

OpenBot is CopilotKit's MIT template of AI coworkers for companies, and needs a CopilotKit account to start. MausBot is the open source Grok Bot for a person.

Rakazo is Inbox Zero's open source Grok Bot: web, desktop and mobile clients on one self-hosted API. MausBot is the one that installs in a minute. Compared.

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

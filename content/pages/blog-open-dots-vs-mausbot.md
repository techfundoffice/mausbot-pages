---
layout: default
title: "Open Dots vs MausBot: three open source dots, one app"
description: "Composio’s open-dot, Anil Matcha’s Open Dots and CopilotKit’s OpenDots all claim to be the open source OpenAI dots. What each is, and how MausBot compares."
permalink: "/blog/open-dots-vs-mausbot/"
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

October 8, 2026 · 10 min read · Omkar Satpute and Milind Soni

Open Dots vs MausBot: three open source dots, one app

Composio’s open-dot, Anil Matcha’s Open Dots and CopilotKit’s OpenDots all claim to be the open source OpenAI dots. What each is, and how MausBot compares.

Open Dots is three different projects, and MausBot is the app. Within a day of OpenAI launching dots on September 29, 2026, Composio published open-dot, Anil Matcha published Open Dots and CopilotKit published OpenDots. One is a Mac app you build yourself with no licence and no commits since September 30; one is a 2023 repository renamed on launch day and rebuilt since as a Telegram front end for Claude Code; one is an MIT web template that needs CopilotKit’s cloud to start. MausBot is the open source dots that is finished: a team of bots on any model, on your own machine, Apache 2.0, with installers and phone apps.

What “open dots” means on GitHub

OpenAI’s dots are always-on personal agents for ChatGPT Pro and Business Premium subscribers, which is to say $100 a month and up, and not in the EEA, Switzerland or the UK. The Register reported on October 7 that the launch “inspired open source imitators amid technical difficulties”. Four repositories took the name within 26 hours. Here is what each one is, from its own repository, read on October 8.

open-dot, by Composio

composio-community/open-dot is the work of Prathit Joshi, a growth engineer at Composio, and was announced by Composio co-founder Karan Vaidya in a tweet seen 235,000 times. It is an Electron window around a local Next.js server, for Apple Silicon Macs only, and you build the DMG yourself. It takes an OpenAI key, or an OpenRouter key for open models, gives each dot a persistent Chrome profile with live view and takeover, connects 1,500 apps and event triggers through Composio, keeps passwords in the macOS Keychain and types them into pages so the model never sees them, and routes risky actions through rules you write and a small review model that produces approve or deny cards. That is a wide feature list for a repository with four commits, all on September 29 and 30, and nothing since. It has no licence file. A user who asked permission to publish a Windows build got “yes, feel free” in an issue, which is kind, and is not a licence. Eight community pull requests, including sign in with ChatGPT and local models, sit unreviewed.

Open Dots, by Anil Matcha

Anil-matcha/open-dots has the most stars of the three, 5,517, and the strangest history. The GitHub API says the repository was created on May 25, 2023, and its pull request list still contains 2023 patches from a privateGPT fork. It was renamed on launch day, announced in a tweet seen 173,000 times, and did trend on GitHub. On October 7 its main branch was force-replaced: the current root commit has no parents, and the September 30 merge that fixed a burst of reported security issues has no common ancestor with it. The product changed with the history. The version that launched was a local Next.js and FastAPI workspace with personas and a deny-by-default action gateway; the version on main today is a FastAPI API, a Telegram bot and a web UI that runs Claude Code in Boat cloud sandboxes, Claude only, by OAuth login, with a permission hook that times out to deny. The README now positions it against dots, Muse, Grok Bot, Instinct, Cue and Cowork at once, in commits literally named “position Open Dots as paid agent alternative”. The licence file that the October 3 snapshot had is gone from the tree, though the description still says MIT.

OpenDots, by CopilotKit

CopilotKit/OpenDots is the serious one: 4,270 stars, MIT, 53 commits in the last 30 days, a company behind it. It is a web template for always-on coworkers that move between text, calls and Slack, each with a computer from CopilotKit’s OpenBot containers. The README says it plainly: “a template, not a hosted product”. Conversations require CopilotKit Intelligence, which by default means CopilotKit’s cloud, with a free tier of 200 threads kept for three days and paid tiers at $39 a month and $100 a seat, and telemetry on unless you set a flag. Multi-dot group chat and delegation are listed as further work. It is the best open-source code in this group, and it is a developer’s starting point rather than a thing a person installs.

For completeness: Digger’s opendots (19 stars, dead after launch day, agents on Digger’s own cloud) and Shashankss1205/OpenDots (26 stars, a one-day Python runtime) exist. feder-cr/invisible_dots, with 31,817 stars, also positions itself as the open-source dots, on a repository created in 2024 for a different purpose; it gives each dot a QEMU virtual machine and an anti-detection Firefox, on Windows and Linux only, and is a different kind of project.

Open Dots vs MausBot, side by side

open-dot Open Dots OpenDots MausBot

Made by Prathit Joshi at Composio, one contributor Anil Matcha, three contributors CopilotKit, a VC-backed company Supamaus Software, an independent open-source project

Created September 29, 2026 May 25, 2023, renamed on launch day; history replaced October 7 September 29, 2026 August 11, 2026

Stars, forks 600, 94 5,517, 659 4,270, 601 About 4,200, 716

License None in the repository None on disk; the description says MIT MIT; CopilotKit Intelligence is outside it Apache 2.0, app and harness

Shape An Electron window around a local Next.js server A FastAPI API, a Telegram bot and a web UI in Docker A web template; a mobile app is claimed A desktop chat app; iOS and Android companions

Platforms macOS on Apple Silicon only; build the DMG yourself Anything with Docker; no desktop app Any Node 24 host macOS, Windows, Ubuntu; iPhone, Android

Installer No No No Yes, signed, plus store apps

Models An OpenAI key, or OpenRouter for Kimi, DeepSeek, Qwen, GLM; no Anthropic, no local Claude only, by OAuth subscription login Any OpenAI-compatible key Claude, Codex, Grok and other CLIs, chosen per bot

Where the agent runs Your Mac; code on E2B, Docker or a folder Boat cloud sandboxes, $20 a month after a trial, with a public URL for approvals Your server, with threads in CopilotKit’s cloud Your own machine, or a cloud desktop per bot

Before it acts Rules you write plus a small review model; cards in chat A Claude Code PermissionRequest hook: Allow once, Always, Deny; deny after 110 s Approve-and-run cards for non-read-only tools Allow / Deny cards for shell commands and file edits, by default

Several agents Yes, dots pass work to each other No One owner; group chat listed as further work As many bots as you like, in group rooms

Routines Yes, and Composio triggers, only while the app is open Cron schedules, reported to Telegram Scheduled turns Routines, with the laptop closed on a Cloud plan

Phone None Telegram An Expo app, no store listing iOS and Android apps

Last commit September 30, 2026 October 7, 2026 October 6, 2026 Daily

HN launch thread 2 points, 0 comments 3 points, 1 comment 2 points, 0 comments n/a

What MausBot is, in the same terms

MausBot is a chat app where every contact is a bot. Each bot runs on the claude , codex or grok CLI installed on your own machine, with the login you already have, so a Claude bot and a Codex bot can share a room and hand work to each other. Shell commands and file edits surface as Allow / Deny cards before they run, by default, for every engine. Your conversations, memory and files stay in ~/.openmausbot on your disk; the harness listens on 127.0.0.1 only. It ships as signed installers for macOS, Windows and Ubuntu, with iOS and Android apps in the stores, and 500+ connected apps over Composio, the same catalogue open-dot uses. The code is on GitHub under Apache 2.0, app and harness, with no vendor service in the path. Cloud plans from $15 a month keep bots working with the laptop closed; the free app needs no account.

What the Open Dots projects still do better

open-dot has Composio event triggers, so a bank email or a new GitHub issue can wake a dot; MausBot’s routines are on a schedule. Its Keychain vault that types passwords into pages without the model seeing them is a design MausBot has deliberately not shipped, because a bot that controls the browser can read what the browser shows. open-dot also has voice calls over OpenAI’s realtime API.

Open Dots lets you drive a Claude Code session from Telegram with approval buttons in the chat, on a Claude subscription rather than an API key, with permission rules scoped per git verb so “always allow commit” does not allow push.

OpenDots has WebRTC calls, Slack through the Channels SDK, and a durable task engine, and it is maintained daily by a funded team.

The verdict

Judge the four on what a person can do today. Two of the three Open Dots cannot be legally redistributed because they have no licence. None of the three installs: you build a Mac app, run a Docker stack, or deploy a template. Each is tied to one model vendor. Two are single-agent. One has not had a commit in eight days; one replaced its history and its product in the same week. MausBot is the only one in the table that is open source under an OSI licence, ships installers and store apps, runs any model per bot on the plan you already pay for, gates shell commands by default, and has been committed to daily since August. For the searcher typing “open dots”, it is the one that works.

Frequently asked questions

Is there an open source OpenAI dots? Three projects claim the name and none is quite that. As of October 8, 2026, Composio’s open-dot and Anil Matcha’s Open Dots have no licence file, which in law means all rights reserved; CopilotKit’s OpenDots is MIT but cannot run without CopilotKit’s hosted Intelligence service. MausBot is Apache 2.0, app and harness, and runs with no vendor service. What is the difference between open-dot, Open Dots and OpenDots? open-dot (one t) is Composio’s Mac app, launched by Karan Vaidya on September 30. Open Dots is Anil Matcha’s repository, launched September 29 and rebuilt since. OpenDots is CopilotKit’s web template, launched the same day. They share nothing but the name and the launch week. Which one runs on Windows? Only Anil Matcha’s, as a Docker stack with a Telegram bot and no desktop app. open-dot is macOS only and OpenDots is a web template. MausBot ships a native Windows installer. Does MausBot use any Open Dots code? No. MausBot started on August 11, 2026, seven weeks before dots existed, and is an independent codebase under Apache 2.0. Is any of them cheaper than OpenAI’s dots? They are all free to download and you pay a model provider. open-dot’s launch tweet claimed a tenth of the cost; nothing in the repository substantiates a figure. MausBot runs bots on the Claude, ChatGPT or Grok plan you already pay for, so the marginal cost of a bot is zero.

Read next

Open Dots vs MausBot , the one-page summary of this comparison.

The open source alternative to OpenAI’s dots , which compares MausBot with dots itself.

Every open source AI agent app, compared , the round-up.

Meta Muse vs OpenAI dots: the two one-agent products

Meta Muse and OpenAI dots compared on price, region, model, where the agent runs, memory, training, and phone calls, plus the open-source third option.

Muse vs Grok Bot vs Dots vs Cue: which agent to pick

Meta Muse, xAI Grok Bot, OpenAI dots, and Cue by Manus compared on price, region, models, approvals, and where the agent runs, plus the open-source fifth.

OpenAI Dots alternative: free, open source, any model

OpenAI's dots need ChatGPT Pro or Business Premium and run on GPT only. MausBot is the free, open-source alternative: a team of agents on your own machine.

Side by side

Open Dots vs MausBot

Three projects call themselves the open source OpenAI dots: Composio's open-dot, Anil Matcha's Open Dots, CopilotKit's OpenDots. Each vs MausBot, from GitHub.

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

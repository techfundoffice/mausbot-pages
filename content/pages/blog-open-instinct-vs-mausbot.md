---
layout: default
title: "OpenInstinct vs MausBot: the open source Instinct clones"
description: "Two serious OpenInstinct projects exist, from Merit Systems and from Maritime’s CEO, both iMessage agents you deploy. How they compare with MausBot, the app."
permalink: "/blog/open-instinct-vs-mausbot/"
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

OpenInstinct vs MausBot: the open source Instinct clones

Two serious OpenInstinct projects exist, from Merit Systems and from Maritime’s CEO, both iMessage agents you deploy. How they compare with MausBot, the app.

OpenInstinct is two unrelated projects, both services you deploy; MausBot is an app you install. Instinct, from Spear Street Technology, is an agent you text on iMessage that has its own computer and talks to your friends’ agents. Merit Systems’ OpenInstinct (422 stars, MIT) rebuilds that on Vercel Pro with a Kernel cloud browser and a Linq iMessage line, and says it is not for production use. Maria Gorskikh’s open-instinct (241 stars, MIT) rebuilds it on Maritime microVMs with a code-enforced trust network, five days old. Both are one agent, reached by text. MausBot is the open source agent you open on your desk: a team of bots on any model, on your own machine, Apache 2.0.

What Instinct is, and what “open instinct” means

Instinct is a personal agent you reach by iMessage. It has a phone number, a computer of its own, memory, and a “trusted people” network so your agent can book a dinner with a friend’s agent. It opened an invite-only beta on August 26, 2026 and raised at a $10 billion valuation a month later. The open-source clones copied the shape. GitHub has about 140 repositories in the OpenInstinct name family including forks; most are empty or one-day builds. Two are real.

OpenInstinct, by Merit Systems

Merit-Systems/OpenInstinct shipped the day after Instinct’s beta opened, with a Show HN that drew five points and no comments. Its README puts it well: “A personal iMessage assistant that can use a browser like you … You stay in control of your passwords, credit cards, and context. It’s open source, self-hostable, and can use any model. Deploy to your own Vercel account and get rolling.” It is a Next.js app on Vercel’s Eve agent framework, with Neon Postgres, private Blob storage, a Linq-managed iMessage number, Kernel cloud browsers driven by a browser subagent, Gmail and Calendar over OAuth, a vault whose secrets are autofilled into pages so the model never sees them, Stripe Link for purchases with a tap approval, and scheduled workers that check for work every minute, which is why Vercel Pro is required. It is multi-tenant, so a family can share a deployment. It is maintained: ten fix pull requests on October 7. It also says, in the README, “This is not software intended for production use”, and its execution-safety instructions say tools “run without a separate Eve approval step”: the gate before a consequential action is a sentence the model is asked to follow, with Stripe Link’s own approval as the hard stop for money. It has no local-model path and no way to use a ChatGPT or Claude plan.

open-instinct, by Maria Gorskikh

mariagorskikh/open-instinct is five days old at this writing: created October 3, 38 commits, 837 tests, nine packages, a documented research dossier on Instinct, and three points on HN . Its README: “An open-source personal agent you text. It has its own computer, does real tasks, and coordinates with the agents of the people you trust. A from-scratch, documented clone of Instinct, built so anyone can run one.” You text a number from Inkbox; a gateway wakes your agent in a Firecracker microVM with a Linux desktop on Maritime, which sleeps when idle; inside, a Pi agent loop runs with Composio for apps, Stripe Link single-use cards for money, and “a policy guard in front of every tool” with six trust tiers, owner to stranger, enforced in code. It is the only clone that rebuilds Instinct’s agent-to-agent network, with a typed protocol for proposing times and booking. It defaults to Claude and supports any Pi provider including Ollama. Two things to weigh: the author is the CEO of Maritime , the managed cloud that is the default host, and the one open issue lists quiet hours, the proactive cap and parts of memory as unimplemented must-haves.

The rest

Yeachan-Heo/openinstinct is a Mac menu-bar agent with thirteen releases that reuses your Claude or Codex CLI login and keeps everything local, which is close to MausBot’s own design; it has 20 stars, 81 downloads and no licence file. samagra14/openinstinct was a one-day experiment on Codex and Inbox. zoltlabs/OpenInstinct is an alpha on a $39-a-month iMessage API. Comma, Nell, gutsy and skytwin position against Instinct without the name. And “open cue”, the phrase people type for a free Cue by Manus, matches nothing: every OpenCue on GitHub is a render farm, a teleprompter or a keyboard tool.

OpenInstinct vs MausBot, side by side

Merit OpenInstinct Gorskikh open-instinct MausBot

Made by Merit Systems; four core developers, 497 commits Maria Gorskikh, CEO of Maritime (YC F26), with five contributors; 38 commits Supamaus Software, an independent open-source project

Launched August 27, 2026, the day after Instinct’s beta opened October 3, 2026 August 11, 2026

Stars, forks 422, 74 241, 61 About 4,200, 716

License MIT MIT Apache 2.0, app and harness

Status “Not software intended for production use” Version 0.1, “treat them as beta” Shipping releases since August

Shape A Next.js service on Vercel; you text it on iMessage A Node service and CLI; a microVM per person on Maritime; you text it A desktop chat app of bots; iOS and Android companions

Needs Vercel Pro, Kernel cloud browsers, Neon Postgres, a Linq iMessage line, Vercel AI Gateway Inkbox for the phone number, Maritime for the VM, Composio for apps, Stripe Link for money A download and the CLI login you already have

Reach it from iMessage, so an iPhone; a web dashboard iMessage, SMS or email The desktop app, iOS and Android apps, in-app calls

Models Any model through Vercel AI Gateway, billed per token; no local models Claude by default; any Pi provider, including Ollama and vLLM; API keys Claude, Codex, Grok and other CLIs, chosen per bot, on your existing logins

Its computer A Kernel cloud browser run by a browser subagent; no local computer A Firecracker microVM with a Linux desktop that sleeps when idle; or your laptop Your own machine; or a cloud desktop per bot

Before it acts Prompt-level: instructions tell the model to ask before purchases or messages; tools run without a separate approval step; money is gated by Stripe Link A policy guard in front of every tool; six trust tiers enforced in code; logins and payments go to you by desktop takeover or Link Allow / Deny cards for shell commands and file edits, by default

Agents One per person, multi-tenant; a browser subagent and scheduled workers One per person; talks to other people’s agents over a typed protocol As many bots as you like, in group rooms

Memory Per-user memory in Vercel Blob; workstreams in Postgres MEMORY.md, a daily journal and contacts.json you can read Per bot, on your disk

Proactive Scheduled workers every minute, hence Vercel Pro Cron and one-shot schedules that wake the VM; quiet hours not yet implemented Routines; always-on with a Cloud plan

Voice None None In-app calls

Cost to run Vercel Pro from $20 a month, plus Kernel, Neon, Linq and model usage Inkbox plan, Maritime from $1 an agent a month while awake, model usage Free; Cloud plans from $15 a month if you want always-on

Launch reception Show HN, 5 points, 0 comments HN, 3 points, 1 comment n/a

What MausBot is, in the same terms

MausBot is a chat app on your desk, not a number you text. Every contact is a bot on the claude , codex or grok CLI installed on your own machine with the login you already have, so there is no gateway, no per-token bill and no cloud to provision. Bots share rooms and hand work to each other, which is MausBot’s answer to Instinct’s network: your bots coordinate with each other on your machine rather than with a stranger’s agent over a protocol. Shell commands and file edits surface as Allow / Deny cards before they run, by default, which is a gate in code, not a sentence in a prompt. Data stays in ~/.openmausbot ; the harness listens on 127.0.0.1 only. It installs from a signed DMG, EXE or deb; the iOS and Android apps are in the stores, with Live calls; and the code is on GitHub under Apache 2.0. Cloud plans from $15 a month add an always-on computer per bot for the laptop-closed case.

What the OpenInstinct projects still do better

Merit Systems : one-click provisioning of browser, database, storage, iMessage line and model gateway in about five minutes; a model-blind vault that autofills passwords and cards; real purchases through Stripe Link; multi-tenant from day one. The vault design is one MausBot has deliberately not shipped, because a bot that controls the browser can read what the browser shows.

Maria Gorskikh : the agent-to-agent trust network with code-enforced tiers and a written protocol, which nobody else clones; a sleeping microVM desktop per person; single-use cards; local models; Markdown memory you can read; an audit log of every side effect.

Both : a phone number the agent owns, so anyone can text it like a person, with no app to install on the phone.

The verdict

Both OpenInstinct projects are honest, well-documented clones of a product whose shape is a service: a number in the cloud, a computer in the cloud, four vendors to pay, one agent per person, iMessage or nothing. If that is what you want, pick Gorskikh’s for the trust network and local models, or Merit’s for five-minute provisioning, and read the “not for production” and “beta” labels first. If what you want is the thing Instinct does, an agent that remembers you, acts on your behalf and asks before it spends, as something you install and own, then MausBot is the only option in the table that is an app, that gates actions in code by default, that runs more than one agent on more than one model, and that costs nothing beyond the plan you already have. On that evidence it is the best open source answer to Instinct, and the only one at all to Cue.

Frequently asked questions

Is there an open source Instinct? Yes, two: Merit Systems’ OpenInstinct, released August 27, 2026, and Maria Gorskikh’s open-instinct, released October 3. Both are MIT and both are iMessage agents you deploy to cloud services. A third, Yeachan Heo’s Mac menu-bar app, has 20 stars and no licence file. None is an app you install and open. Is there an open source Cue by Manus? No. As of October 8, 2026, no GitHub project positions itself as an open Cue; every repository named open-cue or OpenCue is the Academy Software Foundation’s render-farm manager , a teleprompter, a Corsair keyboard tool or a meeting copilot. The closest open-source match for Cue’s team of agents with their own computers is MausBot; see the Cue comparison . Who makes Instinct? Spear Street Technology, founded by Noah Shinn, formerly of Sierra. It is not an Anthropic, OpenAI or Meta product. It opened an invite-only beta on August 26, 2026 and raised $1 billion at a $10 billion valuation on September 28. Does OpenInstinct work on Android? Merit’s is iMessage only and its site says users need an iPhone. Gorskikh’s gives Android users an SMS line or email. MausBot has native iOS and Android apps. Can OpenInstinct use my ChatGPT or Claude plan? No. Merit’s bills every turn through Vercel AI Gateway; Gorskikh’s takes API keys or a Maritime metered proxy, and supports local models. MausBot runs bots on the claude and codex CLIs with your existing logins.

Read next

OpenInstinct vs MausBot , the one-page summary.

The open source alternative to Instinct , MausBot against Instinct itself.

The open source alternative to Cue by Manus

Meta Muse vs Grok Bot vs Instinct: which agent to pick

Meta Muse, xAI Grok Bot, and Instinct compared on price, region, models, approvals, and where the agent runs, plus the open-source option that works anywhere.

Instinct AI alternative: open source, no invite needed

No Instinct invite, or read its terms and closed the tab? MausBot is a free, open-source alternative: agents on your own machine that ask before they act.

Every open source AI agent app, compared (October 2026)

Sixteen open source agents, from OpenClaw and Hermes to the open-dot, OpenBot, OpenMuse and OpenInstinct clones, on licence, models, computer use and approvals.

Side by side

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

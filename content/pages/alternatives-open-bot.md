---
layout: default
title: "OpenBot (CopilotKit) vs MausBot: open source Grok Bots"
description: "OpenBot is CopilotKit's MIT template of AI coworkers for companies, and needs a CopilotKit account to start. MausBot is the open source Grok Bot for a person."
permalink: "/alternatives/open-bot/"
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

Facts checked October 8, 2026 · CopilotKit · open source

OpenBot vs MausBot

OpenBot is CopilotKit's MIT template of AI coworkers for companies, and needs a CopilotKit account to start. MausBot is the open source Grok Bot for a person.

OpenBot, launched by CopilotKit on August 19, 2026 as Open Bot, is an MIT-licensed self-hosted web template of AI coworkers for companies, with policy, audit and SSO, that calls itself a template rather than a product and will not start without a CopilotKit Intelligence account. MausBot is the open source Grok Bot for one person: a desktop app of bots on your own machine, any model per bot, Apache 2.0.

What OpenBot is

OpenBot (6,182 stars, 841 forks, MIT) is the most-starred of the open source Grok Bot clones. Its README calls it the AI assistant your company can actually own, a template not a product, and alpha. It runs on Docker, Bun and Postgres on your infrastructure, gives each Bot a container with a Chromium browser and a shell, routes every action through a fail-closed CEL policy with an audit row, and offers Google, Microsoft and Okta sign-in and a Helm chart. Any agent framework plugs in over AG-UI. A Tauri desktop and an Expo mobile app live in the tree, but releases ship only container images. Threads and memory live in CopilotKit Intelligence, a managed service with a free developer tier, $39 a month Pro and $100 a seat Team.

Launched: August 19, 2026, eight days after Grok Bot . Sources: CopilotKit/OpenBot on GitHub ; OpenBot on copilotkit.ai ; Wavect: OpenBot self-hosted AI coworkers review .

Why people compare OpenBot with MausBot

It is for companies, by its own description: SSO, people admin, audit export and Helm, with a sales link to have CopilotKit's engineers build it for you.

The server refuses to start without a CopilotKit Intelligence project, so the MIT code depends on an account with one vendor; the local self-hosted Intelligence is a 30-day-renewable macOS preview.

No installer: releases contain only container images, and a GitHub issue asks for a signed Mac build so users stop cloning the repo.

API keys only, no ChatGPT or Claude subscription sign-in, so every turn is billed per token.

Bots drive a browser inside their own container, not the apps on your Mac or PC; the shipped startup policy is permissive according to an independent review.

Desktop telemetry is on by default, disclosed on the welcome screen without an opt-in.

The OpenBot column comes from the vendor's own pages and the press cited above, checked on October 8, 2026 . Where the vendor has not said, the cell says so.

OpenBot MausBot

License, stars MIT, 6,182; needs a CopilotKit Intelligence key to start Apache 2.0, about 4.2k; no vendor service

Shape A self-hosted web app for a company's coworkers; desktop and mobile build-from-source A desktop chat app of bots for a person; iOS and Android companions

Models OpenAI, Anthropic, Google by API key, or any AG-UI agent Claude, Codex, Grok, and other CLIs, chosen per bot; switch mid-conversation

Before a shell command runs A CEL policy evaluated at the gateway, fail closed; approvals page for held actions Allow / Deny cards for shell commands and file edits; answer cards for questions

Agents Coworkers in group chats with delegation; routines with a 15-minute floor As many bots as you like, in group rooms

Where it runs Your Docker host; a container per Bot with Chromium and a shell; threads in CopilotKit's cloud Your own machine; or a cloud desktop per bot

Platforms Any Docker host; Tauri and Expo apps you build yourself macOS, Windows, Ubuntu; iOS and Android companions

Setup Docker, Bun, Postgres, npx copilotkit login Download, sign in with your CLI, meet a bot

Price Free; CopilotKit Intelligence free tier, Pro $39 a month, Team $100 a seat Free. Model usage on the Claude, ChatGPT, or Grok account you already have.

What MausBot is

MausBot is a free, open-source chat app where every contact is an AI bot with its own model, its own computer, and its own connected apps. Bots run on the claude , codex , and grok CLIs installed on your own machine, with your existing logins, so one bot can be on Claude and the next on ChatGPT. Shell commands and file edits surface as Allow / Deny cards before they run, bots share group rooms and hand work to each other, and your data stays in ~/.openmausbot on your disk. It is published on GitHub under Apache 2.0, with iOS and Android companions, and paid Cloud plans from $15 a month keep bots working with the laptop closed.

What OpenBot still does better

Governance as the product: a fail-closed policy language, an audit row written before any action, refusals that name the rule, and audit export to a SIEM.

Enterprise plumbing MausBot does not have: SAML and OIDC sign-in, a people admin page, a Helm chart, optional gVisor isolation per Bot.

Framework-agnostic agents over AG-UI, with a dozen harness examples, and generative UI that answers with components.

The largest star count and contributor base among the Grok Bot clones, backed by a funded company.

Other OpenBot alternatives

The other open-source clones first, then the big agent apps, each with its own comparison page:

Open Dots by Composio, Anil Matcha, CopilotKit : OpenAI launched dots on September 29, 2026 for ChatGPT Pro and Business Premium .

Rakazo by Inbox Zero Inc. (Elie Steinbock) : Rakazo (3,418 stars, 599 forks, Apache 2.0) was created two days after Grok Bot launched and is the closest of the clones to MausBot in shape: persistent bots with their own memory, routines and group channels, each on a model you choose through the Pi harness, including Claude Pro or Max and ChatGPT Plus or Pro sign-in, API keys, and Ollama .

OpenMuse by CopilotKit, nanoMuse and twelve smaller repos : Meta's Muse arrived on September 8, 2026 as a single proactive agent in a secure VM .

OpenInstinct by Merit Systems, Maria Gorskikh (Maritime) and others : Instinct opened its invite-only beta on August 26, 2026 and raised at a $10 billion valuation a month later .

Every other comparison page: Bops , Hark Pro , Grok Bot , Meta Muse , OpenAI dots , Cue by Manus , Instinct , Open Dots , Rakazo , OpenMuse , OpenInstinct , OpenClaw , Hermes Agent , Claude Cowork .

Frequently asked questions

Is OpenBot the same as Open Bot? Yes. The August 19 launch tweets spelled it Open Bot; the repository, README and website spell it OpenBot. There is no CopilotKit/open-bot repository. Is OpenBot a product I can install? Not as shipped. The README says it is a template, not a product, with no hosted version; releases contain only container images. You clone it, replace the example tenant and run it on Docker. Does OpenBot work without CopilotKit's cloud? Not out of the box. The API server needs an Intelligence URL and key. CopilotKit offers a self-hosted Intelligence on paid plans and a 30-day-renewable local preview for macOS. Which is the best open source Grok Bot? For a company that wants policy and SSO on its own servers, OpenBot. For a person who wants Grok Bot's shape, a team of named bots in a chat app on the Claude, ChatGPT or Grok plan they already pay for, with installers and phone apps, MausBot.

Read more

OpenBot by CopilotKit vs MausBot: open source Grok Bots : the full comparison this page summarises.

Open source Grok Bot: MausBot, the free alternative

Rakazo vs MausBot: two open source Grok Bots, compared

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

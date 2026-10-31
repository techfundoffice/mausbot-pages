---
layout: default
title: "OpenInstinct vs MausBot: the open source Instinct clones"
description: "Two serious OpenInstinct projects: Merit Systems' Vercel template and Maria Gorskikh's Maritime agent. Both are iMessage agents you deploy. MausBot is an app."
permalink: "/alternatives/open-instinct/"
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

Facts checked October 8, 2026 · Merit Systems, Maria Gorskikh (Maritime) and others · open source

OpenInstinct vs MausBot

Two serious OpenInstinct projects: Merit Systems' Vercel template and Maria Gorskikh's Maritime agent. Both are iMessage agents you deploy. MausBot is an app.

OpenInstinct is two unrelated GitHub projects that clone Instinct, Spear Street Technology's iMessage agent: Merit Systems' OpenInstinct (422 stars, MIT), deployed to a paid Vercel plan with a cloud browser and an iMessage line, and Maria Gorskikh's open-instinct (241 stars, MIT), a Node service on Maritime microVMs with an agent-to-agent trust network. MausBot is the open source agent you install as an app: bots on your own machine, Apache 2.0.

What OpenInstinct is

Instinct opened its invite-only beta on August 26, 2026 and raised at a $10 billion valuation a month later. Merit Systems released OpenInstinct the next day: a multi-tenant iMessage agent built on Vercel's Eve framework, with Kernel cloud browsers, Neon Postgres, a Linq-managed iMessage number, a model-blind password vault with browser autofill, Stripe Link purchase approvals and scheduled workers every minute, which is why it requires Vercel Pro. Its README says it is not software intended for production use. Maria Gorskikh, CEO of the YC company Maritime, released open-instinct on October 3: one Firecracker microVM with a Linux desktop per person, texting over Inkbox, apps over Composio, single-use Stripe Link cards, six code-enforced trust tiers and a typed protocol so your agent can negotiate with a friend's agent; Maritime is the default host. A third, Yeachan Heo's Mac menu-bar app, has 20 stars and no licence file. No open source Cue by Manus exists at all.

Launched: August 27, 2026 (Merit Systems); October 3, 2026 (Maria Gorskikh) . Sources: Merit-Systems/OpenInstinct on GitHub ; mariagorskikh/open-instinct on GitHub ; TechCrunch: Instinct raises $1B Series C .

Why people compare OpenInstinct with MausBot

Both are services you deploy and pay vendors for: Vercel Pro, Kernel, Neon and Linq for one; Inkbox, Maritime and Composio for the other. Neither is an app you open.

Both reach you by iMessage, so an iPhone is required, there is no chat window on your computer, and Android users get an SMS line at best.

Merit's approvals are prompt-level: the instructions tell the model to ask before consequential actions, and tools run without a separate approval step; money is gated by Stripe Link.

Maria's open-instinct is five days old, self-declared beta, with quiet hours and the proactive cap still unimplemented, and its default host is the author's own company.

One agent per person, every clone, with no way to run a Claude bot and a Codex bot side by side.

There is no open source Cue: every repo named open-cue or OpenCue is a render-farm manager, a teleprompter or an unrelated meeting tool.

The OpenInstinct column comes from the vendor's own pages and the press cited above, checked on October 8, 2026 . Where the vendor has not said, the cell says so.

OpenInstinct MausBot

License, stars MIT, 422 (Merit); MIT, 241 (Gorskikh); none, 20 (Heo) Apache 2.0, about 4.2k

Shape An iMessage agent service you deploy to Vercel; a Node service and CLI on Maritime microVMs A desktop chat app of bots; iOS and Android companions

Models Any model through Vercel AI Gateway, no local (Merit); Claude by default, any Pi provider incl. Ollama (Gorskikh) Claude, Codex, Grok, and other CLIs, chosen per bot; switch mid-conversation

Before a shell command runs Prompt-level rules, Stripe Link for money (Merit); a policy guard in front of every tool, six trust tiers (Gorskikh) Allow / Deny cards for shell commands and file edits; answer cards for questions

Agents One per person; Gorskikh's talk to other people's agents As many bots as you like, in group rooms

Where it runs Vercel serverless plus Kernel cloud browsers; a Firecracker microVM on Maritime, or your laptop Your own machine; or a cloud desktop per bot

Platforms iMessage, so an iPhone; a web dashboard (Merit); iMessage, SMS, email (Gorskikh) macOS, Windows, Ubuntu; iOS and Android companions

Setup Deploy to Vercel Pro with Kernel, Neon and Linq; or instinct init, Inkbox, Maritime, Composio Download, sign in with your CLI, meet a bot

Price Free code; Vercel Pro from $20 a month plus Kernel, Neon, Linq and model usage; or Inkbox, Maritime from $1 an agent, model usage Free. Model usage on the Claude, ChatGPT, or Grok account you already have.

What MausBot is

MausBot is a free, open-source chat app where every contact is an AI bot with its own model, its own computer, and its own connected apps. Bots run on the claude , codex , and grok CLIs installed on your own machine, with your existing logins, so one bot can be on Claude and the next on ChatGPT. Shell commands and file edits surface as Allow / Deny cards before they run, bots share group rooms and hand work to each other, and your data stays in ~/.openmausbot on your disk. It is published on GitHub under Apache 2.0, with iOS and Android companions, and paid Cloud plans from $15 a month keep bots working with the laptop closed.

What OpenInstinct still does better

Merit Systems OpenInstinct: one-click provisioning of browser, database, storage, iMessage line and model gateway in about five minutes, a model-blind vault that autofills passwords and cards, and real purchases through Stripe Link.

Maria Gorskikh's open-instinct: an agent-to-agent trust network with code-enforced tiers and a written protocol, which nobody else clones, plus a sleeping microVM desktop per person, single-use cards, local models and readable Markdown memory.

Both: a phone number your agent owns, so you text it like a person.

Other OpenInstinct alternatives

The other open-source clones first, then the big agent apps, each with its own comparison page:

Open Dots by Composio, Anil Matcha, CopilotKit : OpenAI launched dots on September 29, 2026 for ChatGPT Pro and Business Premium .

OpenBot by CopilotKit : OpenBot (6,182 stars, 841 forks, MIT) is the most-starred of the open source Grok Bot clones .

Rakazo by Inbox Zero Inc. (Elie Steinbock) : Rakazo (3,418 stars, 599 forks, Apache 2.0) was created two days after Grok Bot launched and is the closest of the clones to MausBot in shape: persistent bots with their own memory, routines and group channels, each on a model you choose through the Pi harness, including Claude Pro or Max and ChatGPT Plus or Pro sign-in, API keys, and Ollama .

OpenMuse by CopilotKit, nanoMuse and twelve smaller repos : Meta's Muse arrived on September 8, 2026 as a single proactive agent in a secure VM .

Every other comparison page: Bops , Hark Pro , Grok Bot , Meta Muse , OpenAI dots , Cue by Manus , Instinct , Open Dots , OpenBot , Rakazo , OpenMuse , OpenClaw , Hermes Agent , Claude Cowork .

Frequently asked questions

Is there an open source Instinct? Yes, two: Merit Systems' OpenInstinct, released August 27, 2026, and Maria Gorskikh's open-instinct, released October 3. Both are MIT and both are iMessage agents you deploy to cloud services rather than apps you install. Is there an open source Cue by Manus? No. As of October 8, 2026, no GitHub project positions itself as an open Cue; the OpenCue name belongs to the Academy Software Foundation's render-farm manager. The closest open-source match for Cue's team of agents with their own computers is MausBot. Does OpenInstinct work on Android? Merit's is iMessage only and needs an iPhone. Gorskikh's gives Android users an SMS line or email. MausBot has native iOS and Android apps. Who makes Instinct? Spear Street Technology, founded by Noah Shinn, not Anthropic or any big lab. It raised $1 billion at a $10 billion valuation on September 28, 2026.

Read more

OpenInstinct vs MausBot: the open source Instinct clones : the full comparison this page summarises.

Instinct AI alternative: open source, no invite needed

Cue by Manus alternative: open source, no invite code

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

---
layout: default
title: "Bops vs MausBot: Orgo's business bots vs the open team"
description: "Bops (bops.bot) is Orgo's Mac app of business-ops bots on OpenAI, each with a cloud computer, email and phone. MausBot is the open source team on any model."
permalink: "/blog/bops-vs-mausbot/"
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

October 7, 2026 · 7 min read · Omkar Satpute and Milind Soni

Bops vs MausBot: Orgo's business bots vs the open team

Bops (bops.bot) is Orgo's Mac app of business-ops bots on OpenAI, each with a cloud computer, email and phone. MausBot is the open source team on any model.

Bops and MausBot are both a team of named bots in a chat app. Bops, from the cloud-computer company Orgo, is Mac only, runs on OpenAI models, gives its bots Orgo cloud computers and, on paid plans, their own email addresses and phone numbers, and is fair source. MausBot is open source under Apache 2.0, runs each bot on the Claude, Codex or Grok account you already have, starts on your own machine, and ships for Mac, Windows and Ubuntu with phone apps.

What is Bops?

Bops launched on October 6, 2026, the work of Nick Vasilescu, co-founder of Orgo, the cloud-computer company that joined YC F26 in September. His launch post put it plainly: "Instinct, Muse, Dot and Grokbot are personal agents. I wanted a business agent. So I built Bops." The name stands for business ops run by bots.

A macOS app for Apple Silicon. A local server runs on your Mac; the bots' computers run in Orgo's cloud.

A roster of named bots: Boppy the chief of staff, Penny for finance, Otto for outbound, Iris for the inbox. Boppy delegates to the specialists and reports back.

A four-screen cloud computer you can watch or take over, shared by all bots on Free and Pro and up to three on Max; on paid plans, phone numbers and email addresses the bots can own, for texts, iMessage and live calls.

Reach a bot by text, call, email, Slack, Telegram or Discord; WhatsApp is listed as coming soon.

OpenAI models only. Using your own Mac runs through the Codex CLI.

Free with $5 of AI credit; Pro $20 a month; Max $200 a month. Credit is billed at what the work costs.

Code on GitHub under the Functional Source License, which the project calls fair source.

It is one day old as this is written: version 0.0.6, two commits, one maintainer, a one-page site. That is not a criticism; MausBot was the same in August. It is a reason to check the facts here against the vendor's pages before you decide.

The same shape, two different bets

Both products reject the single-assistant model that Muse, dots and Instinct chose. Both give you named bots, each with its own computer, memory and connected apps, that hand work to each other and bring decisions back to you. Bops shows an approval card before money moves; MausBot shows one before a shell command or file edit. The differences are underneath, and they are the same three that separate MausBot from every closed agent.

Whose model. Bops runs on OpenAI, and only OpenAI. MausBot runs each bot on the CLI you pick: Claude for one job, Codex for the next, Grok for a third, in the same room. If you pay for more than one of those, Bops uses one of them.

Whose computer. Bops is built by a cloud-computer company, and it shows: the bots work on four-screen Orgo machines in the cloud, and your own Mac is the exception you switch on. MausBot starts on the machine in front of you, where your files and sessions already are, and hands a bot a cloud desktop only when you ask.

Whose code. Bops' code is published, which puts it ahead of Muse, dots, Cue and Grok Bot, and its site calls it open source; its README says fair source, and the Functional Source License is not an open-source licence: it forbids a competing service, and each release only becomes Apache 2.0 after two years. MausBot is Apache 2.0 today, with nothing held back.

Bops vs MausBot

The Bops column comes from bops.bot, the README and licence in its repository, and the launch post, read on October 7, 2026.

Bops MausBot

Launched October 6, 2026, version 0.0.6 August 2026

Made by Orgo (Organic Intelligence, Inc.), a cloud-computer company in YC F26 Supamaus Software, an independent open-source project

Built for Business ops: inbox, pipeline, invoices, reports Any job: code, inbox, research, ops

Price Free with $5 of AI credit once and one shared computer for 10 hours a week; Pro $20 a month; Max $200 a month; credit billed at cost Free. Model usage on the Claude, ChatGPT or Grok account you already have; Cloud plans from $15 a month

Models OpenAI only: GPT-6 Astra, GPT-6.1 Sol, GPT-Live for calls; the Codex CLI for your Mac Claude, Codex, Grok and other CLIs, chosen per bot

Agents A roster of named bots; Boppy, the chief of staff, delegates to specialists As many bots as you like, in group rooms with hand-offs

Each bot's computer A four-screen Orgo cloud computer, shared by all bots on Free and Pro, up to three on Max; your Mac when you allow it Your own machine; or a cloud desktop per bot

Each bot's identity A phone number and email address bots can own: one of each on Pro, up to five on Max, none on Free; text, iMessage, live calls None of its own; bots sign into your apps over OAuth

Reach it from The Mac app, text, iMessage, calls, email, Slack, Telegram, Discord; WhatsApp soon The desktop app, iOS and Android companions, in-app calls

Where your data lives Chat state on your Mac; memory, email, phone and the bots' computers with Bops Cloud and its providers (OpenAI, Orgo, Honcho, Composio, AgentMail, AgentPhone) ~/.openmausbot on your disk; nothing leaves unless you send it

Before it acts Reading runs at once; sending, paying and deleting wait for your OK Allow / Deny cards for shell commands and file edits; answer cards for questions

Connected apps About 1,000 over Composio, scoped per bot 500+ over Composio, OAuth once

Platforms macOS on Apple Silicon only macOS, Windows, Ubuntu; iOS and Android companions

Self-host Yes, with your own OpenAI and Orgo keys Yes; npx openmausbot serve, or the desktop app with no server at all

License FSL-1.1-ALv2, fair source; each release becomes Apache 2.0 two years later Apache 2.0, app and harness

What Bops does better

Three things, and they are the point of the product. Bops bots can have their own phone number and email address, as many as the plan allows, so Otto can text a lead and Iris can answer an inbox as herself; MausBot bots sign into your accounts over OAuth and have no identity of their own. Bops bots work on four-screen cloud computers from the company that builds them, watchable and takeable-over. And Bops starts you with Boppy as chief of staff and a cast of named specialists, where MausBot gives you an empty sidebar and a catalog of teams to import.

What MausBot does that Bops does not

MausBot runs on Windows and Ubuntu as well as the Mac, with iOS and Android companions, and it is free with no AI credit to buy: a bot on Claude costs you nothing beyond the Claude plan you have. Any model per bot, and a Claude bot beside a Codex bot in one room. A local-first default, with the full conversation record in ~/.openmausbot and a harness that listens only on 127.0.0.1 . And an Apache 2.0 licence, which is why it is published on GitHub as MausBot and why reviewers can read every line before the first message is sent.

One bot, any model. Bops runs on OpenAI only.

Which one should you choose?

Choose Bops if you are on a Mac, you want bots that can text and call as themselves from their own numbers, your ops run on inbox, pipeline and invoices, and OpenAI is the model you want. Give it a few weeks of releases first; it is version 0.0.6.

Choose MausBot if you want the same team shape on Windows or Linux or a phone, you pay for Claude or Grok as well as ChatGPT, you want the bots on your own machine by default, or you need a licence a legal team will sign off on. For the rest of the field, see Muse vs Grok Bot vs Dots vs Cue and the alternatives hub .

Frequently asked questions

What is Bops? Bops (bops.bot) is a macOS app from Orgo, the cloud-computer company, launched on October 6, 2026 by co-founder Nick Vasilescu. It runs a team of business-ops bots on OpenAI models, with a four-screen Orgo cloud computer (one shared on Free and Pro, up to three on Max) and, on paid plans, phone numbers and email addresses the bots can own; you reach a bot by text, iMessage, call, email, Slack, Telegram or Discord. Is Bops open source? No, although its site says open source on GitHub. The README calls it fair source: the code is published under the Functional Source License, FSL-1.1-ALv2, under which you may use, modify and self-host it, but not offer a competing service, and each version becomes Apache 2.0 two years after its release. MausBot is Apache 2.0 today, app and harness. Is Bops free? There is a free tier: $5 of AI credit once and one shared cloud computer for ten hours a week, with no email or phone number. Pro is $20 a month and Max is $200, each with that much AI credit every month, billed at what the work costs. MausBot is free; you pay only the model provider you already use. Does Bops run on Windows, or on a phone? Not at launch. Bops is a macOS Apple Silicon app and has no phone app; you reach the bots through messaging channels instead. MausBot runs on macOS, Windows and Ubuntu, with iOS and Android companions. Can Bops use Claude or Grok? No. Bops runs on OpenAI models, and its mode for using your own Mac runs through the Codex CLI. MausBot runs each bot on the Claude, Codex or Grok CLI you choose, and a Claude bot and a Codex bot can share a room. Is MausBot affiliated with Bops or Orgo? No. MausBot is an independent open-source project. Bops and Orgo are products of Organic Intelligence, Inc.

Get started in two minutes

No credits, no signup. Download for macOS , Windows , or Ubuntu , sign in with the CLIs you already have, and meet your first bot. Or read the source on GitHub first. Everything on the features list is free, forever.

Read next

Hark Pro vs MausBot: Adcock’s assistant vs the open team

Hark Pro, from Brett Adcock’s Hark Labs, is one assistant in Hark’s cloud on web, iOS and Android. MausBot is the open source alternative on your own machine.

Meet MausBot: your own team of AI bots, in a chat app

Meet the free, open-source chat app for your own team of AI bots. Bring a supported provider, try a first task, and explore the project and its contributors.

Grok Bot Team Bots vs MausBot teams: shared agents compared

xAI's Grok Bot Team Bots, in public beta since Sept 28, against MausBot's Team plan and free rooms: price for five people, who runs the bot, chats, approvals.

Side by side

Bops alternative: MausBot

A Bops alternative that is open source, runs on any model, and ships for Mac, Windows and Ubuntu with phone apps. Bops is Orgo's Mac-only roster on OpenAI.

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

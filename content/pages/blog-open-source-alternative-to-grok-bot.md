---
layout: default
title: "Open source Grok Bot: MausBot, the free alternative"
description: "An open source Grok Bot alternative: MausBot is a free, Apache 2.0 chat app of AI bots on your own Mac or PC, running on Claude, Codex, and Grok."
permalink: "/blog/open-source-alternative-to-grok-bot/"
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

August 17, 2026 · Updated October 3, 2026 · 5 min read · Omkar Satpute and Milind Soni

Open source Grok Bot: MausBot, the free alternative

An open source Grok Bot alternative: MausBot is a free, Apache 2.0 chat app of AI bots on your own Mac or PC, running on Claude, Codex, and Grok.

MausBot is the open source Grok Bot alternative. It is the same idea, a chat app where every contact is an AI bot with its own model, computer, and apps, but it is free, Apache 2.0 licensed, runs on your own machine, and uses the Claude, Codex, and Grok agents you already pay for. The app itself lives on the home page of the open source Grok Bot alternative ; this post is the comparison.

What is Grok Bot?

Grok Bot is xAI's agent product, launched in beta on August 11, 2026. Instead of one chatbot, you get a roster of bots in a messaging app. Each has its own thread and a cloud computer, signs into your tools, and comes back when a job is done or needs your call.

Runs on Grok, in xAI's cloud, on macOS, Windows, Linux, iOS, and Android.

Bots can share a group chat and hand work to each other.

Show a bot a workflow once and it saves it as a routine.

Included with SuperGrok ($30), Cursor Pro ($20), and higher plans since August 26, 2026; no free tier.

What is MausBot?

MausBot keeps the shape and changes everything underneath. Bots run on the claude , codex , and grok CLIs installed on your computer, with your existing logins. A small harness on 127.0.0.1 owns every agent process, and your data stays in ~/.openmausbot . The code is on GitHub under Apache 2.0.

Every chat in the sidebar is a real agent with its own model, computer, and connected apps.

Try it. This is a live simulation of four bots working in parallel:

Search Inbox 2:21 AM Keeps the mail moving Inbox Release 1:04 AM Published. latest.yml is live, so anyone… Release Chief of Staff 9:12 AM One cause, not three: the mobile signup… Chief of Staff Weekly numbers 6:00 AM Monday's report is ready. Revenue up 4%… Weekly numbers Research Yesterday The split is about trust, not capability… Research Review Yesterday One real problem: the broker resolves an… Review MS Milind Soni Inbox Claude Sonnet 5 Message Inbox +

A simulation. Pick a bot, or type to it. The replies are scripted; the real thing runs on your own machine.

The short version of the comparison

Five rows decide it for most people. For the full fifteen — computers, connected apps, approvals, routines, voice, platforms, and the two things Grok Bot still does better — read Grok Bot vs MausBot .

Grok Bot MausBot

Price Included with SuperGrok ($30), Cursor Pro ($20), and higher plans, with its own weekly usage cap Free. You pay your model providers directly.

License Proprietary Apache 2.0

Models Grok only Claude, Codex, and Grok, per bot

Where agents run xAI's cloud Your machine, on the CLIs you already have

Where your data lives xAI's servers ~/.openmausbot on your disk

What MausBot does

Pick a model per bot

Claude, Codex, and Grok models sit side by side in a provider rail. Give one bot Claude for writing and another Codex for code, and switch mid-conversation.

One bot, any model. Unavailable providers are dimmed with the reason.

Every bot gets a computer

Open the Computer panel and a cloud desktop spins up on its own, with a live preview while the bot works. Or point the bot at your own Mac.

Watch the bot work, or open the desktop and take over.

Bots ask before they act

Shell commands, file edits, and questions surface as cards in the chat. Allow, deny, or answer. It works the same for cloud and local computers.

Questions and approvals land in the chat as cards. Every risky action is a decision you make.

Connected apps

Gmail, Slack, GitHub, Notion, Linear and hundreds more over Composio. OAuth once, and every bot can use them as tools.

Connect an app once. Every bot gets it.

Bots that work as a team

Put bots in a group room. One answers by default, or everyone does, or only the ones you @mention. Bots can ask each other questions and hand off work, and a peer-comms approval card lets you decide who talks to whom. Put the whole room on a call, or export the team for someone else to import.

Bots that talk back

Press the speaker on any reply, or hit call and have a conversation. The bot hears you, narrates its work, and asks for approvals out loud. Bring your own ElevenLabs key.

Hear what ran overnight while you make breakfast.

Which one should you choose?

Choose Grok Bot if you already pay for SuperGrok or Cursor Pro, Grok is the only model you need, and you are fine with your work living in xAI's cloud.

Choose MausBot if you have Claude, Codex, or Grok subscriptions and want to use them, want a different model per bot, need your data on your own machine, or have a security review to pass.

Open source Grok Bot: the short answer

People search for "open source grok bot," "open source version of grok bot," and, from the project's first name, "opengrok bot github." xAI has not open-sourced Grok Bot. MausBot began as OpenGrokBot, an open-source recreation of the Grok Bot shape, and kept the shape while changing everything underneath: your models, your machine, your disk, under Apache 2.0. The old name still reaches the same repository.

Frequently asked questions

Is MausBot really free? Yes. The whole app is Apache 2.0 licensed with no paid tier and no locked features. You only pay the model providers you already use, such as your Claude or Codex subscription. Do I need a Grok subscription? No. MausBot runs on whichever agent CLIs you have installed: claude, codex, or grok. Any one of them is enough to start. Is MausBot affiliated with xAI? No. It is an independent open-source project inspired by Grok Bot. Grok is a trademark of its owner, and MausBot has no token or cryptocurrency of any kind. Where does my data go? Nowhere, unless you send it. Transcripts, keys, and events live in ~/.openmausbot on your own disk, and the harness listens only on 127.0.0.1 . Is Grok Bot open source? Is there an open source Grok Bot? Grok Bot is proprietary. MausBot, formerly OpenGrokBot, is the open-source alternative: the same roster-of-bots shape, running on your own machine on the Claude, Codex, and Grok CLIs you already have, Apache 2.0 licensed on GitHub.

Get started in two minutes

The harness is embedded, so there is nothing else to install. Download for macOS , Windows , or Ubuntu , paste the keys you already have, and meet your first bot. Or read the source on GitHub first. Everything on the features list is free, forever.

Read next

OpenBot by CopilotKit vs MausBot: open source Grok Bots

Open Bot, CopilotKit’s MIT template of AI coworkers, is built for companies and needs a CopilotKit account. MausBot is the open source Grok Bot for a person.

Rakazo vs MausBot: two open source Grok Bots, compared

Rakazo is Inbox Zero’s Apache 2.0 Grok Bot alternative: web, desktop and mobile clients on one self-hosted API with Docker. MausBot installs in a minute.

Grok Bot Team Bots vs MausBot teams: shared agents compared

xAI's Grok Bot Team Bots, in public beta since Sept 28, against MausBot's Team plan and free rooms: price for five people, who runs the bot, chats, approvals.

Side by side

Bops alternative: MausBot

A Bops alternative that is open source, runs on any model, and ships for Mac, Windows and Ubuntu with phone apps. Bops is Orgo's Mac-only roster on OpenAI.

Grok Bot alternative: MausBot

An open source Grok Bot alternative: the same roster-of-bots idea, free and Apache 2.0, on your own machine, on the Claude, Codex and Grok accounts you have.

OpenBot vs MausBot

OpenBot is CopilotKit's MIT template of AI coworkers for companies, and needs a CopilotKit account to start. MausBot is the open source Grok Bot for a person.

Rakazo vs MausBot

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

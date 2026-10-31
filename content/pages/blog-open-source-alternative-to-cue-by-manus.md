---
layout: default
title: "Cue by Manus alternative: open source, no invite code"
description: "Cue by Manus gives each agent its own phone, email, wallet, and computer, behind an invite code. MausBot is the open-source take: your agents, your machine."
permalink: "/blog/open-source-alternative-to-cue-by-manus/"
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

September 28, 2026 · Updated October 2, 2026 · 8 min read · Omkar Satpute and Milind Soni

Cue by Manus alternative: open source, no invite code

Cue by Manus gives each agent its own phone, email, wallet, and computer, behind an invite code. MausBot is the open-source take: your agents, your machine.

MausBot is the open-source alternative to Cue by Manus. Cue is the same idea, several personal agents that each get their own computer and work together in one chat, but it is closed, invite-only, runs in Manus's cloud on an undisclosed model, and keeps your data under Manus's terms. MausBot is free, Apache 2.0 licensed, runs on your own machine, and uses the Claude, Codex, and Grok subscriptions you already pay for. There is no invite code.

What is Cue by Manus?

Cue launched on September 28, 2026, the same day as Manus 2.0 . Where Manus is the workspace you open to research and build, Cue is the app for the rest of your life: "your personal agents, with their own identity." Each agent gets its own email address, its own phone number, a wallet with a budget you set, and a computer in Manus's cloud. It can take your calls while you are in meetings, message people from its own number, pay for things inside its budget, and see a task through on its own machine.

Web, macOS on Apple Silicon, and Android ; iOS is in App Store review and Windows is marked coming soon.

Early access with an invite code. The launch code was reported to be capped at 1,000 users, and members get codes to share.

Free for now. The Play listing says a Plus membership is included at no charge once you are in, which suggests a paid tier later.

Agents collaborate in a group conversation, run automations on a schedule or an event, and remember your preferences per agent.

Scan a QR code at a cafe and an agent reads the menu and orders; you confirm the payment.

Made by Butterfly Effect Pte. Ltd. in Singapore. Tencent is the largest outside shareholder after Meta's $2 billion purchase was blocked by China's NDRC in April.

Why people look for a Cue alternative on day one

You cannot get in. One code and a reported cap of 1,000. Most people who read the launch post will not have an agent by tonight.

Whose cloud, whose model. Cue does not say which model runs your agents, and every one of them lives on a computer in Manus's cloud. If you already pay for Claude, Codex, or Grok, none of that is used.

The data question. Cue runs under Manus's privacy terms. A third-party audit in August graded Manus a B: data in the US and Singapore, a training opt-out that is off by default, retention for conversation logs unspecified. In the same month Manus deleted data generated since December 29, 2025 for users in unnamed jurisdictions. An agent with your email, your phone, and a wallet is a lot to hand to a company that changed hands twice in the last nine months.

Credits. Cue's price is not published, but Manus bills in credits, and a common Manus complaint is credits burning fast, including on failed tasks, with the cost invisible until afterwards. Cue has not said whether Plus will bill the same way.

Closed source. Nothing to read, nothing to self-host, nothing to run air-gapped.

What is MausBot?

MausBot has the same shape as Cue and has had it since August. It is a chat app where every contact is a bot with its own model, its own computer, and its own connected apps, and bots can share a room. The difference is everything underneath. Each bot runs on the claude , codex , or grok CLI installed on your computer, with your existing login. A small harness on 127.0.0.1 owns every agent process, and your data stays in ~/.openmausbot . The code is on GitHub under Apache 2.0.

Every chat in the sidebar is a real agent with its own model, computer, and connected apps.

Try it. This is a live simulation of four bots working in parallel:

Search Inbox 2:21 AM Keeps the mail moving Inbox Release 1:04 AM Published. latest.yml is live, so anyone… Release Chief of Staff 9:12 AM One cause, not three: the mobile signup… Chief of Staff Weekly numbers 6:00 AM Monday's report is ready. Revenue up 4%… Weekly numbers Research Yesterday The split is about trust, not capability… Research Review Yesterday One real problem: the broker resolves an… Review MS Milind Soni Inbox Claude Sonnet 5 Message Inbox +

A simulation. Pick a bot, or type to it. The replies are scripted; the real thing runs on your own machine.

Cue by Manus vs MausBot

Cue's column comes from cue.im, the Manus 2.0 launch post, and the Google Play listing on launch day. Where Manus has not said, the cell says so.

Cue by Manus MausBot

How you get in Invite code, early access; the launch code was reported capped at 1,000 users Download. No invite, no waitlist.

Price Free during early access; a Plus membership is mentioned, price not published Free. You pay your model providers directly.

License Proprietary Apache 2.0, app and harness

Models Not disclosed; Chinese coverage reports the same infrastructure as Manus 2.0 Claude, Codex, and Grok, chosen per bot, plus Cursor, Kimi, OpenCode, Qwen, and other CLIs

Where the agent runs Manus's cloud; each agent gets its own computer there Your machine, on the CLIs you already have; or a cloud desktop per bot

Where your data lives Manus servers in the US and Singapore, under Manus's privacy terms ~/.openmausbot on your disk

Training on your data Opt-out exists in Manus settings and is off by default, per a third-party audit Never. There is no server to train from.

How many agents Several, each with its own identity and memory As many bots as you like, each with its own model, computer, and apps

Agents in one conversation Yes, group collaboration Yes: group rooms with @mentions, hand-offs, and group calls

Before it acts You set review boundaries; it brings work back when a decision needs you Allow / Deny card for every shell command, file edit, and question

Own phone number, email, wallet per agent Yes No

Connected apps Gmail, Trip.com, Oura, MyFitnessPal, YouTube, Instagram, LinkedIn, and more 500+ apps over Composio, OAuth once

Automations Yes, on a schedule or an event Yes, on a schedule or from a webhook

Keeps working with your laptop closed Runs in Manus's cloud, so automations and calls do not depend on your device Only for bots on a cloud computer

Platforms Web, macOS (Apple Silicon), Android; iOS in review; Windows coming soon macOS, Windows, Ubuntu; iOS and Android companions

Self-host or air-gap No Yes

What MausBot does

A team of agents, in rooms

This is the part Cue and MausBot agree on. Put bots in a group room; one answers by default, or everyone does, or only the ones you @mention. Bots ask each other questions and hand off work, a peer-comms approval card lets you decide who talks to whom, and the whole room can join a call. Export the team for someone else to import.

Your models, not an undisclosed one

Cue does not say what runs your agents. MausBot runs whichever agent you already pay for. Claude, Codex, and Grok sit side by side in a provider rail, and the engine list also covers Cursor, Kimi, OpenCode, and Qwen. Give one bot Claude for writing and another Codex for code, and switch mid-conversation.

One bot, any model. Unavailable providers are dimmed with the reason.

A computer per bot, yours or a cloud one

Cue gives every agent a computer in Manus's cloud. MausBot gives every bot a choice: open the Computer panel and a cloud desktop spins up with a live preview and a take-over button, or point the bot at your own machine and it browses as you, with your sessions, from your IP.

Watch the bot work, or open the desktop and take over.

Bots ask before they act

Cue says you set the review boundaries and the agent brings work back when a decision needs you. MausBot draws the line at every risky action: shell commands, file edits, and questions surface as cards in the chat, and nothing runs until you answer. The decision log is yours to read.

Questions and approvals land in the chat as cards. Every risky action is a decision you make.

Connected apps

Gmail, Slack, GitHub, Notion, Linear, and hundreds more over Composio. OAuth once, and every bot can use them as tools. The tokens live on your disk, not in a cloud that a data-retention policy applies to.

Connect an app once. Every bot gets it.

Bots that talk back

Press the speaker on any reply, or hit call and have a conversation. The bot hears you, narrates its work, and asks for approvals out loud. Bring your own ElevenLabs key.

Hear what ran overnight while you make breakfast.

What Cue does that MausBot does not

Four things, and they are the reason Cue exists. Each Cue agent has its own phone number and can answer your calls and call people back; MausBot bots call you inside the app, not third parties. Each Cue agent has its own email address and a wallet with a spending limit; MausBot bots use your accounts over OAuth and have no money. Cue can order from a restaurant's QR code. And Cue agents run in Manus's cloud, so nothing depends on your device being awake; MausBot only does that for bots you have put on a cloud computer. If any of those is the job, Cue is the better tool, once you have a code.

Which one should you choose?

Choose Cue if you have an invite, you want agents that can phone, pay, and email as themselves, you need them running with your phone in your pocket, and you are comfortable with your agents' inboxes and wallets living on Manus's servers.

Choose MausBot if you want the same team-of-agents shape today, you already pay for Claude, Codex, or Grok, you want a different model per bot, you need your data on your own machine, or you have a security review to pass. It is also the one you can read before you run it. For the other closed agents in this category, see our posts on Meta Muse , Grok Bot , and Instinct .

Open Cue, open Manus: the open-source version

Manus has a long-running open-source shadow: "open manus ai," "open manus github," and "open source manus alternative" are established searches, and OpenManus on GitHub is the known clone of the research workspace. Cue is newer, and there is no open Cue from Manus. For Cue's shape in particular, several personal agents with their own computers working together, the open-source answer is MausBot, which has shipped that team shape since August 2026 under Apache 2.0.

Frequently asked questions

What is Cue by Manus? Cue is a consumer app from Manus (Butterfly Effect Pte. Ltd., Singapore) launched on September 28, 2026 alongside Manus 2.0. You get several personal agents, each with its own identity: an email address, a phone number, a wallet with a budget you set, and a computer in Manus's cloud. They can take your calls, order from a QR code at a restaurant, run automations, and work together in one conversation. It is not the Cue meeting-notes app or the heycue.io desktop assistant, which share the name. How do I get a Cue invite code? Cue launched in early access with a launch code, MEETCUE, that Chinese press reported was capped at 1,000 users; accepted users get codes to share. MausBot has no invite. Download it and it runs. Is Cue by Manus free? Free during early access, and the Play Store listing says a Plus membership is included at no charge once you are in, which points to a paid tier later. No price is published. MausBot is free and open source; you only pay the model providers you already use. Is Cue open source? Is there an open-source alternative to Manus? Cue is not open source, and neither is Manus. The closest open-source thing to Cue's shape, several agents that each get a computer and work together, is MausBot, which is Apache 2.0 licensed. For the Manus research-and-build workspace, OpenManus on GitHub is the well-known clone. Where does my Cue data go? Cue runs under Manus's privacy policy. A third-party audit in August 2026 found data stored in the US and Singapore, a training opt-out that is off by default, and an unspecified retention period for conversation logs. In August, Manus deleted data generated since December 29, 2025 for users in unnamed jurisdictions. MausBot keeps everything in ~/.openmausbot on your own disk. Is MausBot affiliated with Manus? No. It is an independent open-source project. Manus and Cue are products of Butterfly Effect Pte. Ltd., and MausBot has no token or cryptocurrency of any kind. Is there an open-source Cue, or an open Manus? Not from Manus. OpenManus on GitHub is the known open-source clone of the Manus workspace. For Cue's shape, a team of personal agents each with its own computer, MausBot is the open-source option, published on GitHub under Apache 2.0.

Get started in two minutes

The harness is embedded, so there is nothing else to install. Download for macOS , Windows , or Ubuntu , sign in with the CLIs you already have, and meet your first bot. No invite code, no card, no credits. Or read the source on GitHub first. Everything on the features list is free, forever.

Read next

Muse vs Grok Bot vs Dots vs Cue: which agent to pick

Meta Muse, xAI Grok Bot, OpenAI dots, and Cue by Manus compared on price, region, models, approvals, and where the agent runs, plus the open-source fifth.

AI agent memory: who keeps it, and can you delete it?

Where OpenAI dots, Meta Muse, Grok Bot, Cue, Instinct, OpenClaw, Hermes, and Claude keep memory, whether you can delete one entry, and what trains the model.

Which AI agent should I use? A five-question decision

Five questions that decide between Meta Muse, Grok Bot, OpenAI dots, Cue, and MausBot: one agent or a team, your plan, your region, your data, and uptime.

Side by side

Cue by Manus alternative: MausBot

A Cue by Manus alternative without the invite code: the open source team-of-agents app, each bot with its own model, computer and apps, on your own machine.

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

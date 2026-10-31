---
layout: default
title: "OpenAI Dots alternative: free, open source, any model"
description: "OpenAI's dots need ChatGPT Pro or Business Premium and run on GPT only. MausBot is the free, open-source alternative: a team of agents on your own machine."
permalink: "/blog/openai-dots-alternative/"
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

September 30, 2026 · Updated October 2, 2026 · 9 min read · Omkar Satpute and Milind Soni

OpenAI Dots alternative: free, open source, any model

OpenAI's dots need ChatGPT Pro or Business Premium and run on GPT only. MausBot is the free, open-source alternative: a team of agents on your own machine.

MausBot is the free, open-source alternative to OpenAI dots. A dot is one always-on agent inside ChatGPT, on GPT only, for Pro and Business Premium subscribers, and not on Pro in the EEA, Switzerland, or the UK. MausBot is a team of agents in a chat app on your own machine, each on the model you pick, using the Claude, ChatGPT, or Grok subscription you already pay for. It is Apache 2.0 licensed and the app is free.

What are OpenAI dots?

Dots are OpenAI's always-on agents, launched at DevDay on September 29, 2026. A dot is not a separate app. It lives inside ChatGPT: you name it, it gets a handle and a character avatar, and it works from its own OpenAI-hosted cloud computer, a sandboxed Linux machine with Chrome that you can open and watch. TechCrunch called it a "bubbly agentic avatar." The Register was blunter: "Think OpenClaw [...] but less open, more contained, and more user-friendly."

One primary dot today. OpenAI says it envisions teams of dots "over time"; extra dots are promised and unpriced.

Runs on GPT-6 Astra. There is no model choice.

Included with ChatGPT Pro and Business Premium. Not on Free, Go, or Plus. Pro excludes the EEA, Switzerland, and the UK .

Uses 4,000+ apps through ChatGPT plugins, runs scheduled tasks, and does read-only "proactive research" in the background.

Reachable in ChatGPT, Slack, and Teams. You can call your dot; it cannot call you yet.

Asks according to Custom Rules you set. Password changes and money transfers are always handed back to you.

Why people look for a dots alternative

The price of admission. Dots are for Pro and Business Premium. Pro is reported to start at $100 a month, and the first month's extended limits are temporary; what the allowance is afterwards, and what a second dot costs, OpenAI has not said. If you are on Plus, you do not get a dot.

Europe. Pro subscribers in the EEA, Switzerland, and the UK are excluded at launch.

One dot, one model. The Hacker News thread kept returning to the same points: platform lock-in, a blurry line between dots, Codex, and ChatGPT Work, and no appetite for paying per dot. If you also pay for Claude or Grok, a dot cannot use them.

It lives on OpenAI's servers. Your dot's memory is kept "for as long as you keep your dot." Per OpenAI's privacy FAQ , you cannot view, edit, or delete individual memories, only reset everything, and disconnecting an app does not delete what the dot already learned from it. On personal plans, training follows your model-improvement setting and can include the dot's actions and connected-app data.

Trust, in launch week. NBC News reported that the day before the launch OpenAI apologised for agents that had accessed non-public health-insurance data in Australia. OpenAI's own privacy and security FAQ says its prompt-injection protections reduce the risk but "do not eliminate" it; the safety post describes the protections themselves.

What is MausBot?

MausBot is where dots say they are heading: a team of agents, not one. It is a chat app where every contact is a bot with its own model, its own computer, and its own connected apps, and bots share rooms. Each bot runs on the claude , codex , or grok CLI installed on your computer, with your existing login. A small harness on 127.0.0.1 owns every agent process, and your data stays in ~/.openmausbot . The code is on GitHub under Apache 2.0.

Every chat in the sidebar is a real agent with its own model, computer, and connected apps.

Try it. This is a live simulation of four bots working in parallel:

Search Inbox 2:21 AM Keeps the mail moving Inbox Release 1:04 AM Published. latest.yml is live, so anyone… Release Chief of Staff 9:12 AM One cause, not three: the mobile signup… Chief of Staff Weekly numbers 6:00 AM Monday's report is ready. Revenue up 4%… Weekly numbers Research Yesterday The split is about trust, not capability… Research Review Yesterday One real problem: the broker resolves an… Review MS Milind Soni Inbox Claude Sonnet 5 Message Inbox +

A simulation. Pick a bot, or type to it. The replies are scripted; the real thing runs on your own machine.

OpenAI dots vs MausBot

The dots column comes from OpenAI's launch post, its safety post, and its help-centre articles. Plan prices are as reported by the press; OpenAI's post names plans, not prices.

OpenAI dots MausBot

Price Included with ChatGPT Pro (from $100 a month, as reported) and Business Premium; not on Free, Go, or Plus Free. You pay your model providers directly.

License Closed; no open-source component announced Apache 2.0, app and harness

Where you can use it Pro excludes the EEA, Switzerland, and the UK; 18+ Anywhere

Models GPT-6 Astra only Claude, Codex, and Grok, chosen per bot, plus Cursor, Kimi, OpenCode, Qwen, and other CLIs

How many agents One primary dot today; more dots and teams of dots are planned As many bots as you like, each with its own model, computer, and apps

Agents in one conversation A dot can delegate to other agents; no dot-to-dot group chats Group rooms with @mentions, hand-offs, and group calls

Where the agent runs An OpenAI-hosted cloud computer per dot; local control is optional and off by default Your machine, on the CLIs you already have; or a cloud desktop per bot

Where your data lives OpenAI's servers, kept for as long as you keep your dot ~/.openmausbot on your disk

Training on your data On personal plans it follows your model-improvement setting; off by default on Business, Enterprise, and Edu MausBot does not train on it; the local app has no server. Your model provider's own setting applies.

Who holds the memory OpenAI; no per-memory view, edit, or delete, only a full reset You; the full conversation record is on your own disk

Approvals Custom Rules with four behaviours, plus an auto-review check Allow / Deny cards for shell commands and file edits, answer cards for questions

Connected apps 4,000+ through ChatGPT plugins 500+ over Composio, OAuth once

Scheduled routines Yes, plus read-only proactive research Yes, on a schedule or from a webhook

Keeps working with your laptop closed Yes For bots on a cloud computer, or the whole team with Pro

Voice You can call your dot; it cannot call you yet Bots read replies aloud, or you call them

Platforms Set up in the ChatGPT desktop app or desktop web; chat from ChatGPT, Slack, and Teams macOS, Windows, Ubuntu; iOS and Android companions

Self-host or air-gap No Yes

What MausBot does

Every model, your pick

A dot is GPT-6 Astra. An MausBot bot is whichever agent you already pay for. Claude, Codex, and Grok sit side by side in a provider rail, and the engine list also covers Cursor, Kimi, OpenCode, and Qwen. If ChatGPT is what you have, the codex CLI signs in with that account and your bots run on it. Give another bot Claude for writing, and switch mid-conversation.

One bot, any model. Unavailable providers are dimmed with the reason.

A team today, not over time

OpenAI envisions teams of dots. MausBot ships them. Put bots in a group room; one answers by default, or everyone does, or only the ones you @mention. Bots ask each other questions and hand off work, a peer-comms approval card lets you decide who talks to whom, and the whole room can join a call. There is no price per bot.

A computer per bot, yours or a cloud one

A dot works from OpenAI's cloud computer and reaches your own machine only if you switch that on. MausBot starts on your machine, where your files and sessions already are, and gives any bot a cloud desktop with a live preview and a take-over button when you want it out of your way.

Watch the bot work, or open the desktop and take over.

Bots ask before they act

Dots have Custom Rules: act without asking, act if pre-approved, ask first, or hand off. MausBot's default is simpler to reason about. Shell commands, file edits, and questions surface as cards in the chat, and nothing runs until you answer.

Questions and approvals land in the chat as cards. Every risky action is a decision you make.

Connected apps, tokens on your disk

Gmail, Slack, GitHub, Notion, Linear, and hundreds more over Composio. OAuth once, and every bot can use them as tools. What a bot learns from an app stays in the conversation record on your own disk, not on a server you cannot inspect.

Connect an app once. Every bot gets it.

Bots that talk back

Press the speaker on any reply, or hit call and have a conversation. The bot hears you, narrates its work, and asks for approvals out loud.

Hear what ran overnight while you make breakfast.

The always-on question

The real advantage of a dot is that it never sleeps: it lives in OpenAI's cloud, so it works with your laptop shut. MausBot is free because it runs on your computer, and a closed computer runs nothing. There are three ways to close that gap. Put one bot on a cloud desktop. Run the whole thing on a box you own with npx openmausbot serve . Or take Pro , which is $49 a month for a personal always-on cloud workspace that runs your bots and their scheduled tasks around the clock, with cloud computers and voice included. You still bring your own Claude or ChatGPT account, so there is no second model bill from us.

What dots do better

Four things, and they are real. A dot shares memory with ChatGPT and app permissions with ChatGPT, ChatGPT Work, and Codex, so if you live in ChatGPT it already knows you. It reaches 4,000+ apps, about eight times what MausBot connects to. It answers you in Slack and Teams, where MausBot is its own app with iOS and Android companions. And its background research is read-only, a limit OpenAI says it enforces in code. If you are a Pro subscriber outside Europe and one GPT agent is what you want, a dot is the better tool today.

Other dots alternatives

Meta Muse is the product the press measures dots against: one consumer agent with a free tier, US and Canada only. See our comparison .

Grok Bot from xAI is a roster of named bots on one shared cloud computer, Grok only, from a SuperGrok ($30) or Cursor Pro ($20) plan at list prices. See Grok Bot vs MausBot .

Cue by Manus gives each agent its own phone number, email, and wallet, behind an invite code. See our comparison .

OpenClaw and Hermes Agent are the open, self-hosted agents you reach through chat apps. You host a gateway yourself or pay a host to run it; we compared the hosts for OpenClaw and Hermes .

Which one should you choose?

Choose dots if you already pay for ChatGPT Pro or Business Premium, you are outside the EEA, Switzerland, and the UK, GPT is the only model you need, and you want one agent that lives where you already work.

Choose MausBot if you are on Plus or no plan at all, you are in Europe, you want a team of agents and not one, you want Claude or Grok alongside GPT, you need your data on your own disk, or you have a security review to pass. It is free, and you can read every line before you run it.

Open dots: the open-source version people are searching for

Within a day of DevDay, "opendots github" and "open dots ai" appeared in search, and a handful of GitHub repositories took the Open Dots name. OpenAI has not released any part of dots as open source. If what you want is an open dot, an always-on agent with its own computer whose code you can read, MausBot has shipped that shape since August 2026, with a team of them rather than one, and it runs on the ChatGPT account you already have through the codex CLI.

Frequently asked questions

What are OpenAI dots? Dots are always-on agents inside ChatGPT, launched on September 29, 2026 at OpenAI's DevDay. You name your dot and pick an avatar, it gets a handle, and it works from its own OpenAI-hosted cloud computer: it runs scheduled tasks, does read-only research in the background, uses your connected apps, and answers you in ChatGPT, Slack, or Teams. It runs on GPT-6 Astra. Are OpenAI dots free? No. Your first dot is included at no extra cost, but only on ChatGPT Pro and Business Premium, with a beta for Enterprise, Edu, and Healthcare that an admin has to enable. Free, Go, and Plus do not get one. Pro is reported by NBC News to start at $100 a month. MausBot is free and open source; you only pay the model provider you already use. Are dots available in the UK and EU? Not on ChatGPT Pro: OpenAI's help page excludes the European Economic Area, Switzerland, and the United Kingdom for Pro. Business Premium covers all ChatGPT regions. MausBot has no region check. Is OpenAI dots open source? No. OpenAI's launch post mentions no open-source component. A few community clones appeared on GitHub within a day of launch; we have not tested them. MausBot is Apache 2.0 licensed, app and harness, and has shipped since August 2026. Can I use my ChatGPT subscription in MausBot? Yes. MausBot runs bots on the codex CLI, which signs in with your ChatGPT account, and on the claude and grok CLIs the same way. You use the plan you already pay for; MausBot adds no charge and no second quota. Is MausBot affiliated with OpenAI? No. It is an independent open-source project. ChatGPT, Codex, and dots are products of OpenAI, and MausBot has no token or cryptocurrency of any kind. Is there an open-source version of OpenAI dots? Not from OpenAI. Several community projects named Open Dots appeared on GitHub within a day of launch; we have not tested them. MausBot is the open-source agent app with the same shape, a team of always-on agents on your own machine, published on GitHub as MausBot under Apache 2.0.

Get started in two minutes

The harness is embedded, so there is nothing else to install. Download for macOS , Windows , or Ubuntu , sign in with the CLIs you already have, and meet your first bot. No ChatGPT Pro plan, no region check, no price per bot. Or read the source on GitHub first. Everything on the features list is free, forever.

Read next

Open Dots vs MausBot: three open source dots, one app

Composio’s open-dot, Anil Matcha’s Open Dots and CopilotKit’s OpenDots all claim to be the open source OpenAI dots. What each is, and how MausBot compares.

Meta Muse vs OpenAI dots: the two one-agent products

Meta Muse and OpenAI dots compared on price, region, model, where the agent runs, memory, training, and phone calls, plus the open-source third option.

Muse vs Grok Bot vs Dots vs Cue: which agent to pick

Meta Muse, xAI Grok Bot, OpenAI dots, and Cue by Manus compared on price, region, models, approvals, and where the agent runs, plus the open-source fifth.

Side by side

Hark Pro alternative: MausBot

A Hark Pro alternative that is open source and runs on your own computer: a team of bots on any model, free under Apache 2.0, on Mac, Windows and Ubuntu.

OpenAI dots alternative: MausBot

An OpenAI dots alternative with no Pro plan and no region lock: a free, open source team of agents on your own machine, on the ChatGPT account you have.

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

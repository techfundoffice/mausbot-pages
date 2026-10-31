---
layout: default
title: "Meta Muse alternative: open source, runs on your machine"
description: "A Meta Muse alternative that is open source, works outside the US, and keeps your data off Meta's servers, on the Claude, Codex, or Grok login you already have."
permalink: "/blog/open-source-alternative-to-meta-muse/"
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

September 22, 2026 · Updated October 2, 2026 · 8 min read · Omkar Satpute and Milind Soni

Meta Muse alternative: open source, runs on your machine

A Meta Muse alternative that is open source, works outside the US, and keeps your data off Meta's servers, on the Claude, Codex, or Grok login you already have.

MausBot is the open-source alternative to Meta Muse. Muse is one agent that lives in Meta's cloud, in the US and Canada only, on Meta's model, with a card on file. MausBot is a team of agents that lives on your own machine, anywhere in the world, on the Claude, Codex, and Grok subscriptions you already pay for. It is free and Apache 2.0 licensed.

What is Meta Muse?

Muse is the personal AI agent from Meta Superintelligence Labs, launched on September 8, 2026. You give it a goal and it does the work: it books the table, tracks the price, reads the email thread, and pings you when it needs a decision. It runs on Meta's own Muse Spark model, in a Linux virtual machine in Meta's cloud, with a browser it can drive.

iOS, Android, web, and inside WhatsApp; a Mac app followed on September 17.

United States and Canada only, 18 and over, with a payment card at signup.

Free tier metered in weekly tokens; paid Power and Maximum tiers.

One agent per person. It spawns its own subagents, but you cannot create a second Muse with a different job.

Keeps working after you close the app, and calls US businesses for you.

It topped the US App Store within ten days. It also collected the loudest privacy backlash of any agent launch this year: The Verge found it inferring a family member's location from Amazon shipping data , Reuters reported Meta staff flagging that it routed around its own guardrails during testing, and on September 20 Amazon blocked it from shopping on Amazon.com.

Why people look for a Muse alternative

The reasons show up in the same order in every thread we read.

It is Meta. Muse asks for your Gmail, your calendar, your bank via Plaid, and on the Mac your files and messages. In the Hacker News launch thread, the most upvoted comments were not about features. They were about who holds the keys.

It is cloud only. The Mac app does not run the agent on your Mac. A VM in Meta's data center reaches into your Mac. Meta's own security post is honest that Meta can access VM data today and that a locked-down "Confidential VM" is coming later.

It is US and Canada only. "Is Muse available in India" and "Muse UK" are among the top searches about it.

One model, one agent. You get Muse Spark and one Muse. If you already pay for Claude or Codex, none of that is used, and you cannot give one agent your inbox and another your repos.

Training is opt-out. Sanitized sessions are used to improve the model unless you turn it off.

What is MausBot?

MausBot keeps the promise, an agent that does the work while you do something else, and changes everything underneath. It is a chat app where every contact is a bot. Each bot runs on the claude , codex , or grok CLI installed on your computer, with your existing login. A small harness on 127.0.0.1 owns every agent process, and your data stays in ~/.openmausbot . The code is on GitHub under Apache 2.0.

Every chat in the sidebar is a real agent with its own model, computer, and connected apps.

Try it. This is a live simulation of four bots working in parallel:

Search Inbox 2:21 AM Keeps the mail moving Inbox Release 1:04 AM Published. latest.yml is live, so anyone… Release Chief of Staff 9:12 AM One cause, not three: the mobile signup… Chief of Staff Weekly numbers 6:00 AM Monday's report is ready. Revenue up 4%… Weekly numbers Research Yesterday The split is about trust, not capability… Research Review Yesterday One real problem: the broker resolves an… Review MS Milind Soni Inbox Claude Sonnet 5 Message Inbox +

A simulation. Pick a bot, or type to it. The replies are scripted; the real thing runs on your own machine.

Meta Muse vs MausBot

Muse's side comes from Meta's launch post, its security post, and the press coverage of its plans. Where Meta has not published a number, the cell says so.

Meta Muse MausBot

Price Free tier with a weekly token quota; paid Power and Maximum plans. A payment card is required at signup. Free. You pay your model providers directly.

License Proprietary. Meta says open weights for the Spark model are on the roadmap; the agent is not. Apache 2.0, app and harness

Where you can use it United States and Canada only, 18+ Anywhere

Models Muse Spark only Claude, Codex, and Grok, chosen per bot, plus Cursor, Kimi, OpenCode, Qwen, and other CLIs

Where the agent runs A Meta cloud VM. The Mac app reaches into your Mac from that VM. Your machine, on the CLIs you already have; or a cloud desktop per bot

Where your data lives Meta's servers. Meta can access VM data under its operational policy today. ~/.openmausbot on your disk

Training on your sessions On by default, opt-out Never. There is no server to train from.

How many agents One Muse; it spawns hidden subagents As many bots as you like, each with its own model, computer, and apps

Approvals Scoped permissions; every purchase needs a human Allow / Deny card for every shell command, file edit, and question

Connected apps Gmail, Calendar, Instagram, WhatsApp, OpenTable, Spotify, Plaid, and more 500+ apps over Composio, OAuth once

Scheduled routines Yes, goals and background tasks Yes, on a schedule or from a webhook

Keeps working with your laptop closed Yes Only for bots on a cloud computer

Phone calls to businesses Yes, US businesses, in beta No. Bots talk to you on a call, not to third parties.

Platforms iOS, Android, web, WhatsApp, macOS macOS, Windows, Ubuntu; iOS and Android companions

Self-host or air-gap No Yes

What MausBot does

Pick a model per bot

Muse is Muse Spark. MausBot is whichever agent you already pay for. Claude, Codex, and Grok sit side by side in a provider rail, and the engine list also covers Cursor, Kimi, OpenCode, and Qwen. Give one bot Claude for writing and another Codex for code, and switch mid-conversation.

One bot, any model. Unavailable providers are dimmed with the reason.

A computer per bot, yours or a cloud one

Muse gives you one VM in Meta's cloud. In MausBot, open the Computer panel and a cloud desktop spins up for that bot, with a live preview while it works. Or point the bot at your own machine and skip the cloud entirely.

Watch the bot work, or open the desktop and take over.

Bots ask before they act

Shell commands, file edits, and questions surface as cards in the chat. Allow, deny, or answer. Nothing runs on your machine because a web page told the bot to. Muse gates purchases the same way; MausBot gates every risky action, and the decision log is yours to read.

Questions and approvals land in the chat as cards. Every risky action is a decision you make.

Connected apps

Gmail, Slack, GitHub, Notion, Linear, and hundreds more over Composio. OAuth once, and every bot can use them as tools. The tokens live on your disk, not on a server that a data-sharing policy applies to.

Connect an app once. Every bot gets it.

A team, not a single Muse

The most common feature request in Muse reviews is a second agent. MausBot starts there. Put bots in a group room; one answers by default, or everyone does, or only the ones you @mention. Bots can ask each other questions and hand off work, and a peer-comms approval card lets you decide who talks to whom.

Bots that talk back

Press the speaker on any reply, or hit call and have a conversation. The bot hears you, narrates its work, and asks for approvals out loud. Bring your own ElevenLabs key.

Hear what ran overnight while you make breakfast.

What Muse still does better

Two things, and they are real. Muse keeps working after you close the app on every task, because the agent never lived on your device; MausBot only does that for bots you have put on a cloud computer. And Muse can phone a US restaurant or a customer-service line on your behalf; MausBot bots call you, not third parties. If either of those is the job, Muse is the better tool today.

Other Meta Muse alternatives

MausBot is not the only option, and the right one depends on what you want to own.

OpenClaw is the most-starred self-hosted agent, run from a terminal and reached over messaging apps. Powerful, and the reason a lot of people wanted a GUI with an approval gate.

Hermes Agent from Nous is a self-hosted agent with a desktop app, closer to a single assistant than a team.

Grok Bot from xAI is the closest product to MausBot in shape, a roster of bots in a messaging app, but it is Grok only, cloud only, and needs a SuperGrok or Cursor Pro plan or higher. We compared them line by line in Grok Bot vs MausBot .

Claude Cowork from Anthropic is a macOS app for giving Claude your files and apps. One model, no team, no Windows.

Which one should you choose?

Choose Meta Muse if you are in the US, you want one assistant that needs zero setup, you need it to keep going with your phone in your pocket, and you are comfortable with Meta holding the accounts it works in.

Choose MausBot if you are anywhere else, you already pay for Claude, Codex, or Grok, you want more than one agent with more than one job, you need your data on your own machine, or you have a security review to pass.

For Muse against the other new agents, see Meta Muse vs OpenAI dots and the five-way Muse vs Grok Bot vs Dots vs Cue ; for a decision in five questions, Which AI agent should I use? .

Open Muse: what people mean by it

Searches for "open muse," "openmuse bot," and "open muse github" all ask the same question: is there an open-source Muse? There is no open Muse from Meta; the agent is closed, and the only openness Meta has mentioned is a future open-weights release of the Spark model, which would not make the agent self-hostable. What people want when they type it is an agent shaped like Muse whose code they can read and whose data they keep. That is what MausBot is, and its GitHub repository is the "open muse github" result in practice: a chat app of agents with their own computers, under Apache 2.0, on the models you already pay for.

Frequently asked questions

Is Meta Muse open source? No. The Muse app, the agent harness, and the Muse Spark model are all proprietary. Meta has said an open-weights release of Spark is on its roadmap, with no date. Even if the weights ship, the agent product will still run only in Meta's cloud. MausBot is Apache 2.0 licensed end to end. Is Meta Muse available in India, the UK, or the EU? Not as of October 2026. Muse launched in the United States and added Canada on September 18, 2026, for people 18 and over; no other country has a date. MausBot has no region check: it runs wherever your Claude, Codex, or Grok login works. Is Meta Muse free? There is a free tier, metered by a weekly token quota, and Meta asks for a payment card at signup. Testers have reported burning most of the free quota in a day of heavy use. MausBot has no quota and no card; you keep paying your model providers exactly what you pay them now. Does MausBot need Meta or any Meta account? No. MausBot has no relationship with Meta and never contacts Meta's servers. You sign in with the agent CLIs you already use. Can MausBot make phone calls like Muse? Not to businesses. A bot can talk to you on a voice call inside the app, read replies aloud, and ask for approvals out loud. Calling a restaurant on your behalf is something Muse does and MausBot does not. Where does my data go? Nowhere, unless you send it. Transcripts, keys, and events live in ~/.openmausbot on your own disk, and the harness listens only on 127.0.0.1 . Nothing is used for training because there is nothing to train from. Is there an open-source Muse, or an "open muse"? Not from Meta. Muse is closed, and the only open component on Meta's roadmap is the Spark model's weights, with no date. The closest open-source Muse in shape is MausBot: the same personal-agent idea, with several agents instead of one, running on your own machine under Apache 2.0.

Get started in two minutes

The harness is embedded, so there is nothing else to install. Download for macOS , Windows , or Ubuntu , sign in with the CLIs you already have, and meet your first bot. No card, no waitlist, no region check. Or read the source on GitHub first. Everything on the features list is free, forever.

Read next

OpenMuse vs MausBot: every open source Muse, compared

Fifteen GitHub repos call themselves OpenMuse. CopilotKit’s template and nanoMuse are the two that matter. What each is, and how the open source Muse compares.

Muse for Small Business vs a team of bots you own

What Meta's Muse for Small Business is, what it is not, the trust questions a business has to ask, and how the same five jobs run on a team of bots you own.

Meta Muse vs OpenAI dots: the two one-agent products

Meta Muse and OpenAI dots compared on price, region, model, where the agent runs, memory, training, and phone calls, plus the open-source third option.

Side by side

Hark Pro alternative: MausBot

A Hark Pro alternative that is open source and runs on your own computer: a team of bots on any model, free under Apache 2.0, on Mac, Windows and Ubuntu.

Meta Muse alternative: MausBot

A Meta Muse alternative that is open source, works outside the US and Canada, and keeps your data off Meta's servers: a team of agents on your own machine.

OpenMuse vs MausBot

Fifteen GitHub repos call themselves OpenMuse. The two that matter, CopilotKit's template and nanoMuse, compared with MausBot on licence, models and approvals.

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

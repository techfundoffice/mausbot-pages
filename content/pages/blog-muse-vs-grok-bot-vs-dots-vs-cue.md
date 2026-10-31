---
layout: default
title: "Muse vs Grok Bot vs Dots vs Cue: which agent to pick"
description: "Meta Muse, xAI Grok Bot, OpenAI dots, and Cue by Manus compared on price, region, models, approvals, and where the agent runs, plus the open-source fifth."
permalink: "/blog/muse-vs-grok-bot-vs-dots-vs-cue/"
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

October 2, 2026 · 8 min read · Omkar Satpute and Milind Soni

Muse vs Grok Bot vs Dots vs Cue: which agent to pick

Meta Muse, xAI Grok Bot, OpenAI dots, and Cue by Manus compared on price, region, models, approvals, and where the agent runs, plus the open-source fifth.

Four big companies shipped a personal agent in seven weeks. Meta Muse is one consumer assistant, free to start, US and Canada only. Grok Bot is a roster of bots on one shared cloud computer, from a $20 or $30 plan, Grok only. OpenAI dots are one always-on agent inside ChatGPT, for Pro and Business Premium, GPT only, not on Pro in the EEA, Switzerland, or the UK. Cue by Manus gives several agents their own phone, email, and wallet, behind an invite code. MausBot is the open-source fifth: a team of agents on your own machine, on the Claude, ChatGPT, or Grok plan you already pay for, free.

Five agents, two shapes

Every one of these does the same job: you describe an outcome, the agent gets a computer and your apps, and it comes back when it needs you. They split on one design question. Muse and dots give you one agent and hide the rest. Grok Bot, Cue, and MausBot give you a team : named agents you can put in a room together. Once you know which shape you want, half the table below stops mattering.

Meta Muse

Muse launched on September 8 from Meta Superintelligence Labs. One agent on Meta's Muse Spark model, in a Linux VM in Meta's cloud, with a browser it can drive. It books the table, runs goals in the background, and phones US businesses for you. iOS, Android, web, WhatsApp, and a Mac app that is a client for the cloud VM. US and Canada only, 18 and over, card at signup, free tier metered in weekly tokens; Power is $20 a month and Maximum $100. It topped the US App Store within ten days and drew a sharp privacy backlash: Meta's own security post says Meta can access VM data today, and Amazon blocked it from shopping on September 20. Our full comparison: Meta Muse alternative .

xAI Grok Bot

Grok Bot has been in beta since August 11 and is the most mature of the four. A messaging app where every contact is a named bot; group chats of two to six bots with @mentions; routines, up to 50 per bot; a marketplace of bot templates; "Teach a task" by screen recording; and, since September 28, Team Bots in public beta for Teams and Enterprise. Grok only. All bots share one cloud computer per account, and xAI's docs say not to use separate bots as a security boundary. Since August 26 it comes with SuperGrok ($30) and Cursor Pro ($20) and up, with its own weekly allowance that xAI does not publish. It ships on macOS, Windows, Linux, iOS, and Android . Our full comparison: Grok Bot vs MausBot .

OpenAI dots

Dots launched at DevDay on September 29. A dot is not an app; it is an always-on agent inside ChatGPT, on GPT-6 Astra, with its own OpenAI cloud computer. It uses 4,000+ apps through ChatGPT plugins, runs scheduled tasks and read-only background research, and answers you in ChatGPT, Slack, and Teams. One primary dot today; OpenAI says it envisions teams of dots over time. Included with ChatGPT Pro and Business Premium, plus an admin-enabled beta for Enterprise, Edu, and Healthcare, and Pro excludes the EEA, Switzerland, and the UK . Its memory is kept for as long as you keep your dot, with no way to delete a single memory. Our full comparison: OpenAI dots alternative .

Cue by Manus

Cue launched on September 28 alongside Manus 2.0 , from Butterfly Effect in Singapore. Several personal agents, each with its own identity: an email address, a phone number that can take and make calls, a wallet with a budget you set, and a computer in Manus's cloud. Agents collaborate in one conversation, and one can order from a restaurant's QR code. Invite only, with a launch code reported capped at 1,000 users; free during early access with a Plus tier implied; model undisclosed. Web, macOS on Apple Silicon, and Android, with iOS in review. Our full comparison: Cue by Manus alternative .

MausBot

MausBot, published on GitHub as MausBot, has had the team shape since August. It is a chat app where every contact is a bot with its own model, its own computer, and its own connected apps. Bots run on the claude , codex , or grok CLI installed on your computer, with your existing login, so one bot can be on your Claude plan and the next on your ChatGPT plan. A small harness on 127.0.0.1 owns every agent process and your data stays in ~/.openmausbot . The app is free and Apache 2.0 licensed; Pro , $49 a month, adds an always-on cloud workspace so the team keeps working with your laptop shut.

Every chat in the sidebar is a real agent with its own model, computer, and connected apps.

Side by side

Each column comes from that product's own launch post, docs, or store listing. Where a company has not said, the cell says so. Plan prices are list prices as reported where the company names plans but not numbers.

Meta Muse Grok Bot OpenAI dots Cue by Manus MausBot

Launched Sept 8, 2026 Aug 11, 2026, still beta Sept 29, 2026, gradual rollout Sept 28, 2026, early access Aug 2026

Price Free tier with a weekly token quota; paid Power and Maximum tiers; card at signup Included with SuperGrok ($30), Cursor Pro ($20), and up; no free tier Included with ChatGPT Pro (reported from $100) and Business Premium; not on Free, Go, or Plus Free in early access; a Plus membership is mentioned, price not published Free. Pro is $49 a month for an always-on cloud workspace.

How you get in Sign up, US and Canada only, 18+ Subscribe to a qualifying plan Pro or Business Premium account; Pro excludes the EEA, Switzerland, and the UK Invite code; the launch code was reported capped at 1,000 users Download

Models Muse Spark only Grok only GPT-6 Astra only Not disclosed Claude, Codex, Grok, and more, chosen per bot

How many agents One, with hidden subagents A roster of named bots One primary dot today; teams of dots planned Several, each with its own identity Unlimited bots

Agents in one conversation No Yes, 2 to 6 bots with @mentions Delegation only; no dot-to-dot group chats Yes, group collaboration Yes, group rooms with @mentions, hand-offs, and group calls

Where the agent runs A Meta cloud VM; the Mac app is a client One shared cloud computer per account; local commands with approval An OpenAI cloud computer per dot; local control optional, off by default A Manus cloud computer per agent Your machine; or a cloud desktop per bot

Where your data lives Meta's servers; Meta can access VM data today xAI's servers OpenAI's servers, for as long as you keep your dot Manus's cloud; US and Singapore per a third-party audit ~/.openmausbot on your disk

Training on your data On by default, opt-out Not covered in this review Personal plans follow your model-improvement setting; off by default on business plans Opt-out exists in Manus settings and is off by default, per a third-party audit MausBot does not train on it; the local app has no server. Your model provider's own setting applies.

Before it acts Scoped permissions; every purchase needs a human Pulls you in for judgment calls; local commands need approval Custom Rules: act, act if pre-approved, ask, or hand off; plus auto-review You set review boundaries; it brings decisions back to you Allow / Deny cards for shell commands and file edits, answer cards for questions

Connected apps Gmail, Calendar, Instagram, WhatsApp, OpenTable, Spotify, Plaid, and more Signs into your tools 4,000+ through ChatGPT plugins Gmail, Trip.com, Oura, YouTube, Instagram, LinkedIn, and more 500+ over Composio, OAuth once

Routines Goals and background tasks Up to 50 per bot Scheduled tasks plus read-only proactive research Automations on a schedule or an event On a schedule or from a webhook

Keeps working with your laptop closed Yes Yes Yes Runs in Manus's cloud Bots on a cloud computer, or the whole team with Pro

Phone calls Calls US businesses, in beta Live voice chat, rolling out on mobile You can call your dot; it cannot call you yet Each agent has its own number and can take and make calls Bots read replies aloud, or you call them in the app

Platforms iOS, Android, web, WhatsApp, macOS macOS, Windows, Linux, iOS, Android Inside ChatGPT: desktop app or desktop web; Slack and Teams Web, macOS (Apple Silicon), Android; iOS in review; Windows coming macOS, Windows, Ubuntu; iOS and Android companions

Open source No No No No Yes, Apache 2.0

Who each one is for

Meta Muse is for someone in the US or Canada who wants one assistant with no setup, needs it to phone a restaurant, and is fine with Meta holding the accounts it works in. The cost is one agent, one model, two countries, and the trust question.

Grok Bot is for someone who already pays for SuperGrok or Cursor, wants a roster of bots today, and wants a marketplace and teach-by-recording. The cost is Grok only, one shared computer for every bot, and a weekly allowance nobody will tell you the size of.

OpenAI dots are for a ChatGPT Pro subscriber outside the EEA, Switzerland, and the UK, or a Business Premium subscriber anywhere ChatGPT is sold, who lives in ChatGPT, Slack, or Teams and wants one agent that already knows them. The cost is a Pro plan, reported from $100 a month, GPT only, and memory you cannot edit.

Cue by Manus is for someone with an invite who wants agents that can phone, pay, and email as themselves. The cost is a closed model, Manus's cloud, and a paid Plus tier once early access ends.

MausBot is for someone who already pays for Claude, ChatGPT, or Grok, wants a team of agents on more than one model, wants them to ask before they act, needs their data on their own disk, or has a security review to pass. The cost is that the free app runs on your computer, so a closed laptop runs nothing unless you put a bot on a cloud computer or take Pro.

What changes when the fifth one is open source

Put the feature table aside for a moment. The four closed agents differ in price and polish, but they share three properties, and the open-source one inverts all three.

The model is a vendor. Muse is Meta's model, Grok Bot is Grok, dots are GPT, Cue does not say. Whichever you choose, you have chosen a lab, and when a better model ships somewhere else your agent cannot use it. In MausBot the model is a setting on each bot. A bot that reads your inbox on Claude today can read it on Codex tomorrow, and the two can sit in the same room.

The computer is theirs. Every closed agent works from a machine in its maker's cloud, which is why they all keep going with your phone in your pocket, and why none of them can see the browser session you are logged into right now. MausBot starts on the machine in front of you, where your files and cookies already are, and hands any bot a cloud desktop only when you ask for one.

You cannot read it. Meta's security post is unusually candid and still ends in "trust us." OpenAI's says its injection defences do not eliminate the risk. Manus and xAI publish less. With an Apache 2.0 codebase, the approval gate, the harness on 127.0.0.1 , and the folder your data sits in are all things a reviewer can open before the first message is sent. That is the row that decides it for anyone with a security review to pass, and it is the one row no closed agent can ever match.

Try it. This is a live simulation of four bots working in parallel:

Search Inbox 2:21 AM Keeps the mail moving Inbox Release 1:04 AM Published. latest.yml is live, so anyone… Release Chief of Staff 9:12 AM One cause, not three: the mobile signup… Chief of Staff Weekly numbers 6:00 AM Monday's report is ready. Revenue up 4%… Weekly numbers Research Yesterday The split is about trust, not capability… Research Review Yesterday One real problem: the broker resolves an… Review MS Milind Soni Inbox Claude Sonnet 5 Message Inbox +

A simulation. Pick a bot, or type to it. The replies are scripted; the real thing runs on your own machine.

Frequently asked questions

Which personal AI agent is cheapest? MausBot, which is free and open source; the only cost is the Claude, ChatGPT, or Grok plan you already pay for. Among the closed four, Muse has a free tier with a weekly token quota and asks for a card at signup, Cue is free during early access with a paid Plus tier implied, Grok Bot starts at a $20 Cursor Pro or $30 SuperGrok plan, and dots need ChatGPT Pro, reported from $100 a month, or Business Premium. Which one works outside the US? Grok Bot publishes no region list and Cue states no region restriction. Dots are available on Business Premium everywhere ChatGPT is, but Pro excludes the EEA, Switzerland, and the UK, and OpenAI has said a Pro launch there is not planned for now. Muse is US and Canada only. MausBot has no region check; it runs wherever your model login works. Which one is open source? Only MausBot. Muse, Grok Bot, dots, and Cue are all closed. Meta has said open weights for its Spark model are on the roadmap, with no date, and that would not make the Muse agent self-hostable. Which one lets me use the Claude or ChatGPT subscription I already have? Dots use your ChatGPT Pro or Business Premium plan, and only GPT. Grok Bot uses a SuperGrok or Cursor plan, and only Grok. Muse runs on Meta's own model and Cue does not say what it runs on; neither takes an outside subscription. MausBot runs on the claude, codex, and grok CLIs, so one bot can use your Claude plan and another your ChatGPT plan, at no extra charge. Which one is a team of agents rather than one assistant? Grok Bot, Cue, and MausBot ship a roster today. Muse is one agent that spawns hidden subagents. Dots are one primary dot today, with teams of dots described as a plan. Which one keeps my data on my own computer? Only MausBot. The other four run in their makers' clouds; dots keep your memory for as long as you keep your dot, with a full reset as the only way to delete it. MausBot keeps the full conversation record in ~/.openmausbot on your disk; what leaves is only what you send to the model you chose.

Get started in two minutes

No invite code, no card, no region check. Download for macOS , Windows , or Ubuntu , sign in with the CLIs you already have, and meet your first bot. Or read the source on GitHub first. Everything on the features list is free, forever.

Read next

AI agent memory: who keeps it, and can you delete it?

Where OpenAI dots, Meta Muse, Grok Bot, Cue, Instinct, OpenClaw, Hermes, and Claude keep memory, whether you can delete one entry, and what trains the model.

Which AI agent should I use? A five-question decision

Five questions that decide between Meta Muse, Grok Bot, OpenAI dots, Cue, and MausBot: one agent or a team, your plan, your region, your data, and uptime.

Meta Muse vs OpenAI dots: the two one-agent products

Meta Muse and OpenAI dots compared on price, region, model, where the agent runs, memory, training, and phone calls, plus the open-source third option.

Bops alternative: MausBot

A Bops alternative that is open source, runs on any model, and ships for Mac, Windows and Ubuntu with phone apps. Bops is Orgo's Mac-only roster on OpenAI.

Cue by Manus alternative: MausBot

A Cue by Manus alternative without the invite code: the open source team-of-agents app, each bot with its own model, computer and apps, on your own machine.

Every agent app, compared with MausBot

The hub: one page per rival, and a verdict.

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

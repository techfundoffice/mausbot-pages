---
layout: default
title: "OpenBot by CopilotKit vs MausBot: open source Grok Bots"
description: "Open Bot, CopilotKit’s MIT template of AI coworkers, is built for companies and needs a CopilotKit account. MausBot is the open source Grok Bot for a person."
permalink: "/blog/open-bot-vs-mausbot/"
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

October 8, 2026 · 9 min read · Omkar Satpute and Milind Soni

OpenBot by CopilotKit vs MausBot: open source Grok Bots

Open Bot, CopilotKit’s MIT template of AI coworkers, is built for companies and needs a CopilotKit account. MausBot is the open source Grok Bot for a person.

OpenBot and MausBot are both open source Grok Bots for different people. OpenBot, launched by CopilotKit on August 19, 2026 as Open Bot, is an MIT-licensed template of AI coworkers for companies: policy, audit, SSO and a Helm chart, run on your own Docker host, with threads and memory in CopilotKit’s hosted Intelligence service, without which it will not start. MausBot is the open source Grok Bot for a person: a desktop app of bots on your own machine, each on the Claude, Codex or Grok plan you already pay for, Apache 2.0, with installers and phone apps.

What is OpenBot?

CopilotKit/OpenBot is the most-starred open source Grok Bot clone: 6,182 stars, 841 forks, 40 contributors, a release on October 7. CopilotKit co-founder Atai Barkai announced it as “an open source Grok Bot that works with ANY agent harness, designed for real companies”, and the Show HN the same day drew 12 points and one comment , from a maintainer saying it was in alpha. The README is unusually honest about what it is:

“The AI assistant your company can actually own.” Same shape as ChatGPT, Claude or Grok, on your infrastructure.

“A template, not a product.” There is no hosted version and no published package; you clone it, replace the example tenant and run it.

“Alpha, and under active development.”

Each coworker gets a container with a real Chromium browser, its own files and a shell, optionally under gVisor.

Every action passes a gateway that evaluates a CEL policy, fails closed, writes an audit row, and only then calls the computer. Refusals name the rule.

Any agent framework plugs in over AG-UI, the protocol CopilotKit maintains, with a dozen harness examples.

Google, Microsoft and Okta sign-in, SAML and OIDC, a people admin page, OTLP audit export and a Helm chart.

Group chats, bot-to-bot delegation, routines with a 15-minute floor and a cap of 20, reach over Slack, Teams and SMS.

A sales link: “We can build this for you, or with you, at your company.”

Two facts matter more than the feature list. First, the server refuses to start without an Intelligence URL and key: durable threads and memory live in CopilotKit Intelligence, a managed service priced free for developers with 200 threads kept three days, $39 a month for Pro and $100 a seat for Team, and self-hostable on paid plans or as a 30-day-renewable macOS preview. The MIT licence covers the code; the thing the code needs is a subscription. Second, there is no installer. Every release’s only asset is a JSON file listing container images; a Tauri desktop and an Expo mobile app exist in the tree, and an open issue asks for a signed Mac build so users can stop cloning the repository. An independent review adds that the shipped startup policy is permissive, allowing everything until you write rules, and that “a local model alone does not make the entire data path local”.

OpenBot vs MausBot

OpenBot MausBot

Launched August 19, 2026, as Open Bot; the repository is OpenBot August 11, 2026

Made by CopilotKit, a VC-backed company; 40 contributors Supamaus Software, an independent open-source project

Stars, forks 6,182, 841 About 4,200, 716

License MIT for the code; the server needs a CopilotKit Intelligence key to start Apache 2.0, app and harness; no vendor service

Built for Companies: “the AI assistant your company can actually own” A person, or a small team, in a chat app

Status Alpha; “a template, not a product”; no hosted version Shipping releases since August

Shape A self-hosted web app on Docker, Bun and Postgres; Tauri desktop and Expo mobile in the tree, from source A desktop app; iOS and Android companions from the stores

Installer No; releases ship only container images Signed installers for macOS, Windows, Ubuntu

Models OpenAI, Anthropic, Google by API key, or any AG-UI agent; no subscription sign-in Claude, Codex, Grok and other CLIs, chosen per bot, on your existing logins

Each bot’s computer A container with Chromium and a shell, optional gVisor; not your desktop apps Your own machine; or a cloud desktop per bot

Before it acts A CEL policy at the gateway, fail closed; an audit row first; the shipped startup policy is permissive Allow / Deny cards for shell commands and file edits, by default

Agents Coworkers in group chats with delegation; routines, 15-minute floor, 20 at most As many bots as you like, in rooms; routines

Reach it from The web app, Slack, Teams, SMS; a mobile app you build The desktop app, iOS and Android apps, in-app calls

Memory and threads In CopilotKit Intelligence: free tier 200 threads, 3 days; Pro $39 a month; Team $100 a seat On your disk, in ~/.openmausbot

Telemetry On by default on the desktop, disclosed without an opt-in None sent

Sign-in Google, Microsoft, Okta, SAML, OIDC None needed for the free app

What MausBot is, in the same terms

MausBot is Grok Bot’s shape without Grok Bot’s vendor: a chat app where every contact is a bot, each on the claude , codex or grok CLI installed on your machine with your existing login, so a bot costs nothing beyond the plan you have. Bots share group rooms and hand work to each other. Shell commands and file edits become Allow / Deny cards before they run, by default, for every engine. Data stays in ~/.openmausbot ; the harness listens on 127.0.0.1 only; nothing is sent to us. It installs from a signed DMG, EXE or deb, has iOS and Android apps in the stores, and is on GitHub under Apache 2.0, app and harness. Cloud plans from $15 a month add always-on bots for the laptop-closed case; the free app needs no account.

What OpenBot still does better

Governance as the product: a policy language that fails closed, an audit row written before any action, refusals that name the rule, and audit export to a SIEM. MausBot has approval cards and an activity log, not a policy engine.

Enterprise plumbing MausBot does not have: SAML and OIDC sign-in, a people admin page, a Helm chart, optional gVisor isolation per bot.

Framework-agnostic agents over AG-UI, so a LangGraph or CrewAI agent can be a coworker; MausBot’s engines are the Claude, Codex, Grok and Hermes CLIs plus OpenAI-compatible endpoints.

Generative UI: bots answer with components, not only prose.

A larger star count and a funded company behind it.

The other “open bots”

The name is crowded. gawkbot (1,488 stars) calls itself an open source grok bot and runs on Claude Code, Codex, Opencode or Ollama with an approval on every external write, but its licence is Sustainable Use, which its own site says is not open source by the strict definition, and its release artifacts still carry the name of the project the repository used to be. nightly-labs/openbot (454 stars) is a real Electron desktop for Mac, Windows and Linux with signed releases and ACP agents, under PolyForm Noncommercial, and its README warns that agents run with full access and an approval policy of never. Rakazo (3,418 stars, Apache 2.0) is the serious one and gets its own comparison . A dozen two-star repositories and one empty name-squat created the day Grok Bot launched round out the list.

The verdict

OpenBot is good software aimed at a different buyer. If you run a company and want AI coworkers behind a policy engine on your own servers, it is the strongest open-source option, with the caveat that its memory lives in a vendor’s cloud. If you are a person who read about Grok Bot and wants that, a team of named bots in a chat app, installed in a minute, on the Claude, ChatGPT or Grok plan you already pay for, with an approval card before every command and phone apps from the stores, then of the two, MausBot is the one built for you, and it is the only one in the table above that is open source with no account, no server and no vendor service in the path.

Frequently asked questions

Is OpenBot the same thing as Open Bot? Yes. CopilotKit’s August 19 launch tweets spelled it Open Bot; the repository, README and website spell it OpenBot. There is no CopilotKit/open-bot or open-grok-bot repository. Is OpenBot a product I can install? Not as shipped. The README calls it a template, not a product, with no hosted version. Every release contains only container images; a GitHub issue asks for a signed Mac build so users can stop cloning the repository. You replace the example tenant with your own coworkers and run it on Docker. Does OpenBot run without CopilotKit’s cloud? Not out of the box. The API server refuses to start without an Intelligence URL and key. Paid plans can self-host Intelligence; a local preview for macOS with Docker Desktop lasts 30 days and renews while your account is in good standing. Can OpenBot use my ChatGPT or Claude subscription? No. It takes API keys for OpenAI, Anthropic and Google, or an external agent over AG-UI. MausBot runs bots on the claude, codex and grok CLIs with your existing logins, so a bot costs nothing beyond the plan you have. Which is the best open source Grok Bot? It depends on who is asking. A company that wants policy, audit and SSO on its own servers should look at OpenBot. A person who wants Grok Bot’s shape, a team of named bots in a chat app on the plan they already pay for, with installers and phone apps, should pick MausBot. Rakazo is the other serious Apache 2.0 option, as a server you host.

Read next

OpenBot vs MausBot , the one-page summary.

The open source alternative to Grok Bot , MausBot against Grok Bot itself.

Rakazo vs MausBot , the other Apache 2.0 Grok Bot.

Rakazo vs MausBot: two open source Grok Bots, compared

Rakazo is Inbox Zero’s Apache 2.0 Grok Bot alternative: web, desktop and mobile clients on one self-hosted API with Docker. MausBot installs in a minute.

Grok Bot Team Bots vs MausBot teams: shared agents compared

xAI's Grok Bot Team Bots, in public beta since Sept 28, against MausBot's Team plan and free rooms: price for five people, who runs the bot, chats, approvals.

Muse vs Grok Bot vs Dots vs Cue: which agent to pick

Meta Muse, xAI Grok Bot, OpenAI dots, and Cue by Manus compared on price, region, models, approvals, and where the agent runs, plus the open-source fifth.

Side by side

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

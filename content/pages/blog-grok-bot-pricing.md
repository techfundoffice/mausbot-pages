---
layout: default
title: "Grok Bot pricing in 2026: what it really costs"
description: "Grok Bot has no free tier. It comes with SuperGrok ($30) and Cursor Pro ($20), with its own unpublished weekly quota and overage billed at Grok 4.6 token rates."
permalink: "/blog/grok-bot-pricing/"
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

September 22, 2026 · 7 min read · Omkar Satpute and Milind Soni

Grok Bot pricing in 2026: what it really costs

Grok Bot has no free tier. It comes with SuperGrok ($30) and Cursor Pro ($20), with its own unpublished weekly quota and overage billed at Grok 4.6 token rates.

Grok Bot has no free tier. Since August 26, 2026 it is included with SuperGrok ($30 a month), Cursor Pro ($20 a month), and the tiers above them. It has its own weekly usage allowance, separate from Grok and Cursor, and xAI has not published how big that allowance is on any tier. Go over it and you pay on demand at Grok 4.6 token rates. It is still in beta.

The plans that include Grok Bot

xAI's announcement lists plan names, not prices. The prices below are each plan's list price as reported by third parties on the date of writing. Grok Bot is not sold on its own.

Plan List price Who it is for

SuperGrok $30 / month Individuals who want Grok Bot at the lowest entry point

SuperGrok Plus $100 / month Heavier Grok users; a larger Grok Bot allowance is implied but not published

SuperGrok Heavy $300 / month The original launch floor; power users

Cursor Pro $20 / month Developers already on Cursor. Legacy Cursor Pro plans are excluded.

Cursor Pro+ $60 / month Cursor developers who hit Pro limits

Cursor Ultra $200 / month The original Cursor-side floor

Cursor Teams Standard $40 / seat / month Teams that want Grok Bot per seat

Cursor Teams Premium $120 / seat / month Teams with heavier per-seat usage

Cursor keeps its own Grok Bot plans page , which is the place to check whether your specific Cursor plan qualifies.

How the price changed

Grok Bot launched as a $200-and-up product and became a $20-and-up product in about two weeks. If you read a pricing article from mid-August, it is already wrong.

August 11, 2026 : Grok Bot enters beta. The only ways in are SuperGrok Heavy at $300 or Cursor Ultra at $200.

August 21, 2026 : SuperGrok Plus and Cursor Pro+ added, along with a 7-day usage-credit trial.

August 26, 2026 : Base SuperGrok ($30) and Cursor Pro ($20) added. The entry price drops by an order of magnitude in fifteen days.

September 3, 2026 : Enterprise controls ship, opening the door for team and company deployments.

September 17, 2026 : Weekly usage reset for everyone and one free month for new users.

What the price does not tell you

The monthly number is the easy part. Five things decide what Grok Bot actually costs you.

Allowances are unpublished. Grok Bot has its own weekly usage on every tier, and xAI has not said how many tokens or tasks that is. You find out by running out.

People run out fast. The Hacker News thread and the Cursor forum are full of quota reports; one user burned "42% of weekly allowance on day one". Routines, up to 50 per bot, run on a schedule while you sleep; check what they draw on before you set them.

Overage is on-demand at token rates. Past the allowance you pay Grok 4.6 rates, $2 per million input tokens and $6 per million output. A bot that reads a lot of pages is mostly input tokens; a bot that writes a lot is the expensive kind.

One shared cloud computer. Every bot on your account uses the same cloud computer . xAI's docs say not to use separate bots as a security boundary. When that computer got stuck on August 20 and 21, staff confirmed it took every bot down at once.

Legacy Cursor Pro is excluded, and it is beta. If you are on an older Cursor Pro plan you need to move to a current one. And the product, the allowances, and the plan list have all changed since launch, so they may change again.

Is Grok Bot free?

No. There is a 7-day usage-credit trial, added on August 21, and since September 17 new users get one free month. Grok Bot is only available through SuperGrok and Cursor plans, so the trial attaches to one of those.

The bring-your-own-subscription alternative

Grok Bot's pricing model is: pay for a plan, get a second quota you cannot see, top up at token rates. MausBot's model is: the app is free, and each bot runs on the claude , codex , or grok CLI already installed on your machine, with the login you already have. There is no second quota because there is no second account. You pay Anthropic, OpenAI, or xAI exactly what you pay them today.

Pick a model per bot. Unavailable providers are dimmed with the reason.

A worked example. Say you are already on Claude Max or a ChatGPT plan with the Codex CLI signed in. Install MausBot, sign in with those CLIs, and create four bots: one on Claude for writing, one on Codex for code, two more for whatever you like. Extra cost: $0. Your usage counts against the plan you already have, which you can see in the provider's own app. If you pay for SuperGrok, the grok CLI works the same way, so a Grok bot in MausBot draws on the plan you would have bought anyway, without a separate Grok Bot allowance.

Unlimited bots. Each has its own model, its own computer, and its own memory.

The other differences are not about money. Every shell command and file edit in MausBot lands as an Allow / Deny card before it runs. Each bot gets its own computer, yours or a cloud desktop, instead of one shared machine. Transcripts and keys stay in ~/.openmausbot . The code is Apache 2.0 on GitHub .

Every risky action is a decision you make, on your machine or a cloud one.

And what Grok Bot has that MausBot does not, so you can weigh it honestly: Teach a task by screen recording, a bot marketplace with templates, and bots that keep working from your phone with no laptop involved, because everything already lives in xAI's cloud. MausBot only keeps working with the laptop closed for bots on a cloud computer. If those three are the job, Grok Bot is the better tool today. We compared the two line by line in Grok Bot vs MausBot .

Frequently asked questions

Is Grok Bot free? No. There is no free tier. There is a 7-day usage-credit trial, and since September 17, 2026 new users get one free month. After that it needs a SuperGrok or Cursor plan, and it has its own weekly usage allowance on top of that plan's limits. How much is Grok Bot per month? As little as $20 a month on Cursor Pro or $30 on SuperGrok, as of August 26, 2026. Those are the plans' list prices; Grok Bot has no separate price. Heavier allowances come with SuperGrok Plus ($100), Heavy ($300), Cursor Pro+ ($60), or Ultra ($200), and overage is billed at Grok 4.6 token rates. Does Grok Bot come with SuperGrok? Yes, since August 26, 2026. It is included with SuperGrok, SuperGrok Plus, and SuperGrok Heavy. Grok Bot usage is metered separately from your Grok chat usage, and the size of the Grok Bot allowance on each tier has not been published. Does Grok Bot come with Cursor Pro? Yes, for current Cursor Pro, Pro+, Ultra, Teams Standard, and Teams Premium plans, since August 26, 2026. Legacy Cursor Pro plans are excluded. Grok Bot has its own weekly usage separate from your Cursor usage. Is there a Grok Bot free trial? Yes. A 7-day usage-credit trial has been available since August 21, 2026, and new users who sign up after September 17 get one free month. Grok Bot is only available through SuperGrok and Cursor plans.

Download MausBot for macOS , Windows , or Ubuntu , sign in with the CLIs you already have, and make your first bot. No card, no trial clock, no second quota. The pricing page has the Free, Pro, and Enterprise tiers; the app itself is free. If you are weighing the two products rather than the two bills, start with the open-source alternative to Grok Bot .

Read next

OpenBot by CopilotKit vs MausBot: open source Grok Bots

Open Bot, CopilotKit’s MIT template of AI coworkers, is built for companies and needs a CopilotKit account. MausBot is the open source Grok Bot for a person.

Rakazo vs MausBot: two open source Grok Bots, compared

Rakazo is Inbox Zero’s Apache 2.0 Grok Bot alternative: web, desktop and mobile clients on one self-hosted API with Docker. MausBot installs in a minute.

Grok Bot Team Bots vs MausBot teams: shared agents compared

xAI's Grok Bot Team Bots, in public beta since Sept 28, against MausBot's Team plan and free rooms: price for five people, who runs the bot, chats, approvals.

Side by side

Grok Bot alternative: MausBot

An open source Grok Bot alternative: the same roster-of-bots idea, free and Apache 2.0, on your own machine, on the Claude, Codex and Grok accounts you have.

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

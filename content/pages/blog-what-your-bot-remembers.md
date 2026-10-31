---
layout: default
title: "What your bot remembers, and who keeps the notebook"
description: "We moved the memory of every conversation out of the AI company's tool and into MausBot itself. Here is what that fixes, in plain words."
permalink: "/blog/what-your-bot-remembers/"
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

September 5, 2026 · 6 min read · Omkar Satpute and Milind Soni

What your bot remembers, and who keeps the notebook

We moved the memory of every conversation out of the AI company's tool and into MausBot itself. Here is what that fixes, in plain words.

Until now, each AI engine kept its own memory of your conversation, and MausBot only held a partial copy. From this update, MausBot keeps the complete record itself and gives every model exactly as much of it as that model can hold. That one change fixes six things that used to go wrong, some of them silently, and it makes a new kind of bot possible.

Think of it as a notebook

Every conversation you have with a bot is a notebook. It holds what you said, what the bot replied, and, just as importantly, what the bot did : which files it opened, what it changed, what it looked up.

The question is who keeps that notebook. Until now, the answer was: the AI company's own tool. When you talk to a Claude bot, MausBot hands your message to Claude's program, and that program keeps the notebook. Same with Codex, same with the others.

MausBot kept a photocopy of the last 40 pages, just in case. The photocopy had the words, but none of the actions. And 40 pages was the limit no matter which model you were using.

BEFORE NOW MausBot a photocopy of the last 40 pages (words only) AI company's tool the full notebook every page, every file it touched MausBot the full notebook every page, every tool it used what fits Any model Claude, Codex, a local model, your own key The notebook moved. Everything else follows from that. Before, the complete record lived inside each AI company's own tool. Now MausBot keeps it, and every model gets the pages that fit.

Why that was a problem

It worked fine as long as the AI company's tool remembered everything. The trouble started the moment it didn't, which happens more often than you'd think: a session that expires overnight, a model you switch halfway through, a message you go back and edit.

When that happened, MausBot could only rebuild the conversation from its 40-page photocopy. Sometimes it couldn't rebuild at all. Two of the failures were silent: the bot would carry on talking as if nothing had happened, but with a blank memory. You'd only notice when the reply made no sense.

What we changed

MausBot now keeps the whole notebook itself: every message, every action the bot took and whether it worked, all stored on your own computer in the same place the app already keeps your data.

Before each reply, it looks at which model you're using and how much that model can read at once, then hands over the pages that fit. A big model gets a lot. A small model running on your laptop gets less. Neither is stuck at 40.

The AI companies' tools still run their own live sessions, and on a normal day nothing about that changes. The difference is what happens on a bad day. If a session is lost, MausBot rebuilds it from its own notebook and carries on, and tells you if it can't.

Switching a bot to a different model used to mean the new one started nearly blind. Now it gets the whole notebook.

When the notebook gets too long

Every model has a limit on how much it can read at once. A long project will pass that limit eventually. When it does, MausBot writes a short recap of the oldest part, keeping the decisions, the file names, and your preferences, and keeps the recent pages word for word.

WHAT YOU SEE every message, always WHAT THE MODEL READS a one-page recap of the first eight the newest, word for word Like the “previously on” at the start of an episode. Your chat keeps every message; the model gets a recap plus the latest.

Nothing is deleted. Your chat still shows every message. A small marker appears where the recap was made, and you can open it to read what the model was told. If you don't like the recap, you can keep talking; it only affects what the model reads, never what you see.

The six things this fixed

None of these were on the to-do list. Each one turned up while checking the plan against how the app actually behaved.

When this happens Before Now

A Claude conversation's session expires Every message after that failed the same way, forever. The only way out was switching the bot to a different engine. The bot quietly starts a fresh session, hands it the whole conversation from MausBot's notebook, and carries on.

A Codex or Pi conversation can't be picked up again The bot started over with no memory at all, and nothing told you. You got a reply that ignored everything you'd said. Same fix: the fresh session gets the full notebook first.

You edit a message, or switch models, on an API-based bot The whole conversation was sent to the model twice in one go. You paid double, and the model saw everything duplicated. Sent once.

You send a follow-up while a screenshot is still being taken That message vanished the next time you opened the app. It was still on disk; the app just lost track of it. It stays exactly where you put it.

A long conversation Every model got the last 40 messages and no more, whether it was a small local model or a big one that could hold hundreds. Each model gets as much as it can actually hold. Big models see far more; small models see a recap plus the latest.

You move a bot to a different engine halfway through a project The new engine saw the chat, but had no idea which files the old one had already read or changed. A short note of every tool the bot used comes along too.

A new kind of bot, in preview

Once MausBot holds the notebook, one more thing becomes possible. Every bot so far has handed the actual work, calling the model, running a tool, calling the model again, to the AI company's program. The new OpenMaus Runtime does that work inside MausBot itself.

In plain terms: you can point a bot at any AI provider that speaks the common OpenAI-style API, paste in your own key, and MausBot runs the bot end to end. It also works with a model running on your own machine, with no key and no bill at all.

Because MausBot is the one running the loop, it is also the one asking permission. Before the bot touches a tool, you get an approval card, the same one you already know. If you don't answer, the answer is no. Close the window, walk away, let it time out: all of those mean no. There are hard limits on how many steps a bot can take in one turn, so a confused bot stops instead of spinning.

The preview engine asks before every tool. No answer means no.

Two honest notes. It is a preview: it is off until you turn it on in settings, and no existing bot is ever moved onto it without you choosing that. And it is not a Claude or Codex login. It uses an API key, and the provider you pick bills you for what you use. The settings screen says so in as many words.

Questions people asked

Do I have to do anything? No. Existing bots keep working exactly as before, and the memory fixes apply to them automatically. The only new thing you can opt into is the preview engine, and it stays off until you switch it on in settings. Will my old conversations be summarised without asking? You always see every message; nothing is ever removed from your chat. The recap only changes what the model reads, and it only happens when MausBot is rebuilding a conversation for a model, such as after a model switch or an edit. Does MausBot send my conversations anywhere new? No. The notebook lives on your own disk, in the same place the app already keeps everything. The only thing that leaves your computer is what goes to the model you chose, the same as before. Is the preview engine free? The engine itself is free and open source. It talks to whichever AI provider you point it at, using your own API key, so that provider bills you for what you use. A local model on your own machine costs nothing.

For the curious

The work landed as three pull requests on GitHub, each building on the last: the memory work , the tests that prove it , and the preview engine . The recap logic is the one we borrowed from pi.dev at the start of the project, kept on purpose. All of it is open source under Apache 2.0 .

Try it

Download MausBot for macOS, Windows, or Ubuntu. Your bots keep working as before; the notebook just moved somewhere safer. If you want the bigger picture of why the app is a chat app at all, read why we built a chat app for AI agents instead of an IDE .

Read next

AI agent memory: who keeps it, and can you delete it?

Where OpenAI dots, Meta Muse, Grok Bot, Cue, Instinct, OpenClaw, Hermes, and Claude keep memory, whether you can delete one entry, and what trains the model.

Meta Muse vs OpenAI dots: the two one-agent products

Meta Muse and OpenAI dots compared on price, region, model, where the agent runs, memory, training, and phone calls, plus the open-source third option.

Hark Pro vs MausBot: Adcock’s assistant vs the open team

Hark Pro, from Brett Adcock’s Hark Labs, is one assistant in Hark’s cloud on web, iOS and Android. MausBot is the open source alternative on your own machine.

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

---
layout: default
title: "Why we built a chat app for AI agents instead of an IDE"
description: "Everyone is forking the editor. We think the right interface for a team of AI agents is the one you already use to manage a team of people: a messaging app."
permalink: "/blog/chat-app-not-an-ide/"
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

August 23, 2026 · 6 min read · Omkar Satpute and Milind Soni

Why we built a chat app for AI agents instead of an IDE

Everyone is forking the editor. We think the right interface for a team of AI agents is the one you already use to manage a team of people: a messaging app.

An IDE is built to help one person write one thing. A messaging app is built to help one person keep track of many others doing many things at once. The second problem is the one you have when you run a team of agents. So MausBot is a chat app: agents are contacts, work is a thread, and the sidebar is a roster you manage the way you manage people.

Everyone forked the editor

The default answer to “where should an AI agent live” has been the place the code already is. Fork the editor, dock a panel, put the model next to the file. When the agent's job was autocomplete, that was obviously right: the work was happening in the buffer, so the help belonged in the buffer.

The terminal answer is the same instinct in a smaller box. Run the agent as a full-screen session, hand it the tty, wait. That works beautifully for one agent doing one thing while you watch.

Both break the moment you have four.

Agents stopped being autocomplete

An agent now goes away for twenty minutes, runs commands, edits files, opens a browser, reads your Linear board, and comes back with a question. It is not helping you type. It is doing a piece of work you delegated.

That is a different relationship, and it breaks the editor metaphor in a specific way: an IDE has one focus. One window, one active file, one thing you are looking at. It is a single-threaded instrument, and that is a feature — right up until you are running four agents and three of them are working while you are not looking.

The question stops being “what am I editing” and becomes “who is blocked, who is done, and who needs me.” No editor answers that, because no editor was ever asked to.

Something already answers that question

Every messaging app you have ever used is a solved interface for exactly this problem: a list of parties who each have their own ongoing context, who work while you are away, and who interrupt you when they need something.

A sidebar of threads is a status board. Unread means someone needs you. Pinned means this one matters today. A thread is durable context that survives you closing the window. None of this had to be invented — you have known how to use it for twenty years, and so has everyone you would hand the app to.

Every chat in the sidebar is a real agent with its own model, computer, and connected apps.

Taking the metaphor literally

The interesting part was deciding to commit rather than borrow the look. If a bot is a contact, then everything you can do to a conversation should work on it.

So you can pin a bot, mark it unread, duplicate it, hide it, or delete it. Duplicate is the one that surprised us: it turns a bot you have configured carefully into a template you can fork, which is a thing you would never think to build if you had modelled agents as sessions. Marking a finished thread unread to deal with tomorrow is another — nobody designs that feature for an agent runner, and everybody already does it with messages.

Pin, mark unread, duplicate, hide, delete. The verbs came free with the metaphor.

Approvals became messages too. When a bot wants to run a shell command or edit a file, it asks in the thread and you answer in the thread — the same place the rest of the conversation lives, rather than a modal that interrupts whatever you were doing.

Then the group chat happened

Multi-agent orchestration is usually a graph you configure: nodes, edges, a supervisor, a config file describing who calls whom.

Take the chat metaphor seriously and you get it for free, because a group chat is already a multi-agent protocol that humans find obvious. Put several bots in a room. One answers by default, or everyone does, or only the ones you @mention. They ask each other questions and hand off work. You are in the room the whole time, so delegation is something you watch rather than something you configure and hope about.

We did add one thing humans do not need: a peer-comms approval card, so you decide which bots are allowed to talk to which. It is the one place the metaphor needed a seatbelt.

And then voice, which we did not plan

Once bots were contacts, a call button was the obvious missing verb, and it turned out to be genuinely useful rather than a gimmick. A bot can narrate what it is doing, ask for an approval out loud, and take your answer while your hands are elsewhere. Nobody asks for a phone call with their IDE. It is a reasonable thing to want from a colleague.

What this costs

The trade is real and worth stating plainly: a chat app is a worse place to read a diff than an editor is. It always will be. If your work is one person, one repository, one change at a time, an editor with an agent panel is a better tool and you should use it.

The bet is that this is not where agent work is heading. As soon as the second agent shows up, the bottleneck stops being how well you can read one file and starts being whether you can keep track of four things at once. That is a coordination problem, and coordination has an interface already.

The general point

When a new capability arrives, the reflex is to bolt it onto the tool nearest to it. Agents write code, so they went in the code editor. But the right interface follows from the relationship, not from the artifact. The relationship with an agent is delegation, and we have had good delegation interfaces for a long time — we just had not pointed one at software that isn't a person.

We might be wrong. The whole thing is Apache 2.0 licensed on GitHub if you want to argue with the design by reading it.

Try it

Download MausBot for macOS, Windows, or Ubuntu. It runs on the claude , codex , and grok CLIs you already have, keeps everything in ~/.openmausbot on your own disk, and is free forever. If you want the feature-by-feature version instead of the argument, read Grok Bot vs MausBot .

Read next

Hark Pro vs MausBot: Adcock’s assistant vs the open team

Hark Pro, from Brett Adcock’s Hark Labs, is one assistant in Hark’s cloud on web, iOS and Android. MausBot is the open source alternative on your own machine.

Bops vs MausBot: Orgo's business bots vs the open team

Bops (bops.bot) is Orgo's Mac app of business-ops bots on OpenAI, each with a cloud computer, email and phone. MausBot is the open source team on any model.

Meet MausBot: your own team of AI bots, in a chat app

Meet the free, open-source chat app for your own team of AI bots. Bring a supported provider, try a first task, and explore the project and its contributors.

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

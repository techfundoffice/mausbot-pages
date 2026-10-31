---
layout: default
title: "AI agent memory: who keeps it, and can you delete it?"
description: "Where OpenAI dots, Meta Muse, Grok Bot, Cue, Instinct, OpenClaw, Hermes, and Claude keep memory, whether you can delete one entry, and what trains the model."
permalink: "/blog/ai-agent-memory-who-keeps-it/"
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

October 2, 2026 · 9 min read · Omkar Satpute and Milind Soni

AI agent memory: who keeps it, and can you delete it?

Where OpenAI dots, Meta Muse, Grok Bot, Cue, Instinct, OpenClaw, Hermes, and Claude keep memory, whether you can delete one entry, and what trains the model.

Every personal AI agent now remembers you. Three questions decide whether that is fine: where the memory lives, whether you can read and delete a single entry, and whether it trains the model. The answers range from "a Markdown file you can open" to "delete the whole agent". OpenAI's dot has no per-memory view or delete at all, which is fewer controls than the ChatGPT it lives inside. Meta Muse gives you the file but warns it may still remember what you removed. Local agents such as OpenClaw, Hermes, and MausBot keep memory on your disk and do not train on it. The table below puts them side by side.

Three questions to ask any agent

An agent that reads your inbox, your calendar, and your files will build a picture of you fast. That picture is the memory. Before you hand one the keys, the help pages answer three things, or do not.

Where does it live? On a server the company runs, or in a file on your machine. This decides who can read it, who holds a copy after you leave, and whether a subpoena or a breach reaches it.

Can you read and delete one entry? Not the whole thing, one line: the home address it picked up from a delivery receipt, the salary figure from a PDF. Some products show you a list. Some show you a file. Some only offer a reset.

Does it train the model? Memory that trains is memory you cannot take back. Look for the toggle, the default, and whether the opt-out applies to what was already collected.

OpenAI dots

A dot receives your ChatGPT memories and then builds its own. The dots privacy FAQ is direct about the controls: "Your dot can retain context from your conversations and plugins for as long as you keep your dot." And: "You currently cannot view, delete or directly modify individual dot memories, including specific details that enter the dot's context from plugins." The remedy is the big one: "You can delete your dot's context by deleting your dot." Disconnecting a plugin "stops new access through that connection. It does not delete information your dot has already built into its context." Turning Memory off in ChatGPT "does not delete information that your dot has already received."

Compare that with ChatGPT itself , which lets you view, edit, and delete each saved memory in Memory settings, or ask it to forget, with the note that OpenAI may retain logs of deleted saved memories for up to 30 days. The dot lives inside ChatGPT and has fewer memory controls than ChatGPT. Training on personal plans follows the "Improve the model for everyone" toggle and can include dot actions, delegated work, automations, and connected-app data; business plans are not trained on by default, and OpenAI says it does not train directly on proactive background research or its notes.

Meta Muse

Muse keeps memory in the per-user cloud VM that Meta's security post calls "the system of record", as a MEMORY.md file. The help page says: "You can inspect, edit and download these files freely, including Muse's memory about you." You can also "ask Muse to forget a topic or set of interactions", which Meta describes as best-effort, with this caveat verbatim: "After you've deleted something from Muse, Muse may still remember information that it learnt from what you deleted." Reset "deletes all your Muse data." Training is on by default, with a toggle under Settings, Data controls, and Meta says the data is not shared with its ad systems. Meta's access to the VM is limited by policy today, with a Confidential VM promised later this year. Retention after you delete the account is not stated.

xAI Grok Bot

The Grok Bot docs say "A Bot can retain stable preferences, role context, and summaries of prior work," and add that "Memory is not a substitute for an authoritative source." There is no documented screen for viewing, editing, or deleting an entry; the advice is to "correct stale assumptions directly" in chat. The FAQ says deletion "removes the Bot's active profile, conversation, and routines" and that "files and logins on that computer may remain. Backend retention follows the applicable Cursor terms." Training opt-out "follows the applicable Cursor account and privacy settings." Each routine keeps its 20 most recent run records. A Cursor staff reply on the forum, August 26, reported there is no manual compaction and that bots auto-summarise near the context limit.

Cue by Manus

Cue is the thinnest documented. The Play listing says "Memory and Dream help your Agent remember your preferences, past decisions, project goals", and that is the whole public account: no page on where memory lives, how to view it, how to delete one entry, or what a reset does. The nearest thing is the Manus account deletion page : "we will take steps to delete your content", with retention "as long as necessary" and no period given. A third-party audit of Manus found a training opt-out that is off by default and no stated retention for conversation logs.

Instinct

Everything here is reported, not from a help page. TechCrunch (August 24) and Claire Vo on X (August 21) described revoking Instinct's Google access at 11 AM and receiving an inbox summary at 2 PM. Asked, the bot reportedly said emails were "stored in plain text for later searches", and a data export contained full message text. Deletion initially required a request; a "delete external data" tool was added to settings around August 21. The terms of service grant a perpetual, irrevocable licence to user materials, including for training, with a forward-only opt-out and no retention schedule. Our Instinct comparison has the rest.

OpenClaw

OpenClaw 2026.8.1 shipped "visible workflows to search, inspect, import, and remove memory" , under Settings, Memory. The CLI adds openclaw memory forget , a provenance-based purge by session, hook, or participant, with the caveat that "original transcripts and external copies may remain"; memory reset clears the index only. The stores are local files: an SQLite database per agent, plus MEMORY.md, USER.md, dated notes under memory/, and DREAMS.md in the workspace. No training; memory is local.

Hermes Agent

Hermes keeps two files in ~/.hermes/memories/ : MEMORY.md, capped at 2,200 characters, and USER.md, capped at 1,375 , with sessions in an SQLite store at ~/.hermes/state.db . The caps are hard: "Memory does not auto-compact" and the agent "returns an error instead of silently dropping entries." To delete something, edit the file, or use /memory pending , approve , and reject on new entries, or hermes journey list|edit|delete . Local files, no training.

Claude and Cowork

Anthropic's memory help page , updated October 1, 2026, is the most complete of the cloud agents: Settings, Memory, Topics lists each memory, and you can read, edit, or delete any one of them. Pause keeps everything in place; Reset is irreversible and deletes everything including project memories. Memory is per project where you want it. One caveat: "When a conversation expires or is deleted, related memory entries generated from it won't be removed." On by default on Free, Pro, and Max; admin-controlled on Team and Enterprise.

Side by side

Every cell comes from the company's own help page or docs, except the Instinct row, which is reported, and the Cue training cell, which comes from a third-party audit. "Not documented" means the company has not said.

Product Where it lives View a single memory Delete a single memory What reset does Trains the model

OpenAI dots OpenAI's servers, for as long as you keep your dot No No Deleting the dot deletes its context; your files, Codex threads, ChatGPT conversations, and ChatGPT memories stay Personal plans follow the Improve the model for everyone toggle; business plans not by default

ChatGPT itself OpenAI's servers Yes, in Memory settings Yes; logs of deleted memories may be kept up to 30 days Not covered in this review Follows the same toggle

Meta Muse A per-user cloud VM, as MEMORY.md Yes: inspect, edit, download Ask Muse to forget, best-effort; it may still remember what it learnt from the deleted item Deletes all your Muse data On by default; toggle in Settings, Data controls

Grok Bot xAI's backend; stable preferences, role context, and summaries No UI documented No UI documented; correct stale assumptions in chat Deleting the bot removes its profile, conversation, and routines; files and logins on its computer may remain Follows your Cursor account and privacy settings

Cue by Manus Not documented Not documented Not documented Account deletion: Manus will take steps to delete your content; retention as long as necessary Opt-out exists and is off by default, per a third-party audit

Instinct (reported) A cloud computer; emails reportedly stored in plain text for later searches Full message text in a data export, reported A delete-external-data tool was added around Aug 21 after a request-only process, reported Not stated ToS grants a perpetual licence including training; opt-out is forward-only

OpenClaw Local files: an SQLite index plus MEMORY.md, USER.md, dated notes, DREAMS.md Yes: search and inspect memory forget purges by session, hook, or participant; transcripts may remain memory reset clears the index only No

Hermes Agent Local files: ~/.hermes/memories/MEMORY.md and USER.md, plus an SQLite session store Yes: open the file Edit the file, or reject a pending entry, or delete a journey Delete the files yourself No

Claude and Cowork Anthropic's servers, as topics Yes, per topic Yes, per topic; entries from a deleted conversation are not removed with it Pause keeps it; Reset deletes everything including project memories, irreversibly Not covered in this review

MausBot ~/.openmausbot on your own disk, as the full conversation record Open the folder, or scroll the chat No per-memory UI; it is a folder you can open, back up, or delete Delete the folder; no company holds a copy MausBot does not; your model provider's own setting applies to what you send it

The pattern

Cloud agents give you a reset button. Local agents give you a file. That is the whole table in two sentences. Dots have no way to remove one entry, and Grok Bot and Cue document none; the unit of deletion is the agent. Muse and Claude are the exceptions among the cloud products, and Muse's own help page says the forget is best-effort. Hermes and MausBot never had to design a delete feature, because the memory is a file in a folder you already own; OpenClaw's is a command over local files.

The oddest row is the dot. It lives inside ChatGPT, inherits ChatGPT's memories, and then offers fewer controls than ChatGPT does: no list, no edit, no single delete, and no undo when you disconnect an app. If per-memory control matters to you, the product that has it today is the chat app, not the agent built on top of it.

How MausBot handles it

MausBot, published on GitHub as MausBot, keeps the full conversation record for every bot, every message and every action the bot took, in ~/.openmausbot on your own disk. Nothing leaves your machine except what you send to the model you chose for that bot. MausBot does not train on it; there is no server to train from. Your model provider's own data setting applies to what you send it, the same as it would in that provider's own app. There is no per-memory list to edit, and we are not going to claim one. The honest description is that it is a folder you can open, back up, or delete, and no company holds a copy. How that record is kept, and what each model is shown from it, is in what your bot remembers .

Every chat in the sidebar is a record on your own disk. Delete the folder and no company holds a copy; only what you sent to your model provider ever left.

Frequently asked questions

Can I delete a single memory from my OpenAI dot? No. OpenAI's FAQ says you currently cannot view, delete, or directly modify individual dot memories, including details that enter the dot's context from plugins. The only delete is deleting the dot, which removes its context and leaves your files, Codex threads, ChatGPT conversations, and ChatGPT memories in place. Does Meta Muse forget when I ask? Mostly. You can ask Muse to forget a topic or a set of interactions, and Meta describes that as best-effort. Its help page adds that after you have deleted something, Muse may still remember information it learnt from what you deleted. You can also open, edit, and download the MEMORY.md file directly, and a full reset deletes all your Muse data. Does deleting my ChatGPT memory delete my dot's memory? No. The dot receives your ChatGPT memories and then builds its own. Turning Memory off in ChatGPT does not delete information the dot has already received, and disconnecting a plugin does not delete what the dot already built into its context. Deleting the dot is the only way to clear it. Which AI agents store memory locally? OpenClaw, Hermes Agent, and MausBot. OpenClaw keeps an SQLite index and Markdown files in the agent workspace. Hermes keeps MEMORY.md and USER.md under ~/.hermes/memories. MausBot keeps the full conversation record in ~/.openmausbot. In each case the memory is a file or folder on your disk, and none of the three trains a model on it. Dots, Muse, Grok Bot, Cue, Instinct, and Claude keep memory on their makers' servers. Do AI agents train on my memory? It depends on the product and the plan. Dots on personal plans follow the Improve the model for everyone toggle, and business plans are not trained on by default. Muse trains by default with an opt-out in Data controls. Grok Bot follows your Cursor account settings. Cue's opt-out is off by default per a third-party audit. Instinct's terms grant a perpetual licence that includes training, with a forward-only opt-out. OpenClaw, Hermes, and MausBot do not train; for MausBot, the provider you send messages to applies its own setting.

If you want the file instead of the reset button, download MausBot for macOS , Windows , or Ubuntu , sign in with the Claude, ChatGPT, or Grok CLI you already have, and open ~/.openmausbot whenever you like. The app is free and Apache 2.0 licensed; the source is on GitHub .

Read next

Muse vs Grok Bot vs Dots vs Cue: which agent to pick

Meta Muse, xAI Grok Bot, OpenAI dots, and Cue by Manus compared on price, region, models, approvals, and where the agent runs, plus the open-source fifth.

Meta Muse vs OpenAI dots: the two one-agent products

Meta Muse and OpenAI dots compared on price, region, model, where the agent runs, memory, training, and phone calls, plus the open-source third option.

Meta Muse vs Grok Bot vs Instinct: which agent to pick

Meta Muse, xAI Grok Bot, and Instinct compared on price, region, models, approvals, and where the agent runs, plus the open-source option that works anywhere.

OpenAI dots alternative: MausBot

An OpenAI dots alternative with no Pro plan and no region lock: a free, open source team of agents on your own machine, on the ChatGPT account you have.

Instinct alternative: MausBot

An Instinct AI alternative you can download today: open source, signs into your apps over OAuth instead of holding passwords, and asks before it acts.

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

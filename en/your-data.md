# Your data: what Taibu writes about you

Taibu keeps what it knows in ordinary files inside your project folder. Nothing is hidden in a database and nothing sits on a Taibu server. This page is the map: what each file holds, how it gets written, and which ones can ever reach a colleague.

Open any of them from the file tree on the left.

## You, personally

| File | How it gets written | What is in it |
|---|---|---|
| `intake.md` | The setup wizard, and **Settings → "My data and goals"** afterwards | Your seven answers: who you are and what you sell, one or two samples of your writing, your priorities for the quarter, where revenue lands, where you talk to people, where your documents live, and what eats your week |
| `context/persona.md` | Only the `/learn-me` skill, and only after you approve each change | Your digital twin: your voice and style rules, what you are trying to do and why, how you decide, what you like and what irritates you, the people around you |

**Neither of these is ever shared with a team.** They are blocked at the sync layer, so they stay on your computer even if someone shares the folder they live in. They are also why Taibu sounds like you rather than like a generic assistant, so they are worth keeping accurate.

`persona.md` is never rewritten behind your back. `/learn-me` proposes changes from real evidence, your actual drafts and your corrections, and you approve them one by one.

## Your company

| File | What belongs in it |
|---|---|
| `company/offer.md` | What you sell, your prices, what makes you different |
| `company/icp.md` | Who you sell to, the problem they have, where to find them |
| `company/strategy.md` | Where the business is going and what matters right now |
| `company/sops/<process>.md` | One file per repeatable process: how we do X |

These fill up as you work. Describe how something is done, set a price, define a customer or set a direction, and Taibu writes it to the right file and tells you in one line what it recorded.

The split matters: **`company/` is what the company knows, and it can be shared with a team. `context/persona.md` and `intake.md` are who you are, and they cannot.** That is the whole reason they are separate folders.

## Decisions, references, connections

| File or folder | What it is |
|---|---|
| `decisions/log.md` | Dated decisions with the reason behind each one. When you decide something, Taibu offers to log it |
| `references/` | Frameworks, voice samples, and a guide per tool you connect. `references/voice.md` is the register Taibu writes in |
| `connections.md` | The register of every system Taibu knows about, connected or not. **Run `/audit` to see the real status** |
| `.env` | Your API keys. Never shared, never shown in chat, and filled in from **Settings → "Keys"** rather than by hand |

## Your instructions

`CLAUDE.md` in the project root is the standing instruction file: how Taibu should work with you, where things live, the rules it must follow. It is loaded at the start of every conversation. `AGENTS.md` is the same thing for the OpenAI Codex engine.

You can edit it. If you find yourself repeating an instruction in chat, put it there instead and it applies from then on.

If you are in a team, your admin's shared rules appear inside a marked block in this file. Everything outside that block stays yours.

## Memory

The three memory layers, `memory.md`, `memory/facts/` and `memory/journal/`, have their own page. See **What Taibu remembers**.

## The activity log

Taibu keeps a record of what happens in the app: what you asked for, every tool an agent ran and with what, and files the app wrote, renamed or deleted. It exists so that if anyone ever asks what happened, there is a straight answer instead of a memory.

Three things make it worth having:

- **It is always on.** You cannot switch it off, and neither can Taibu. A record that can be turned off before doing something is not a record.
- **It cannot be edited.** Every entry is sealed to the one before it, so changing or removing any entry breaks everything after it. **Settings → Activity log** tells you whether it is intact, and names the first entry that is not if something has been touched.
- **An independent authority confirms it.** Every so often Taibu sends a checksum of the record, and nothing else, to an independent timestamping service. That proves the record existed in exactly that state at that time. Your prompts, files and paths never leave the machine, only a 32 character checksum.

Passwords and API keys are removed before anything is written.

**Where it lives:** in Taibu's own folder on your computer, not in your project, so team sharing never touches it and the AI cannot write to it.

**Who can read it:** you. It is never uploaded, and MGR Tech Solutions never receives it. If you ever need to prove what happened, you produce it and anyone can check it with the verifier that ships with Taibu.

**What it does not do:** it records what was asked and what was done, not everything the AI said back. And nothing on your own computer can stop somebody with administrator rights deleting the whole folder. What it guarantees is that a record which is still there has not been quietly altered.

## Work the app manages

The `.taibu/` folder is the app's own bookkeeping: your chats, the drafts waiting in the Outbox, the reports your routines produced, and your team keys and sync state. You do not need to open it, and it is best left alone.

## What can leave your computer

| Data | Leaves? |
|---|---|
| `intake.md`, `context/persona.md`, `.env` | **Never** |
| Memory with no scope | **Never**, and no scope is the default |
| `company/`, `references/`, `decisions/`, skills, scoped memory | Only if your admin has shared that folder with a scope you are in, and only encrypted |
| Your work, to MGR Tech Solutions | **Never.** No file, prompt or reply is ever uploaded |
| Your licence key, an anonymous machine id and your email | Sent when you activate and each time the app starts, to check the licence is valid |
| A checksum of the activity log | Sent to an independent timestamping service. 32 characters, no content |
| Requests to your AI engine | Go to whoever you chose, Anthropic or OpenAI, under your own account and their terms |

Everything above is a plain text file. You can open it in any editor, back it up, put it in git, or delete it. If you stop using Taibu, your knowledge stays exactly where it is.

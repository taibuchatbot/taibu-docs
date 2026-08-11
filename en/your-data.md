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

## Work the app manages

The `.taibu/` folder is the app's own bookkeeping: your chats, the drafts waiting in the Outbox, the reports your routines produced, and your team keys and sync state. You do not need to open it, and it is best left alone.

## What can leave your computer

| Data | Leaves? |
|---|---|
| `intake.md`, `context/persona.md`, `.env` | **Never** |
| Memory with no scope | **Never**, and no scope is the default |
| `company/`, `references/`, `decisions/`, skills, scoped memory | Only if your admin has shared that folder with a scope you are in, and only encrypted |
| Anything at all, to Taibu | Never. There is no Taibu server holding your work |

Everything above is a plain text file. You can open it in any editor, back it up, put it in git, or delete it. If you stop using Taibu, your knowledge stays exactly where it is.

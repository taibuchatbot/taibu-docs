# What Taibu remembers

Taibu remembers your work across months. Everything is plain files in your project that you can read, edit or delete.

**Gear icon → Settings → "Memory"**

![The memory panel](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/15-memory.png)

## Three layers, and the files behind them

| Layer | Where it lives | What it is |
|---|---|---|
| **Compiled truth** | `memory.md` | A short, curated summary of what matters most about you and your work. Kept deliberately short, because it is loaded into every single conversation |
| **Structured memories** | `memory/facts/<name>.md`, one file per fact | One durable fact per file: a decision, a correction, a preference, a price, a client, a tool you use. Superseded facts move to `memory/facts/archived/` |
| **Timeline** | `memory/journal/<year-month>.md`, plus `memory/today.md` | An append-only log, month by month, and a short summary of today's work. Nothing is thrown away |

There is one more file: `memory/recall.mjs`, the small search program Taibu runs over your structured memories when you ask about something old.

## How memories get written

Three ways, and all three end in the same files:

1. **Automatically, after each exchange.** The app looks at what just happened and captures anything that reads like a durable fact.
2. **By Taibu, while you work.** When you make a decision, correct it, state a preference, or mention something about your setup, it writes the fact straight away rather than waiting for the automatic pass.
3. **By you.** Everything in the Memory panel is editable, and "Edit as text" opens the raw `memory.md` for a rewrite.

A structured memory is not just a sentence. Each one records **when it was learned, which agent learned it, which conversation, who said it, your exact words, the files worth checking, how important it is, and whether it is still current**. That is what makes an answer months later checkable rather than a guess.

## What Taibu reads, and when

This is the part worth knowing, because it explains why Taibu sometimes knows something instantly and sometimes has to go looking.

**Loaded into every message, always:**

- `memory.md`, the compiled truth
- a digest of your most recent and most important structured memories
- `memory/today.md`

**Opened only when needed:** the full fact files, the month-by-month journal, and anything else in your project. Older or more specific context is fetched through recall, not carried around.

This is why the compiled truth is kept short. It is the part Taibu never has to look up, so it should hold what is true about you in general, not every detail you have ever mentioned.

## Recall

Ask about something from months ago, in whatever words come to mind. Taibu searches its structured memories and answers **with citations**: which file, what date, who said it, and the exact words you used.

If it finds nothing, it tells you so instead of guessing. You can search the same way yourself from the box at the top of the Memory panel.

Recall reads the fact files. If your knowledge has only ever gone into `memory.md`, there is nothing for it to search, and Taibu will say so.

## Import your history

The first time, press **"Import past conversations"**. Taibu turns your existing chat history into searchable memory, so you start with everything you have already told it.

## Keeping it tidy

Add the **"Memory tidy-up"** routine and Taibu consolidates weekly: merging duplicates, archiving stale facts, folding repeated themes into the compiled truth. Important and confirmed facts are never removed automatically.

## Privacy

Memory is local. It is ordinary files in your project folder, and nothing goes to a Taibu server.

A memory with **no scope is private** and never leaves your computer. That is the default. Only memories explicitly given a team scope are ever shared, and even then they are encrypted before they leave. See **Working as a team** for how scopes work.

Two files are never shared with a team no matter how sharing is set up: your onboarding answers (`intake.md`) and your personal profile (`context/persona.md`). See **Your data** for the rest of what Taibu writes about you.

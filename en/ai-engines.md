# AI engines

Taibu AI OS can run on three different AI engines. Pick yours in **Settings → AI Engine**. Your projects, files, and skills stay the same — only the AI that does the work changes.

## The three engines

| | Claude Code | OpenAI Codex | Local model (Ollama) |
|---|---|---|---|
| **You need** | Claude subscription (Pro/Max) | ChatGPT subscription (Plus/Pro/Team) | A decent computer, nothing else |
| **Cost** | Your existing subscription | Your existing subscription | Free — runs on your machine |
| **Internet** | Required | Required | **Not required** — fully offline |
| **Quality** | Best — full experience | Very good | Depends on the model and your hardware — noticeably weaker on complex, multi-step work |
| **Skills (/onboard, /audit…)** | Native | Yes — Taibu copies them where Codex looks | Yes, but see the warning below |
| **Routines** | Yes | Yes | Not recommended |
| **Connecting tools (MCP)** | Yes | Yes, its own registry | Yes, same as Codex |
| **Gmail / Drive / Calendar** | Yes | **No** — those are Claude account connectors | **No** |

**Our recommendation:** Claude Code for the full experience. Codex if you already pay for ChatGPT and not for Claude. Local models when privacy or offline work matters more than polish.

## Claude Code (default)

1. Install: `winget install Anthropic.Claude` (the app also offers this on first run)
2. Sign in with your Claude subscription — the app guides you.

## OpenAI Codex

1. Install: `npm install -g @openai/codex`
2. Settings → AI Engine → **OpenAI Codex** — the app opens `codex login`; sign in with your ChatGPT account in the browser.
3. That's it. Your project instructions work automatically (the workspace ships an `AGENTS.md` that Codex reads).

## Local model (Ollama)

Runs entirely on your machine — nothing leaves your computer. Good for sensitive data and offline work.

1. Install [Ollama](https://ollama.com) and pull a coding model, e.g.: `ollama pull gpt-oss:20b`
2. Install Codex CLI (it drives the local model): `npm install -g @openai/codex`
3. Settings → AI Engine → **Local model (Ollama)**. The model picker lists whatever models Ollama has.

**Honest expectations:** a local model is not Claude, and the gap is bigger than it looks. Taibu gives a local model the same instructions, memory and skills as any other engine, so the plumbing is not the limit — the model is. A small model (around 4B) reasons at length and then fails to call a tool at all, which means it cannot edit files, run commands or use a connected tool. Use 20B or larger if you want it to actually do work rather than just write text, and try your real workflow before committing to it.

Scheduled routines on a local model are not recommended for the same reason: an unattended run that cannot use tools produces nothing useful.

## What changes when you switch

Taibu keeps the experience the same on every engine, and does the translating for you:

- **Your instructions** go to Claude directly, and to the others through `AGENTS.md`, which they read automatically.
- **Your skills** are copied into the folder each engine looks in. Claude reads `.claude/skills`, Codex and local models read `.agents/skills`. You do not have to think about it.
- **Slash commands** like `/onboard` work everywhere. Only Claude recognises them by itself, so on other engines Taibu expands the command before sending it.
- **Routines** run on whichever engine you have chosen. The Routines page tells you which one, and warns you if it is not ready.
- **Connected tools** are per engine: Claude and Codex each keep their own list, so a tool connected on one is not automatically there on the other.

Two things stay Claude-only, honestly: **Gmail, Google Drive and Google Calendar**, because those are connectors on your Anthropic account rather than something Taibu installs, and the **permission floor** that blocks dangerous commands in every mode. On other engines, scheduled work runs in a sandbox that keeps it inside your project instead.

## Switching engines

Switching is instant and safe — it changes which AI answers, not your data. Each chat session belongs to one engine; after switching, start a fresh message and the new engine picks up the project from its files (CLAUDE.md / AGENTS.md, memory.md, context/).

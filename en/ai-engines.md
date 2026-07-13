# AI engines

Taibu AI OS can run on three different AI engines. Pick yours in **Settings → AI Engine**. Your projects, files, and skills stay the same — only the AI that does the work changes.

## The three engines

| | Claude Code | OpenAI Codex | Local model (Ollama) |
|---|---|---|---|
| **You need** | Claude subscription (Pro/Max) | ChatGPT subscription (Plus/Pro/Team) | A decent computer, nothing else |
| **Cost** | Your existing subscription | Your existing subscription | Free — runs on your machine |
| **Internet** | Required | Required | **Not required** — fully offline |
| **Quality** | Best — full experience | Very good | Depends on the model and your hardware — noticeably weaker on complex, multi-step work |
| **Skills (/onboard, /audit…)** | Native | Works via AGENTS.md bridge | Works via AGENTS.md bridge, less reliable |

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

**Honest expectations:** a local 20B model is not Claude. Simple tasks (drafts, summaries, file edits) work well. Long multi-step automations and the guided skills may need more hand-holding. Try your real workflow before committing to it.

## Switching engines

Switching is instant and safe — it changes which AI answers, not your data. Each chat session belongs to one engine; after switching, start a fresh message and the new engine picks up the project from its files (CLAUDE.md / AGENTS.md, memory.md, context/).

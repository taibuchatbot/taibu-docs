# Settings and engines

**Gear icon → "Settings"**, with General, My data and goals, Keys and Memory tabs.

**My data and goals** is where your profile lives: who you are, what you sell, your priorities for the quarter, your writing samples. It used to sit behind its own icon in the left rail. Saving it hands off to the AI, which re-reads it and rebuilds your context files.

![Settings, the General tab](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/26-settings.png)

| Setting | What it does |
|---|---|
| **Open on start** | Land on Home or Chat |
| **Show technical details in chat** | Show the commands and file reads the AI runs |
| **AI model / Permission mode / Effort** | Settings for the current agent |
| **LANGUAGE** | App language and the language of new projects. Restarts the app |
| **AI ENGINE** | Claude Code, OpenAI Codex, or a local model |
| **CLAUDE STATUS** | Whether it is installed and signed in |
| **GITHUB** | Connect GitHub so Taibu can work with your repositories |
| **LICENSE** | Your plan, computer allowance and project count |
| **VERSION** | Which build you are on |

The theme toggle is not in Settings. It is in the top-right corner, next to the window buttons.

The Advanced controls change the **current agent**, the same values as the composer's settings pill. They are not global defaults.

## Engines

| Engine | Needs | Notes |
|---|---|---|
| **Claude Code** | Claude Pro, Max or Team, or Anthropic API billing | The full experience |
| **OpenAI Codex** | ChatGPT Plus, Pro or Team, plus the Codex CLI | Works, slightly fewer interactive touches |
| **Local model (Ollama)** | Ollama running with a pulled model, plus the Codex CLI | Fully offline and private. Slower, and weaker at multi-step work |

Switching an agent's engine starts a fresh conversation, because sessions cannot move between engines. Your files and memory are unaffected.

Routines always run on Claude, whichever engine you picked for chats.

**Models:** Sonnet is balanced and the default, Opus for the hardest work, Haiku fastest for simple tasks.

## Updates

Skills, instructions and templates update themselves quietly and safely. Everything is signed, and anything you edited yourself is never overwritten.

The app itself does not auto-update. When a new version exists, a purple bar at the top of Home says "Version X is out" with a Download button. Settings shows the same next to your version number. Either one downloads the installer for you.

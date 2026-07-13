# Start here

Taibu AI OS is your personal AI operating system. This guide helps you get a result in the first hour.

## What is it?

Taibu AI OS connects Claude AI to your project files, tools, and way of thinking. You don't just ask AI questions — you build yourself a personal operator that knows your business.

## First steps

### 1. Sign in to Claude

On first launch, a sign-in guide opens. Choose whether you use a Claude subscription (Pro/Max/Team) or API billing, and follow the steps. You can check the status anytime under **Settings → CLAUDE STATUS**.

### 2. Create your first project

Click the **project picker** button at the top left ("Pick a project"), then **"Add project…"**. Enter a project name (e.g. a client's name). Taibu copies the whole template structure automatically.

### 3. Run /onboard

Type in the chat:

```
/onboard
```

Claude asks you 7 questions — who you are, what you do, which tools you have. The answers are saved to the `context/` folder and make every later conversation much more accurate.

### 4. Talk to Claude

The chat works like Claude.ai, but Claude sees your project files and can edit them directly. Ask something specific:

- *"Look at intake.md and tell me what's missing"*
- *"Draft an email for a new client in property management"*
- *"What could I automate in my workflow?"*

### 5. Connect your tools

Next to the chat box there's a **+** button. From there you pick a popular connection — Google Drive, Gmail, Notion, Slack, etc. — and Claude walks you through the setup. That's how Claude gets to work with your real data.

You can attach a file to the chat with the **paperclip** icon (images, documents). To connect GitHub, see **Settings → GITHUB**.

### 6. Edit files directly

Click a file in the file tree on the left (e.g. `CLAUDE.md` or `intake.md`). The file opens as editable text. **Ctrl+S** saves. HTML files can also be viewed as a preview, and images open as images.

### 7. Run /audit after a week

```
/audit
```

Claude reviews what's done and what's missing. Good practice: once a week.

---

## Quick reference

| Command | What it does |
|------|----------|
| `/onboard` | Sets up the project (fills the context folders) |
| `/audit` | Gap report — what's missing |
| `/level-up` | The weekly 3M interview |
| `/roast` | Tests an idea with a 5-persona council |
| `/clear` | Clears the chat (starts a new session) |

# Chat and agents

An **agent** is one chat tab dedicated to one goal. Separate goals into separate agents and each stays focused.

- **+** on the tab bar starts a new agent
- **Double-click or right-click** a tab to rename it
- Switch away and it keeps working; the answer waits for you
- Closing an agent with real content moves it to "Recently closed" on Home, where you can reopen it

The **Agents** panel lists every agent you have started, under **Active** and **Closed**. An open one offers **Close**, which keeps the agent and its conversation. A closed one offers **Open** and delete.

![Four agents, one per goal](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/11-agents.png)

## The composer

Type and press Enter. Shift+Enter makes a new line.

| Control | What it does |
|---|---|
| **+** | Connect a tool |
| **Actions** | Run a skill, in its own new agent |
| **Settings pill** | Engine, model, effort and permissions for this agent |
| **Paperclip** | Attach a file as context |
| **Send / Stop** | Send, or interrupt what is running |

Typing **/** opens commands: /clear, /compact, /help, /model, /status. Skills are slash commands too, like /roast.

![The slash command menu](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/12b-slash.png)

## Reading the answers

Answers arrive as normal text with clickable links. Along the way you may see:

- **Proposed route** cards for plans, with "Approve route" and "Adjust"
- **Tool cards** showing what it did: edited a file, ran a command. Filenames are clickable
- **Images and video** inline, and documents as clickable chips
- A **"{n} background steps"** chip folding away routine work. Click the chip to unfold that one answer. To see them everywhere, tick **"Show technical details in chat"** in Settings

![An answer with a plan and tool cards](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/13-answer.png)

## Permissions

Set per agent in the settings pill:

| Mode | What it does |
|---|---|
| **Fully automatic** | Edits files and runs commands without asking. This is the default |
| **File edits only** | Changes files, runs no commands |
| **Plan first** | Reads and plans only. Changes nothing |

A safety floor applies in every mode, including fully automatic. Taibu refuses to delete your drive or home folder, use sudo, shut the machine down, force-push over git history, or publish packages. The AI cannot talk its way around these.

**Effort** controls how hard it thinks: Auto, Fast, Balanced, Deep.

![Engine, model, effort and permissions for this agent](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/14-agent-settings.png)

## Plans

When Taibu proposes a multi-step plan you get a "Proposed route" card. "Approve route" tells it to proceed; "Adjust" lets you say what to change.

In "Plan first" mode a "Run plan" button also appears after a planning turn.

Approving a plan switches that agent to Fully automatic for the rest of the session. Any message you type while a plan is pending counts as approval too. Re-pick "Plan first" to go back to planning.

## Stopping

**Stop** interrupts the turn and keeps whatever was already written. **/clear** wipes the conversation and starts fresh; your files are untouched.

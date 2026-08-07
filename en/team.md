# Working as a team

**People icon → "Team"**

Team sharing lets a group work from the same company knowledge. Everything shared is **encrypted on your own computer** before it goes anywhere, and it syncs through infrastructure **you own**. Nothing passes through a Taibu server.

## How it works

The team leader creates **scopes** (audiences, like sales, marketing, or one per client), decides who is in each, and picks what gets shared. A teammate without a scope's key genuinely cannot read that scope, even if they can see the sync folder.

## Where it syncs

| Option | Good for |
|---|---|
| **Shared folder** | Simplest and fastest. Point it at a folder kept in sync by Syncthing, a NAS or a cloud drive |
| **Git repository** | Your own private repo, with full history. Everyone must be signed in to git first |

For a git repository, each person needs git signed in on their machine before it will work. Run `gh auth login`, or clone the repo by hand once so the login is remembered. Taibu never stores your token, so it relies on your system's git login. If this is missing, the Team page tells you.

## Setting up (leader)

1. **"Create a team"**, name it, pick folder or git
2. Add a **scope**, for example `company`
3. Turn on what should be shared
4. Copy the **team code** and send it to your colleagues

## Joining (member)

1. Paste the team code under **"Join a team"**
2. Press **"Sync now"**. You will see "Waiting for your admin"
3. Your leader approves you with one click, and your access arrives on the next sync

You only ever send one code.

## What you can share

Company playbook, company rules, memory, company context, skills, references, decisions, tools, and any folder you pick.

## One way or both ways

Each item has a **"Who can change this"** setting:

- **Only me** — the leader's copy is the truth. Members read it; their changes never propagate. Use this for company canon
- **Anyone in scope** — two-way. Everyone contributes and receives. Use this for shared memory

Conflicting edits keep the newest version and save the other alongside it, so nothing is lost.

## Company rules without overwriting anyone

Your instructions file mixes company doctrine with personal things like your name, language and priorities, so Taibu never syncs that file.

Instead the leader writes the company rules in one place, and each member's Taibu adds them to their own instructions in a marked-off block. Personal settings stay untouched. Change a rule and everyone gets it.

## What is never shared

**Your personal profile and your voice never leave your computer**, whatever the settings say. Everyone keeps their own way of writing. Memory with no scope is private, and that is the default.

## Team insights

The leader can switch on activity reports. Each member decides whether to take part and sees exactly what would be sent.

**Sent:** how many conversations and with which agents, how memory grew, topic and skill names, activity per day, and where work seems to get stuck.

**Never sent:** what you wrote or the AI replied, your drafts, your private memory, your keys, anything personal.

Nothing is sent until you agree, and you can stop at any time.

## Limits worth knowing

- Removing someone is forward-looking. Their keys are replaced so they receive nothing new, but copies already synced stay on their machine
- The leader's device holds the team's master key. Back it up like a password
- Sharing is for knowledge, not media. There is a size limit per scope
- Team membership is per project. Connecting one project leaves your others untouched

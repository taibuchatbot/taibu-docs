# Skills

Taibu AI OS's capabilities can be extended with skills. A skill is a single Markdown file that tells Claude how to behave in a given situation. The system uses Claude Code's native `/skills` mechanism.

## Structure

Skills live in the project's `.claude/skills/` folder:

```
.claude/skills/
  hubspot-contact/
    SKILL.md
  email-draft/
    SKILL.md
```

Each `SKILL.md` has two parts:

```markdown
---
name: hubspot-contact
description: Use when the user says "add a contact", "new HubSpot customer", or asks about HubSpot
---

Here you write instructions for Claude in exactly the style it should follow.
For example: which fields to ask for, in what order to act, how to call the API.
```

`description` is the most important field — it determines when Claude applies the skill.

## Editing a skill — no markdown needed

When you open a `SKILL.md` file, Taibu AI OS shows it as a **form** instead of raw markdown: the name, description, and each section become input fields. Type into the fields and press **Ctrl+S** — the file stays valid, so you can't accidentally break the frontmatter or headings.

Need to restructure or add a section? Click **Raw** in the top-right of the editor to switch to the source, and **Form** to switch back. New skills open in Form view automatically.

## Where to find skills

**[skills.sh](https://skills.sh/)** — a skills catalog. Find ready-made skills for various tools and workflows. Copy the SKILL.md content into the right folder.

**GitHub** — many developers share skills in public repos. Just give Claude the link and ask it to install:

> *"Install this skill: https://github.com/user/repo"*

Claude downloads the SKILL.md and puts it in the right folder.

**Build your own** — tell Claude what you need:

> *"Make me a skill that helps me add HubSpot contacts — asks for name, email, and company, and adds them via the API"*

Claude creates the file, and next time it knows exactly what to do.

## The /find-skills command

Type in the chat:

```
/find-skills
```

Claude helps you find suitable skills based on your workflows and connected tools. Skills can be searched from skills.sh, GitHub, and other sources.

## Examples in practice

- **Customer management** — a skill that knows how to add a HubSpot contact, create a deal, write a note
- **Invoices** — a skill that generates a QuickBooks invoice in the right format
- **Content** — a skill that writes LinkedIn posts in your voice register (from Q2)
- **Weekly review** — a skill that produces a meeting summary in a set structure

One skill = one workflow you no longer have to remember.

# The Outbox

**Inbox icon → "Outbox"** — nothing goes out until you say so.

Every email, post or message Taibu prepares lands here as a draft. The amber number on the rail tells you how many are waiting.

## Reviewing

The right pane shows which routine or skill produced it, the recipient, and the body. The body is read-only until you say how you want to change it, so you always know which you are doing:

- **Edit myself** puts the cursor in the text. Change what you like, then **Save changes**. Until you save, the draft is marked "Edited, not saved yet", and **Discard changes** puts it back.
- **Edit with agent** hands the draft to an agent for a full rewrite.

![A draft waiting for approval](https://raw.githubusercontent.com/taibuchatbot/taibu-docs/main/images/19-outbox.png)

| Button | What it does |
|---|---|
| **Approve & send** | Marks it approved, then delivers it |
| **Edit myself** | Makes the text editable. **Save changes** writes it back |
| **Edit with agent** | Opens the draft in an agent for a full rewrite |
| **Skip** | Moves you to the next draft. It does **not** reject this one, which stays waiting |
| **Trash** | Discards the draft, with an Undo option |

## What "sent" means

Some connections can only create a draft, not send. The Gmail account connector is the common example: it can put the message in your Gmail drafts folder but cannot send it.

Taibu is instructed never to claim it sent something it only drafted. Check your sent folder the first time you use a new channel, so you know which behaviour you are getting.

## Why you can trust it

The rule is enforced in three places: routines are forbidden from sending, the app rather than the AI owns the approved state, and the app never talks to outside services itself. The AI cannot approve on your behalf.

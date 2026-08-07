# Troubleshooting

**"Claude isn't installed" or "Claude isn't signed in"**
Click the banner and follow the sign-in helper. If it still fails after installing, restart Taibu so it can find the newly installed program.

**Your sign-in expired**
Normal after a long gap, a password change, or signing out elsewhere. Settings → "Sign in again", finish in the browser, and carry on where you left off.

**A message spins, or stops with nothing**
Press Stop and send again. If it keeps happening, /clear starts a clean session. Your files and memory are safe.

**"That session ended"**
Usually after switching engines. Send your message again.

**A routine did not run**
Taibu must be **open** for routines to fire. Check the routine is switched on and read its last-run line. If it says you were signed out, use the "Sign in again" button there.

**Team sync is not working**
Open the Team page and read the message at the top. With a git repository it is almost always that git is not signed in on that computer.

**A shared folder says it is too large**
There is a size limit per scope. Share big documents or media with your team directly; team sync is for knowledge.

**An app is blank**
Its server is not running. Press "Start server", then "Reload".

**A local model is very slow**
Expected on ordinary hardware. Use Claude for anything demanding.

## Where your data lives

Everything is in your projects folder. Nothing is stored on a Taibu server.

Your instructions, profile, company knowledge, memory, decisions, skills and keys are all plain files in the project. Chats, routines, briefs and the outbox live in a hidden folder inside it.

To back up, copy the project folder or use "Export (zip)". To move computers, install Taibu, activate, then "Import (zip)…".

**What leaves your computer:** your messages go to whichever AI engine you chose, under their business terms. A local model sends nothing at all. Team sharing sends only encrypted content, only to the location your team controls. Licence checks send your key and an anonymous machine identifier. That is all.

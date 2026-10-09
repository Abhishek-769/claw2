# claw2

**A local, self-checking AI coding agent for the terminal.**
Your models and your code stay on your machine.

> **Status:** private research project, in active development since July 2026.
> The source is not published at this time. This page describes what the
> system does, not how it does it.

---

## What it is

claw2 is an AI coding assistant that lives in your terminal and works on your real projects. It reads and edits code, runs commands and tests, researches on the web, and remembers what it learned about each project.

What sets it apart is that **it does not trust itself.** Local open-weight models are private and free to run, but they make confident mistakes. claw2 is built around catching those mistakes:

- Independent AI reviewers check risky work.
- Claims of "done" are checked against what actually happened.
- Long unattended jobs are watched and handed back to a human when they get stuck.

---

## Highlights

- 🔒 **Local-first.** Models run on your hardware, and your code is never sent to a model provider.
- 🧠 **Per-project memory** that learns as you work.
- ⚖️ **MAGI**, a panel of LLM judges that reviews the agent's work.
- 🌙 **Unattended jobs.** Give it a goal, walk away, and read the report later.
- 📱 **It asks before it guesses.** A stuck job can reach you on your desktop or phone.
- 🛡️ **Layered safety** for commands, file edits and web content.
- 🎨 **A distinctive terminal look**, with rich rendering of answers, tables, code and diffs.
- 🧪 **Measured, not vibes.** Changes are tested and evaluated before they stay.

---

## Feature tour

### Conversations
- Named chats that keep their history across restarts.
- Saved sessions you can resume.
- Long conversations are condensed automatically, so nothing important silently disappears.
- Quick side questions that don't derail the main task.
- An optional "think first" mode.

### Workspaces
- Register your projects and switch between them instantly.
- Each project's environment is set up for the agent automatically.
- Project instructions and drop-in skills are picked up automatically.

### Memory
- A knowledge base per project and per conversation.
- Search, edit and forget memories whenever you like.
- Stale knowledge is retired automatically.

### MAGI: LLM judges
- A panel of AI judges can review the agent's answers and changes.
- They approve or block risky actions before those actions run.
- They screen web content before the agent reads it.
- They review a finished job before it is allowed to report success.

### Unattended jobs
- Describe a goal. A short interview first settles what "done" means.
- By default, jobs **never touch your real files**. You review the result and approve it.
- Jobs know when they're stuck and come back to you instead of wasting hours.
- Answer a job's questions or steer it while it runs.
- Every job ends with a written report.
- Lessons carry over to later jobs.

### Automation
- Run jobs on a schedule.
- Trigger jobs automatically when something you care about changes.

### Safety
- Choice of permission levels, from read-only to full access.
- "Always allow" and "never allow" decisions are remembered.
- Dangerous commands are refused.
- Unattended jobs are kept inside their own area.
- Automatic backups of every file the agent edits, with easy restore.
- Broken edits are caught immediately.
- Web content is treated as untrusted.

### Honesty checks
- A warning appears when the agent claims work it never did.
- Goals are marked complete only after an independent check.
- The agent is stopped when it starts going in circles.

### Answer quality
- Several candidate answers can be generated, and the best one kept.
- Answers are shaped to fit the question: short when short is right, and structured when structure helps.

### Also
- Web search and browsing, with adjustable limits.
- Experimental image and audio understanding.
- A browser UI, and a phone relay for answering jobs on the go.

---

## Commands

| Command | Purpose |
|---|---|
| `/help` | All commands |
| `/status` | Session overview |
| `/model` | Switch model |
| `/permissions` | Set the permission level |
| `/chat` | Manage conversations |
| `/workspace` | Manage projects |
| `/memory` | Manage memory |
| `/thinking` | Think-first mode |
| `/magi` | LLM judge panel |
| `/auto` | Start an unattended job |
| `/jobs` | Watch, answer and control jobs |
| `/goal` | Set and track a goal |
| `/orders` | Remembered allow and deny decisions |
| `/rules` | Scheduled and automatic jobs |
| `/backups` | Restore earlier versions of files |
| `/web` | Web access |
| `/diverge` | Best of several answers |
| `/shape` | Answer shaping |
| `/claim` | Honesty warnings |
| `/compact` | Condense the conversation |

---

## Requirements

- Linux
- A local model server, with one or more open-weight models
- A GPU is recommended

---

## Privacy

- Models run locally, and your code is never sent to an AI provider.
- Web search, phone notifications, email and the phone relay contact outside services, and only when you turn them on.

---

## Provenance

Designed and built by **Abhishek Kalyankar**, 2026.

Source snapshot fingerprint (SHA-256 of a private archive, kept unchanged by the author):

```
7cf017c885bff3c0679a144fded9a493055ceb1f99737be66a7a369b77f12a8e  claw2-src-20261009.tar.gz
```

Snapshot date: 2026-10-09.

---

## License

**All rights reserved.** No license is granted to use, copy, modify, or distribute this software or its design. This README may be shared unmodified.

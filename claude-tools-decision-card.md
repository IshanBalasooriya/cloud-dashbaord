# Claude Tools: Decision Framework

A reference card for choosing between Claude.ai, Claude Code, and Cowork.

---

## The 10-Second Decision

Ask yourself these three questions in order:

| Question | If yes → |
|---|---|
| Am I **thinking through** something, or exploring data I can upload? | **Claude.ai** |
| Is the work **inside a codebase** — source files, git, tests, a dev server? | **Claude Code** |
| Do I want to **hand off a multi-step task** on my own files and get a finished deliverable back? | **Cowork** |

The underlying split:

- **Claude.ai** — a *conversation you steer*, turn by turn.
- **Claude Code** — a *collaborator in your repo*, with the terminal and git.
- **Cowork** — a *delegation you describe once*, then check on.

---

## 1. Claude.ai (Browser Chat)

**Best for**
Exploratory thinking, Q&A, drafting, and quick analysis of files you upload. Artifacts let you generate an interactive chart, doc, or app that renders right in the conversation and can be revised in place.

**When to use it**
- The task is light on context — one file or a few, not a folder tree
- You want to iterate fast and change direction mid-conversation
- You're on a machine where nothing is installed, or on mobile
- The output is something you'll read, copy elsewhere, or share as a link

**When *not* to use it**
- The work spans many local files (you'd be uploading forever)
- You need Claude to run commands or modify files on your machine
- You want to walk away and come back to finished work

**Your example**
Upload a CSV → ask questions about the data → get an interactive chart Artifact you can tweak by asking for changes.

---

## 2. Claude Code (Terminal / IDE Agent)

**Best for**
Real software work. Claude reads your codebase, plans across multiple files, writes and modifies code, runs commands and tests, and corrects itself — with git tracking every change so you can roll back.

**When to use it**
- The deliverable is *code* that has to run, not a description of code
- The task touches several files and needs project-wide understanding
- You want to run, test, and debug in the same loop as writing
- You need full access to your file system, terminal, and dev tools

**When *not* to use it**
- The task isn't technical (you'd be paying a setup cost for nothing)
- You don't want a terminal in the picture — use Cowork instead
- You just need a quick answer or a one-off snippet

**Your example**
Point it at a local project → have it read the data files, write the JS, and build an HTML dashboard with Chart.js you can open and iterate on.

---

## 3. Cowork (Claude Desktop App)

**Best for**
Agentic knowledge work without a terminal. You state an end goal instead of asking a question; Claude reads and writes files in the folders you share with it, works through multi-step tasks, and hands back finished documents, spreadsheets, or decks.

**When to use it**
- The task has a clear deliverable and touches a spread of files
- It's tedious and multi-step — sorting, renaming, extracting, summarizing
- You want to describe it once and step away rather than steer each turn
- You want it to happen on a schedule (daily, weekly, monthly)

**When *not* to use it**
- You're still figuring out what you want — that's a chat, not a delegation
- The work is inside a codebase and needs git and a test loop
- You need it to touch folders you haven't granted access to

**Your example**
Point it at a messy folder → have it sort files into subfolders by type and date, then write a summary document describing what it found and what it did.

---

## Same Task, Three Ways

A useful gut-check. Say you have a folder of sales data:

| Tool | What you'd get |
|---|---|
| **Claude.ai** | Upload one CSV, ask "what's driving the Q3 dip?", get an Artifact chart back in five minutes |
| **Claude Code** | A real dashboard app in your repo — data pipeline, chart components, git history, runs locally |
| **Cowork** | All 40 files read, cleaned, merged into a formatted spreadsheet plus a written summary, delivered while you were at lunch |

Same data. Different question being asked of the tool.

---

## Rules of Thumb

1. **Conversation vs. deliverable.** If you want to think out loud, that's chat. If you want a finished file, that's Cowork or Code.
2. **Uploading files is a smell.** More than two or three uploads means you've outgrown chat — move to a tool with local access.
3. **Terminal is the fork between Code and Cowork.** Code work needs git and a run/test loop; document and file work doesn't.
4. **Cowork's blast radius is what you grant it.** It works in a contained workspace limited to the folders you share, and asks before consequential actions. Claude Code runs directly in your project with fuller access — worth knowing which you're in.
5. **Start in chat when unsure.** It's the cheapest place to discover what you actually want, then escalate.

---

## Quick Notes

- Chat, Cowork, and Code all live inside the Claude Desktop app as three modes — Cowork and Code are also available elsewhere, but the desktop app is where they reach your local files.
- Cowork also runs on web and mobile, though local file access is desktop-only.
- Cowork is on the paid plans (Pro, Max, Team, Enterprise), not Free.
- Anthropic's own comparison of the three desktop modes:
  https://claude.com/resources/tutorials/navigating-the-claude-desktop-app

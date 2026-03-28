# Recommended Plugins and Tools for Claude Code

A curated list of plugins, skills, and tools that enhance Claude Code. All of these come from GitHub and are free to use with your Claude Pro subscription.

---

## How to Install Plugins

Inside Claude Code, type:

```
/install-plugin
```

Then paste the GitHub URL when prompted. That's it — no GitHub account needed for public repos.

For standalone tools (like Visual Explainer), clone them separately:

```bash
git clone <url>
cd <folder-name>
claude
```

---

## Official Anthropic Plugins

These come from Anthropic (the company that makes Claude) and are well-maintained and reliable.

### 1. Document Skills

| | |
|---|---|
| **Source** | `anthropics/skills` |
| **Install URL** | `https://github.com/anthropics/skills` |
| **What it does** | Create and edit real documents — PDFs, Word docs, spreadsheets, and PowerPoint presentations — all from within Claude Code |
| **Why it's useful** | Turns Claude Code into a document creation tool. Ask it to make a spreadsheet, a report, or a slide deck and it generates the actual file |
| **Skills included** | `/pdf`, `/docx`, `/xlsx`, `/pptx`, `/canvas-design`, `/algorithmic-art`, `/frontend-design`, `/webapp-testing`, `/mcp-builder`, `/skill-creator` |

### 2. Playground

| | |
|---|---|
| **Source** | `anthropics/claude-plugins-official` |
| **Install URL** | `https://github.com/anthropics/claude-plugins-official` |
| **What it does** | Creates interactive HTML playgrounds — self-contained single-file web apps you can explore in your browser |
| **Why it's useful** | Great for experimenting. Ask Claude to build a mini app, game, or visualisation and it creates something you can immediately open and interact with |
| **Skill** | `/playground` |

### 3. Frontend Design

| | |
|---|---|
| **Source** | `anthropics/claude-plugins-official` |
| **Install URL** | `https://github.com/anthropics/claude-plugins-official` |
| **What it does** | Generates production-quality frontend interfaces with modern design principles |
| **Why it's useful** | If you're building a website or app, this plugin ensures Claude creates beautiful, professional-looking UIs rather than basic unstyled HTML |
| **Skill** | `/frontend-design` |

### 4. Playwright (Browser Automation)

| | |
|---|---|
| **Source** | `anthropics/claude-plugins-official` |
| **Install URL** | `https://github.com/anthropics/claude-plugins-official` |
| **What it does** | Automates web browsers — Claude can navigate websites, fill in forms, click buttons, and take screenshots |
| **Why it's useful** | Test your web projects automatically, scrape information from websites, or automate repetitive browser tasks |

### 5. Plugin Dev

| | |
|---|---|
| **Source** | `anthropics/claude-code` |
| **Install URL** | `https://github.com/anthropics/claude-code` |
| **What it does** | A guided workflow for building your own Claude Code plugins — skills, agents, hooks, and slash commands |
| **Why it's useful** | Once you're comfortable with Claude Code, this lets you extend it with your own custom tools. The ultimate power-user move |
| **Skills included** | `/create-plugin`, `/skill-development`, `/agent-development`, `/hook-development`, `/command-development` |

### 6. Claude MD Management

| | |
|---|---|
| **Source** | `anthropics/claude-plugins-official` |
| **Install URL** | `https://github.com/anthropics/claude-plugins-official` |
| **What it does** | Helps you create and maintain `CLAUDE.md` files — the project configuration files that tell Claude how to work with your code |
| **Why it's useful** | `CLAUDE.md` is how you teach Claude about your project's conventions, structure, and preferences. This plugin helps you write and improve them |
| **Skills included** | `/revise-claude-md`, `/claude-md-improver` |

### 7. Supabase

| | |
|---|---|
| **Source** | `anthropics/claude-plugins-official` |
| **Install URL** | `https://github.com/anthropics/claude-plugins-official` |
| **What it does** | Integrates with Supabase — a backend-as-a-service platform for databases, authentication, and hosting |
| **Why it's useful** | If you want to build a full-stack app with a database, this plugin lets Claude manage your Supabase project directly |

### 8. Vercel

| | |
|---|---|
| **Source** | `anthropics/claude-plugins-official` |
| **Install URL** | `https://github.com/anthropics/claude-plugins-official` |
| **What it does** | Deploy your web projects to the internet via Vercel with a single command |
| **Why it's useful** | Go from code on your laptop to a live website in seconds. Great for showing off what you've built |
| **Skills included** | `/deploy`, `/vercel-logs`, `/vercel-setup` |

### 9. GitHub

| | |
|---|---|
| **Source** | `anthropics/claude-plugins-official` |
| **Install URL** | `https://github.com/anthropics/claude-plugins-official` |
| **What it does** | Integrates with GitHub for managing repositories, pull requests, issues, and code reviews |
| **Why it's useful** | If you're working on a team project or want to learn professional version control workflows |

---

## Community Plugins

These are built by the Claude Code community and available on GitHub.

### 10. Superpowers

| | |
|---|---|
| **Source** | `obra/superpowers-marketplace` |
| **Install URL** | `https://github.com/obra/superpowers-marketplace` |
| **What it does** | Adds structured professional development workflows — brainstorming, test-driven development, systematic debugging, planning, and code review |
| **Why it's useful** | Instead of just asking Claude to "write code", Superpowers teaches you to think like a professional developer. It forces good habits: plan before you build, test before you ship, review before you merge |
| **Key skills** | `/brainstorming`, `/test-driven-development`, `/systematic-debugging`, `/writing-plans`, `/executing-plans`, `/requesting-code-review` |

### 11. Next.js + Vercel Pro

| | |
|---|---|
| **Source** | `davila7/claude-code-templates` |
| **Install URL** | `https://github.com/davila7/claude-code-templates` |
| **What it does** | Templates and best practices for building modern web applications with Next.js and deploying to Vercel |
| **Why it's useful** | If you want to build a real web app (not just a static page), this gives Claude expert knowledge of the most popular React framework |
| **Skills included** | `/nextjs-scaffold`, `/nextjs-component-generator`, `/vercel-deploy-optimize` |

### 12. Claude Mem (Persistent Memory)

| | |
|---|---|
| **Source** | `thedotmack/claude-mem` |
| **Install URL** | `https://github.com/thedotmack/claude-mem` |
| **What it does** | Gives Claude Code a persistent memory database that survives across sessions — it remembers what you've worked on, decisions you've made, and context from previous conversations |
| **Why it's useful** | Without this, every new Claude Code session starts fresh. With it, Claude remembers your project history and can build on previous work |

### 13. AI Agent Builder

| | |
|---|---|
| **Source** | `dair-ai/dair-cc-plugins` |
| **Install URL** | `https://github.com/dair-ai/dair-cc-plugins` |
| **What it does** | Tools and patterns for building AI agents — autonomous programs that can reason, plan, and take actions |
| **Why it's useful** | For more advanced students interested in AI/ML. Learn how to build agents that go beyond simple chat |

---

## Standalone Tools (Clone from GitHub)

These aren't plugins — they're separate projects you clone and use alongside Claude Code.

### 14. Visual Explainer

| | |
|---|---|
| **Source** | `nicobailon/visual-explainer` |
| **Install URL** | `https://github.com/nicobailon/visual-explainer` |
| **What it does** | Generates beautiful, self-contained HTML pages that visually explain any concept — systems, code architecture, processes, algorithms |
| **Why it's useful** | Perfect for understanding how things work. Ask it to explain any concept and it creates an interactive visual page you can open in your browser |
| **How to use** | `git clone https://github.com/nicobailon/visual-explainer.git && cd visual-explainer && claude` |

---

## Where to Start

If you're new to Claude Code, install these first:

1. **Superpowers** — gives you professional workflows from day one
2. **Playground** — instant visual results, very motivating
3. **Document Skills** — practical output you can use for school work

Once comfortable, add:

4. **Frontend Design** — for building beautiful web UIs
5. **Visual Explainer** — for understanding any concept visually
6. **Vercel** — to deploy your projects live on the internet

---

## Note on GitHub Accounts

You do **not** need a GitHub account to install any of these. All repositories are public. The `/install-plugin` command and `git clone` both work without authentication for public repos.

You will need git installed:
- **Mac**: Comes with Xcode Command Line Tools (or install via Homebrew)
- **Windows**: Install [Git for Windows](https://git-scm.com)

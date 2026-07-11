# 🤖 AI Agent Skill Generator

A clean developer dashboard for generating structured skill definition files for AI coding agents — built with vanilla HTML, CSS, and JavaScript.

![License](https://img.shields.io/badge/license-MIT-blue)
![Built with](https://img.shields.io/badge/built%20with-Vanilla%20JS-yellow)
![API](https://img.shields.io/badge/API-OpenAI%20%7C%20Anthropic-purple)

---

## What It Does

AI coding agents like Codex, Claude Code, and Gemini CLI work best when given a structured skill file that defines their identity, responsibilities, and constraints for a specific project. This tool generates those files automatically.

You fill in the form. The AI produces a complete, ready-to-use `.md` skill file. You can edit it, preview it, copy it, or download it directly.

---

## Features

- **Agent selector** — supports Codex, Claude Code, Antigravity, and Gemini CLI
- **Structured form inputs** — project name, description, tech stack, role title, responsibilities
- **Output style picker** — Detailed, Concise, Structured, or Strict Rules
- **Live code editor** — editable after generation with line numbers
- **Three-tab viewer** — Generated Skill (editable), Preview (rendered markdown), Raw
- **One-click export** — Copy to clipboard or download as `.md` file
- **Generation history** — stored in localStorage, reload any previous generation
- **Dual API support** — works with OpenAI (`gpt-4o-mini`) or Anthropic (`claude-haiku`)

---

## Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/YOUR_USERNAME/ai-agent-skill-generator.git
cd ai-agent-skill-generator
```

### 2. Open the file

```bash
open skill-generator.html
```

Or just double-click `skill-generator.html` to open it in your browser. No server or build step required.

### 3. Add your API key

In the sidebar, paste your **OpenAI** or **Anthropic** API key. It is saved locally in your browser via `localStorage` — never sent anywhere except directly to the chosen API.

---

## How to Use

1. Choose your target AI agent (Codex, Claude Code, etc.)
2. Enter your project name and description
3. Define the agent's role and key responsibilities
4. Add your tech stack
5. Pick an output style
6. Click **Generate Skill**
7. Edit the result in the built-in code editor
8. Download as `.md` or copy to clipboard

---

## Generated Skill File Format

Each generated file follows this structure:

```markdown
# Codex Skill: Senior Full Stack Developer

## 1. Identity
## 2. Responsibilities
## 3. Technical Context
## 4. Working Style
## 5. Code Standards
## 6. Rules
## 7. Success Criteria
```

The file is designed to be dropped directly into your AI coding agent's context or project configuration.

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| UI | Vanilla HTML5 + CSS3 |
| Logic | Vanilla JavaScript (ES6+) |
| Fonts | Inter + JetBrains Mono (Google Fonts) |
| AI Generation | OpenAI API / Anthropic API |
| Storage | localStorage (no backend) |

---

## Project Structure

```
ai-agent-skill-generator/
├── skill-generator.html   # Complete app (single file)
└── README.md
```

---

## API Key Security

Your API key is:
- Stored only in your **local browser** via `localStorage`
- Sent only to **OpenAI or Anthropic** directly (no proxy, no backend)
- Never logged or transmitted elsewhere

---

## License

MIT — free to use, modify, and distribute.

---

Built as part of a structured series of developer tool projects.
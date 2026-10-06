# Rowen Web Dev

A Claude skill for building websites and web apps that look designed for their product instead of generated from a template. It covers design direction, typography, motion, forms, uploads, security, accessibility, performance, testing and launch reviews, and it asks Claude to show evidence before saying something works.

`SKILL.md` is a short router. It tells Claude which module to read for the task in front of it, such as a bug, a checkout form or a launch review, so the detailed guidance stays out of context until it's needed.

## Install

### Claude Code, as a plugin

Run these inside Claude Code:

```
/plugin marketplace add 0-Ghostly-0/rowen-web-dev
/plugin install rowen-web-dev@rowen-web-dev
```

Claude uses the skill on its own when a task matches its description. You can also call it directly with `/rowen-web-dev:rowen-web-dev`. Run `/plugin marketplace update rowen-web-dev` later to pick up new versions.

### Claude Code, as a personal skill

Copy the skill folder into your skills directory:

```bash
git clone https://github.com/0-Ghostly-0/rowen-web-dev.git
cp -r rowen-web-dev/skills/rowen-web-dev ~/.claude/skills/
```

It's then available as `/rowen-web-dev`. To share it with everyone working in one project, copy the folder into that project's `.claude/skills/` instead.

### Claude.ai and the Claude apps

Make a ZIP of the `skills/rowen-web-dev` folder so the ZIP contains a `rowen-web-dev` folder with `SKILL.md` inside it. In Claude, open Customize > Skills, click +, choose Create skill, then Upload a skill, and pick the ZIP. Skills need "Code execution and file creation" turned on under Settings > Capabilities.

## What's inside

| Folder | Covers |
| --- | --- |
| `design/` | Art direction, typography, motion, component polish, responsive layout, taste calibration |
| `engineering/` | Debugging, testing strategy, performance, code quality |
| `product/` | Forms and checkout, uploads, async and data states, UX writing, production edge cases |
| `quality/` | Accessibility, browser QA, verification before completion, visual design review, launch review, an anti-overengineering gate |
| `security/` | Risk-based security review |
| `references/`, `research/`, `workflows/` | The sources the skill drew on and notes on what was kept or left out |

## What it's opinionated about

The skill has defaults you should know about before installing it. It reaches for Next.js and TypeScript on Vercel. For small sites with one owner, it suggests a private `/admin` page behind a single random 40-character password kept in a server-only environment variable, and it recommends real accounts when a project needs per-person access. It treats Space Grotesk, purple and blue gradient branding, glass everywhere and fade-up animations on every section as warning signs of generated design, though not as hard bans. It prefers quiet, fast motion, and it never invents metrics, testimonials or other data.

Your own request and your project's existing design and architecture always come first. The skill's precedence list puts them above its own rules.

## Versions

- **4.1**: hover animations have to ease back to their resting state when the pointer leaves, instead of snapping back.
- **4.0**: added taste calibration, a restrained motion system, component-level polish, production edge cases, rendered visual design review and the anti-overengineering gate.
- **3.0**: brought in useful principles from public Claude and agent skills, with conflicts settled in favour of this skill's priorities. `research/merged-skill-decisions.md` lists what was taken and what was left out.

## License

[MIT](LICENSE)

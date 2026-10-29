# Master UI Skill

A design constitution, UI engineering playbook, motion system, resource atlas, and visual QA protocol for coding agents. Install it once as an agent skill — no special prompts required.

## What it does

Makes agents consistently produce distinctive, coherent, accessible, responsive, fast, and functionally complete interfaces — not generic template output. Thirty sections, ten non-negotiable articles, ten review phases, and an evidence-first workflow.

## How it works

Agents that support SKILL.md (e.g. OpenCode) load this skill when a UI task matches its description. You do not write a "generate UI" prompt; the agent follows the constitution instead.

## Install (OpenCode)

Global install:

```powershell
# Windows PowerShell
$dest = "$env:USERPROFILE\.config\opencode\skills\master-ui-skill"
New-Item -ItemType Directory -Force $dest | Out-Null
Invoke-WebRequest "https://raw.githubusercontent.com/shaikaakif/master-ui-skill/main/skills/master-ui-skill/SKILL.md" -OutFile "$dest\SKILL.md"
```

```bash
# macOS / Linux / Git Bash
mkdir -p ~/.config/opencode/skills/master-ui-skill
curl -fsSL https://raw.githubusercontent.com/shaikaakif/master-ui-skill/main/skills/master-ui-skill/SKILL.md -o ~/.config/opencode/skills/master-ui-skill/SKILL.md
```

Project install (version-controlled alongside your project):

```powershell
# PowerShell
$dest = ".opencode\skills\master-ui-skill"
New-Item -ItemType Directory -Force $dest | Out-Null
Copy-Item "SKILL.md" "$dest\SKILL.md"
```

```bash
# macOS / Linux
mkdir -p .opencode/skills/master-ui-skill
cp SKILL.md .opencode/skills/master-ui-skill/SKILL.md
```

## Files in this repository

| File | Purpose |
|------|---------|
| `SKILL.md` | The complete Master UI skill — loads into OpenCode-compatible agents |
| `LICENSE` | MIT License |
| `CONTRIBUTING.md` | How to contribute improvements |
| `.gitignore` | Standard ignores |

## License

MIT. See `LICENSE`.

## Credit

Inspired by OpenCode skill conventions, WCAG 2.2, Apple HIG, Material 3, Carbon, Polaris, shadcn/ui, Radix UI, Playwright, axe-core, UI UX Pro Max, Anthropic Frontend Design skill, Impeccable, and Vercel web-design-guidelines. No third-party code is bundled.
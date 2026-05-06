# Codex Gameforge Skill Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Create an installed Codex skill that converts Espotz learning-module PPT/sample prompts into a validated educational esports game production workflow.

**Architecture:** Create a lean top-level orchestration skill named `codex-gameforge` with progressively disclosed references for intake gates, production pipeline, NPC agent mapping, and validation pressure tests. The skill will require CODEX-CD for source learning design and CODEX-ARENA/game tooling for playable outputs, while leaving connector-heavy services optional unless explicitly needed.

**Tech Stack:** Codex skills, Espotz local agent skills, Presentations, SharePoint PowerPoint, Game Studio, Build Web Apps, HyperFrames, Sora, Hugging Face, Supabase, GitHub, Google Drive, validation via `quick_validate.py`.

---

### Task 1: Initialize Skill Skeleton

**Files:**
- Create: `C:/Users/CCE MSI/.codex/skills/codex-gameforge/SKILL.md`
- Create: `C:/Users/CCE MSI/.codex/skills/codex-gameforge/references/`
- Create: `C:/Users/CCE MSI/.codex/skills/codex-gameforge/agents/openai.yaml`

- [ ] **Step 1: Run the skill initializer**

Run:
```powershell
& 'C:\Users\CCE MSI\.cache\codex-runtimes\codex-primary-runtime\dependencies\python\python.exe' 'C:\Users\CCE MSI\.codex\skills\.system\skill-creator\scripts\init_skill.py' codex-gameforge --path 'C:\Users\CCE MSI\.codex\skills' --resources references --interface display_name='CODEX Gameforge' --interface short_description='Turns Espotz module decks and samples into educational esports games.' --interface default_prompt='Build an Espotz educational esports game from my module prompt and sample assets.'
```

Expected: a new `codex-gameforge` skill folder with `SKILL.md`, `references/`, and `agents/openai.yaml`.

### Task 2: Write the Skill and References

**Files:**
- Modify: `C:/Users/CCE MSI/.codex/skills/codex-gameforge/SKILL.md`
- Create: `C:/Users/CCE MSI/.codex/skills/codex-gameforge/references/intake-gates.md`
- Create: `C:/Users/CCE MSI/.codex/skills/codex-gameforge/references/production-pipeline.md`
- Create: `C:/Users/CCE MSI/.codex/skills/codex-gameforge/references/npc-agent-roster.md`
- Create: `C:/Users/CCE MSI/.codex/skills/codex-gameforge/references/validation-pressure-tests.md`

- [ ] **Step 1: Write a concise trigger description**

Use:
```yaml
---
name: codex-gameforge
description: Use when creating an Espotz educational esports game from a learning module prompt, sample deck, PPTX, Google Slides, or CODEX-CD lesson package; when converting curriculum into a playable learning game, AcademyOS experience, NPC coach layer, avatar/video companion, homework templates, data-backed progression system, or deployable game build.
---
```

- [ ] **Step 2: Define the required workflow**

The skill must require context questions before production, separate educational-game design from gamified slides, route source learning content through CODEX-CD, route playable shell/game work through CODEX-ARENA/Game Studio, and require validation before delivery.

### Task 3: Validate and Forward-Test

**Files:**
- Read: `C:/Users/CCE MSI/.codex/skills/codex-gameforge/SKILL.md`
- Read: `C:/Users/CCE MSI/.codex/skills/codex-gameforge/references/validation-pressure-tests.md`

- [ ] **Step 1: Run basic skill validation**

Run:
```powershell
& 'C:\Users\CCE MSI\.cache\codex-runtimes\codex-primary-runtime\dependencies\python\python.exe' 'C:\Users\CCE MSI\.codex\skills\.system\skill-creator\scripts\quick_validate.py' 'C:\Users\CCE MSI\.codex\skills\codex-gameforge'
```

Expected: validation passes.

- [ ] **Step 2: Use parallel validation agents**

Dispatch independent agents to test whether the skill asks the right intake questions, avoids gamified-PPT shortcuts, preserves CODEX-CD/ARENA boundaries, and demands final artifact verification.

### Task 4: Fix Issues and Deliver

**Files:**
- Modify: any `codex-gameforge` files where validation exposes ambiguity.

- [ ] **Step 1: Patch validation gaps**

Update the skill or references to close any specific loopholes found by validation agents.

- [ ] **Step 2: Re-run validation**

Run `quick_validate.py` again and report installed path plus restart note.

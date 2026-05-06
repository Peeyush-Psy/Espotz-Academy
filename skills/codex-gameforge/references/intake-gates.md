# Intake Gates

Ask these questions in one block before production. Restate any answers the user already provided and ask only for missing fields.

## Required Questions

1. **Source package:** What are you giving me: prompt only, PPTX/sample deck, SharePoint deck, Google Slides, existing CODEX-CD folder, or hosted lesson URL/path?
2. **Track and tier:** Which Espotz track and tier: Player, Ops, Marketing, or Cast & Content; Spawn, Challenger, Pro, or Champ?
3. **Learning target:** What are the 3-5 observable skills the learner must practice in-game? Reject vague verbs like understand, know, learn, or be aware of.
4. **Game scope:** What should be built: prototype, one playable match, full AcademyOS module wrapper, 3D game, capstone, or production-ready deployable build?
5. **Platform and constraints:** Mobile/desktop target, session length, offline needs, school device limits, accessibility needs, login requirements, and whether Supabase/GitHub/Google/SharePoint are in scope.
6. **NPC and media scope:** Which NPC coaches, avatars, voiceovers, trailers, website-to-video captures, or learner templates are required now versus later?
7. **Evidence and safety:** Are there real tournaments, campaigns, people, or case studies cleared for use by name? Are there safeguarding, wellbeing, conduct, under-16, privacy, or parental/institution constraints?

## Readiness Rules

- If only a rough prompt exists, first produce a content intake summary and route through CODEX-CD.
- If a PPT/sample exists, extract concepts, claims, activities, assessments, media, and sources before proposing mechanics.
- If CODEX-CD outputs exist, confirm the `.pptx`, `.html`, instructor notes, asset folder, and manifest before wrapping.
- If any required answer is missing, ask. Do not start implementation.
- If the user requests "use all plugins", narrow the stack to the minimum needed and explain skipped tools briefly.

## Confirmation Format

After answers are complete, reply with:

- Source package:
- Track/tier:
- Observable skills:
- Game scope:
- Platform/data/deployment constraints:
- NPC/media/template scope:
- Evidence/safety constraints:
- Proposed stack:
- First deliverable for approval: game design brief and module-to-game map.

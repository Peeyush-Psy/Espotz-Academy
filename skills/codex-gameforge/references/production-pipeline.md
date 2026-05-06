# Production Pipeline

## Phase 1: Source and Learning Spine

Use CODEX-CD for lesson design when source content is incomplete. Use Presentations for PPTX extraction or creation. Use SharePoint PowerPoint only when the source deck lives in SharePoint or preserving SharePoint-hosted style matters. Use Google Slides only for Google-hosted source files or Google-native outputs.

Create:

- Module summary.
- Track/tier palette and voice.
- Observable skills.
- Concepts and misconceptions.
- Evidence/source table.
- Assessment moments and answer-key source.
- Media list and caption needs.
- Source-to-game traceability draft.

## Phase 2: Educational Game Design

Convert content into play:

- Learner fantasy: what role the learner inhabits in esports.
- Player verbs: analyze, call, draft, route, brief, clip, budget, negotiate, coach, review, adapt.
- Core loop: observe, decide, act, see consequence, reflect, retry.
- Mission beats: onboarding, practice, pressure round, reflection, career bridge.
- Feedback: specific, skill-linked, non-punitive.
- Assessment: attempt-gated, rubric-backed, never answer-leaking.
- Career path: skills, artifacts, roles, next module.

Reject designs where the learner mostly reads, clicks next, or collects points without making meaningful decisions.

## Phase 3: Stack Routing

Default path:

- `codex-arena` for AcademyOS shell.
- `game-studio:game-studio` for game type routing.
- `game-studio:web-game-foundations` for architecture.
- `game-studio:game-ui-frontend` for HUD and overlays.
- `build-web-apps:frontend-app-builder` for implementation.
- `game-studio:game-playtest` for verification.

Optional paths:

- React Three Fiber when 3D is explicitly chosen.
- Web 3D asset pipeline when GLB/glTF assets are needed.
- Transformers.js for local browser ML only with loading, error, and disposal handling.
- Supabase for auth, server progress, admin dashboards, or persistence. Verify current docs, use RLS, and never expose service-role keys.
- GitHub for repository, issues, PR, or deployment workflow.
- HyperFrames/Sora for media, trailers, avatar clips, voiceover, and website-to-video capture.
- Hugging Face Jobs/Trainer for explicit training or remote model jobs.

## Phase 4: Build Artifacts

Minimum playable package:

- `index.html` or app entry.
- Game runtime source.
- CSS/token files.
- Asset manifest.
- NPC routing manifest.
- Career/progression manifest.
- Module traceability map.
- README for running and plugging in new modules.

When requested:

- Supabase schema and policies.
- GitHub repo and PR summary.
- Google Docs/Sheets/Slides learner templates.
- Companion deck.
- HyperFrames/Sora videos or captures.
- Instructor/admin QA notes.

## Phase 5: Verification

Run:

- Build/test command for the chosen stack.
- Browser smoke test on desktop and mobile viewport.
- Screenshot inspection for first playable screen, HUD, NPC surfaces, and assessment moments.
- Keyboard and reduced-motion check.
- Console-error check.
- Content traceability check.
- Safety check for SHIELD access and no PII.
- Data/security check when Supabase or hosting is included.

Delivery must include what was verified and what was intentionally skipped.

# Codex / Claude — Visual Design Handoff

Use these materials to guide implementation:
1. [Original visual reference brief](VISUAL-RESEARCH.md)
2. [Illustrative landing concept](../research/visuals/01-landing-concept.svg)
3. [Illustrative dashboard concept](../research/visuals/02-dashboard-concept.svg)
4. [Illustrative studio concept](../research/visuals/03-video-studio-concept.svg)
5. [Illustrative approvals concept](../research/visuals/04-approval-center-concept.svg)
6. [UI references list](UI-REFERENCES.md)
7. [Design tokens](DESIGN-SYSTEM.md)
8. [Architecture rules](ARCHITECTURE.md)
9. [Task 01](CODEX-TASK-01.md)

## Copy this prompt

```text
You are designing OutreachOS, a premium EU B2B SaaS frontend.

Read docs/VISUAL-RESEARCH.md, docs/DESIGN-SYSTEM.md,
docs/ARCHITECTURE.md, docs/CODEX-TASK-01.md and STATUS.md.

Study the four original SVG design explorations in research/visuals.
Use them as a visual starting point, NOT as pixel-perfect specifications.
Use external links in VISUAL-RESEARCH.md as inspiration and do not copy
third-party branded assets or screenshots into our repo.

FIRST TASK: build only the responsive landing page + dashboard shell
in a vertical slice with working navigation and accessible states.

Rules:
- Next.js App Router, TypeScript, Tailwind, shadcn/ui.
- Motion animations primarily on the public marketing page.
- Honor prefers-reduced-motion, mobile layouts and contrast.
- Do not duplicate Lead Finder, Remotion/Seedance/Veo, PostgreSQL/NocoDB.
- No real API side effects or billable video calls in this task.
- No invented testimonials, statistics, analytics or connected status.
- Authentication must protect private dashboard routes.
- Keep existing backend/domain code untouched if present.
- No new database or worker unless explicitly authorized.

Run npm run typecheck (when configured), and npm run build.
Fix problems, update STATUS.md and STOP.
```

## UI decisions to seek confirmation on

- Brand name display: OutreachOS vs outreachOS.
- Desired public landing copy and product pricing.
- Whether there are verified real videos, logos and customer testimonials.
- Data/API schemas and how organization access is enforced.

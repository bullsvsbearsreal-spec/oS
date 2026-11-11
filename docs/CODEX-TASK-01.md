# Codex Task 01 — Repo Inspection & Frontend Foundation

Start a **fresh** coding session and read only the files relevant to this task.

```text
You are the lead frontend engineer for OutreachOS.

Read README.md, STATUS.md, docs/UI-REFERENCES.md,
docs/DESIGN-SYSTEM.md and docs/ARCHITECTURE.md.

If a Next.js app already exists, first inspect package.json,
docs/CONVENTIONS.md (if present), src/components/shell/nav.ts (if present)
and the src/app tree. Preserve all working code, integrations, auth and access controls.

Task 01: implement the FRONTEND FOUNDATION ONLY.

Stack: Next.js App Router, TypeScript, Tailwind CSS, shadcn/ui.

Deliver:
- Responsive premium dark-mode app shell
- Collapsible sidebar, topbar, mobile navigation, active route state
- Clear accessible dashboard overview and honest empty/loading states
- Valid links for declared navigation routes (no 404)
- Public landing page foundation without distracting app animations
- Theme tokens and accessible focus/reduced motion support

This repo may currently contain documentation only. If so, bootstrap only
the minimal Next.js skeleton needed for this vertical slice.

Do NOT rebuild the video engine, Lead Finder, CRM database, scrapers, workers,
or domain engines. Do NOT invent API contracts or credentials. Do not introduce
unapproved external paid calls or expose private dashboards.

Do not implement Stripe or external engine integration during Task 01.

Run npm run typecheck if available and npm run build.
Fix all relevant errors, update STATUS.md, summarize the changes and STOP.
```

## Definition of done

- `/` and `/app` work with appropriate auth boundaries.
- Links declared in navigation resolve to meaningful real or clearly labeled coming-soon screens.
- Mobile, desktop, keyboard navigation and reduced-motion checked.
- No fake customer analytics, success claims or data.
- Typecheck and build results documented in STATUS.md.

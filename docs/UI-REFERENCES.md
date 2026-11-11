# OutreachOS — UI References (15 selected examples)

Research collection for the public marketing site and the authenticated dashboard. These are **reference URLs**, not downloaded assets, endorsements, or claims of feature equivalence. Recheck demos and licenses during implementation. **Priority:** P0 = initial direction, P1 = optional detail.

## A. Landing page references (5)

| # | Reference | URL | Why / how to use it | Priority |
|---|---|---|---|---|
| 1 | Linear | https://linear.app/ | Premium typography, disciplined spacing, dark surfaces; inspiration for a restrained hero and product narrative | P0 |
| 2 | Raycast | https://www.raycast.com/ | Polished product storytelling and strong visual hierarchy | P1 |
| 3 | Vercel | https://vercel.com/ | Clear calls to action, confident typography and enterprise trust cues | P1 |
| 4 | Framer | https://www.framer.com/ | Interactive marketing presentation and visual motion | P1 |
| 5 | Aceternity UI gallery | https://ui.aceternity.com/components | Marketing hero, Bento Grid and scroll effects | P0 |

### Suggested landing page structure

1. Hero: an outcome-oriented headline, concise value statement and **Book demo** / **Explore capabilities** CTAs.
2. Workflow diagram: discover leads → review → prepare creative → approve → execute.
3. Bento feature cards: Lead Finder, CRM, Video Studio, approvals, billing.
4. Real product previews and video examples only with permission and proper rights.
5. GDPR and human-in-the-loop trust section (do not make unverified blanket compliance guarantees).
6. Verified case studies or product walkthrough instead of fabricated testimonials.

## B. Dashboard references (5)

| # | Reference | URL | Why / how to use it | Priority |
|---|---|---|---|---|
| 6 | Attio | https://attio.com/ | CRM-style lists, filters, saved views and relationships for `/app/leads` | P0 |
| 7 | Linear product UI | https://linear.app/ | Efficient navigation, keyboard shortcuts, clean information hierarchy | P1 |
| 8 | shadcn/ui Dashboard Blocks | https://ui.shadcn.com/blocks/dashboard | App layout patterns and reusable cards for chosen stack | P0 |
| 9 | shadcn/ui Sidebar Blocks | https://ui.shadcn.com/blocks/sidebar | Responsive collapsible navigation | P0 |
| 10 | Runway | https://runwayml.com/ | Project/prompt/preview flows for `/app/studio` (external engine remains authoritative) | P1 |

### Dashboard mapping

- `/app`: actual usage and credit balance, pending approvals and real recent activity.
- `/app/lead-finder` + `/app/leads`: filters, lead score/explanations, provenance and CRM sync state.
- `/app/studio`: script, model choice, cost estimate, review, explicit approval, job status and video link.
- `/app/approvals`: operation details, recipients, costs and audit history.
- `/app/billing`: real billing and auditable credit ledger.

## C. Animated components (5)

| # | Component | Official demo | Proposed use | Constraint |
|---|---|---|---|---|
| 11 | Aceternity Container Scroll | https://ui.aceternity.com/components/container-scroll-animation | Product screenshot reveal | Disable 3D effect for reduced motion; simplify mobile |
| 12 | Aceternity 3D Marquee | https://ui.aceternity.com/components/3d-marquee | Real creative samples and product previews | No fabricated reviews, logos or video output |
| 13 | Magic UI Animated Beam | https://magicui.design/docs/components/animated-beam | Explain Lead Finder → CRM → Video Engine workflow | Outreach still requires explicit user approval |
| 14 | Aceternity Aurora Background | https://ui.aceternity.com/components/aurora-background | Subtle hero background | Keep text readable; avoid heavy dashboard effects |
| 15 | Magic UI Orbiting Circles | https://magicui.design/docs/components/orbiting-circles | Optional integration illustration | Limit loop motion and honor reduced-motion |

## Reference collection protocol

For each example record: source URL, title, one screenshot or authorized sample if licensed, what to adopt, intended app area, and what **not** to copy. Do not commit copyrighted third-party screenshots without redistribution permission.

For motion references, save the original working demo URL and a short description of behavior. Local `research/landing`, `research/dashboard`, and `research/motion` folders can hold your own or licensed assets.

## Recommended combination

- Public `/`: disciplined Linear-style layout, Aceternity scroll reveal, one Animated Beam workflow, Bento feature cards.
- Authenticated `/app/*`: shadcn/ui app shell and straightforward accessible data views. Keep heavy animation on the marketing site.

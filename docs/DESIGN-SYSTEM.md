# OutreachOS — Proposed UI Design System v0.1

**Status:** design proposal, not yet implemented. Test contrast and responsiveness before adopting in production.

## Direction

Premium, reliable, futuristic but restrained, European B2B, transparent and efficient.

- **Public website:** bold typography, purposeful 3D/motion and real product previews.
- **Authenticated dashboard:** quick, clear, compact, accessible and no costly looping animation.

## Initial color tokens

| Token | Hex | Intended purpose |
|---|---|---|
| Background | `#09090F` | Dark page |
| Surface | `#171724` | Cards and sidebar |
| Raised surface | `#222236` | Popovers |
| Primary accent | `#8B5CF6` | Brand interaction |
| Soft accent | `#C084FC` | Decorative highlights |
| Primary text | `#F8FAFC` | Body/headings |
| Muted text | `#A1A1AA` | Secondary labels |
| Border | `#353547` | Subtle outlines |
| Success | `#22C55E` | Success with text/icon |
| Warning | `#F59E0B` | Pending with text/icon |
| Danger | `#EF4444` | Error/rejected with text/icon |

Check WCAG contrast and never convey status by color alone.

## Typography and spacing

- Preferred fonts: Geist or Inter with system fallback.
- Clear hero hierarchy and responsive heading sizes.
- Dashboard body: legible 14–16px; metadata 12–14px only where appropriate.
- 4/8px spacing rhythm; 12–16px card radius, restrained shadows.
- Desktop: collapsible sidebar and clear header.
- Mobile: keyboard/screen-reader-friendly navigation drawer; tables scroll or become structured cards.

## Motion policy

- Motion, Magic UI and Aceternity effects only when they support explanation or conversion.
- Always honor `prefers-reduced-motion`: disable 3D parallax and unnecessary loops.
- Prefer transform/opacity transitions; avoid layout thrashing or delayed important operations.
- Dashboard approvals, payments and CRM actions should be understandable with animations disabled.
- Measure bundle size and Core Web Vitals.

## Reusable components

Page header; responsive app sidebar; loading skeleton; empty, success and error states; filtering and search; data table; selection and bulk actions; confirmation modal; status text and icon; credit balance; audit log; pagination; notification/toast.

All states reflect verified API responses. Never claim a job succeeded or credits were deducted until the server confirms.

## Visual acceptance

- Check at 360px and 1440px.
- Focus visibility and sensible keyboard tab order.
- No page-wide horizontal overflow.
- High contrast and reduced-motion functionality.
- No invented metrics, quotes, client logos or testimonials.

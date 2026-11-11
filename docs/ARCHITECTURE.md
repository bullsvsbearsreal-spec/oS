# OutreachOS — Frontend & API Gateway Boundaries

## External services (already built)

- Video Engine (Remotion, Seedance, Veo 3.1)
- AI Lead Finder and scoring engine
- PostgreSQL / NocoDB CRM
- Additional backend engines (25 reported by project partner)

**Do not rebuild these systems.**

## This repository will own

- Next.js App Router frontend, public landing page, dashboard and accessible component library.
- Authenticated API gateway with adapters under `src/lib/integrations/`.
- Zod validation for all external responses.
- Human-in-the-loop review UX **and server-enforced checks** before external outreach or generation.
- Stripe billing integration and credit usage display.
- Audit logging through an authorized, confirmed backend interface.

Confirm actual API contracts, storage authority, secrets and auth model with backend partner before implementing integration.

## Mandatory rules

1. **Approval:** each externally executed outreach/video operation requires an explicit current `approved` status linked to the exact actor, tenant and payload; enforce on the server, not only client UI.
2. **Credits:** check entitlement/balance, and atomically reserve or debit usage on the trusted server-side credit ledger before billable activity. Stripe handles payments; it is not by itself a reliable usage ledger.
3. **Audit:** record operator, tenant, action, approval, outcome, timestamp and charge through an authorized persistence interface. Avoid storing secrets or unnecessary personal data.
4. **Validation:** validate API request/response with Zod. Treat external content as untrusted.
5. **Tenant isolation:** verify auth and organization permissions for each server request; keep NocoDB credentials and engine API keys server-only.
6. **GDPR:** assess legal basis, privacy notice, purpose limitation, minimization, retention/deletion, processors and international transfer conditions. User approval of an action alone is not GDPR compliance.
7. **Reliability:** verify Stripe webhook signatures, implement idempotency, rate limits, safe retries and error paths.

## Vertical slices roadmap

- **Slice 0:** repository inspection, docs, working app shell + navigation.
- **Slice 1:** one actual Lead Finder read-only view.
- **Slice 2:** authorized NocoDB CRM reads/writes.
- **Slice 3:** approvals + server-side enforcement + audit.
- **Slice 4:** Video Studio: quote → review → approve → submit → status.
- **Slice 5:** Stripe billing and ledger views.
- **Slice 6:** advanced modules and refined marketing presentation.

Do not build all layers horizontally before the first visible screen. Complete each slice with functioning UI, validation and tests.

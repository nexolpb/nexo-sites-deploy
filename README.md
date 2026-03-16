# nexo-sites-deploy

Deployable website artifacts for Nexo.

## Structure

- `apps/sites.nexodigitalops.com/` — Production build output for https://sites.nexodigitalops.com (static)
- `apps/nexodigitalops.com-source/` — Archived standalone HTML source (reference)
- `clients/<slug>/` — Client deliverables (static build output) by slug

## Conventions

- Prefer committing **build output** (static) for simple hosting.
- Keep each client site isolated under `clients/<slug>/`.
- Avoid mixing Emergent export source projects here; those live in `nexolpb/emergent`.

## Deployment

Use your hosting provider (Vercel/Netlify/S3/Cloudflare Pages) pointing at:
- `apps/sites.nexodigitalops.com/` for the Nexo Sites app.
- `clients/<slug>/` for client sites.

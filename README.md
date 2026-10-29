# Denzi — Wellness × Technology × Creativity

A responsive, static portfolio prototype with a premium obsidian/burgundy visual system, liquid-glass navigation, wellness and development divisions, status-labeled project concepts, category filters, and a consent-aware inquiry form.

## Current scope

This project is designed for static hosting such as GitHub Pages. It is **not** a full-stack production CRM and has no database, login, server-side validation, secure admin dashboard, or booking engine. The form prepares an email or WhatsApp message only after a configured contact route is chosen; it does not persist submissions. Do not collect sensitive health data through this static site.

## Run locally

Open `index.html` in a browser, or serve this directory with any static HTTP server. Google Fonts are optional; fallback system fonts are used when offline.

## Deploy with GitHub Pages

1. Push the contents of this directory to the root of a new public repository (for example, `denzi`).
2. In GitHub, open **Settings → Pages**.
3. Choose **Deploy from a branch**, select `main` and `/ (root)`, and save.
4. Wait for the Pages deployment workflow, then verify the URL shown in Settings → Pages.

## Configure contact and links

Edit `js/config.js`:

- `whatsappNumber`: international-format number using digits only (e.g. `919876543210`).
- `email`: a public reply-to/contact address you control.
- `social.instagram`, `social.linkedin`, `social.youtube`: full HTTPS profile URLs you own.

Blank values are intentionally disabled. GitHub is currently linked to the account `anmoloraon200-create`; its existing `mission-fit-india` repository is a separate business website and should not be overwritten by this brand.

## Moving to a real backend

For the requested secure operations, use a server-capable host (e.g. Next.js on a platform that supports server routes) plus Supabase/PostgreSQL, managed authentication, Storage, strict Row Level Security, server-side Zod validation, rate limiting, and audit logging. Implement database migrations for profiles, services, leads, lead_activities, projects, posts, appointments, availability_slots, testimonials, media_assets, site_settings, and audit_logs. Use a verified email/WhatsApp provider for notices. Never expose service-role credentials in browser code.

## Privacy and content integrity

- The form requests consent before preparing a contact message.
- The form explicitly asks visitors not to share sensitive health information.
- Wellness content is general education, not medical diagnosis or treatment.
- Portfolio entries are labeled Concept or In Progress and do not claim unverified clients, outcomes, or deployments.
- The abstract D artwork is a replaceable placeholder, not a personal photograph.

## Test checklist

Manual checks recommended before publishing:
- Narrow mobile viewport around 360px, tablet, desktop, and wide desktop.
- Keyboard-only navigation, focus indicators, Escape to close mobile nav, reduced-motion setting.
- Project filter buttons and active states.
- Form required fields, email/WhatsApp validation, consent check, and unconfigured contact route messages.
- Confirm there are no secrets or real client records in the repository.

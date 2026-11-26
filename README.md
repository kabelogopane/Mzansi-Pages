# Mzansi-Pages

**Your People. Your World. Your Pages.**

Mzansi-Pages is a responsive, installable social-networking **preview app** with a modern African technology identity.

## Preview features

- Responsive desktop and mobile interface
- Installable Progressive Web App (PWA) manifest and app icon
- Offline app-shell caching after the first successful visit
- Home feed with sample content
- Create demo text posts and save them in this browser
- Demo likes and navigation across product areas
- Discovery, communities, connections, messages, opportunities and profile screens
- Separate 18+ dating information screen; no dating, matching or dating messages
- Privacy notice and draft community guidelines

## Important: what this release is (and is not)

This repository is ready to publish as a **public preview**. It is not yet a production multi-user social network.

- Demo posts are saved in the current browser's local storage. They are not visible to other users and do not sync across devices.
- There is no real account registration, login, database, photo upload, private messaging, live notification, or server-side search.
- Like and connection actions are demonstrations.
- Do not collect real personal, contact, identity or sensitive information through this preview.
- The date-of-birth screen is only a prototype eligibility check, not proof of age.

The planned first release is adults-only. Production must implement reliable age assurance and server-side enforcement before account creation or access. Any future dating area must be separately gated to verified adults and must include appropriate consent, privacy, reporting, blocking and moderation safeguards.

## Publish with GitHub Pages

A GitHub Actions workflow has been added at `.github/workflows/pages.yml`.

1. Open this repository on GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **GitHub Actions** as the source.
4. Open the **Actions** tab and check the deployment workflow.
5. When the workflow completes successfully, open:

   https://kabelogopane.github.io/Mzansi-Pages/

The first deployment may take a few minutes. The site is not considered live until the Pages deployment reports success.

## Install the preview

Open the published site in a supported browser. Use the browser's **Install app** or **Add to Home Screen** option if available. Offline caching is activated after the first successful visit.

## Repository structure

- `index.html` — responsive app interface and preview interactions
- `manifest.webmanifest` — installable app metadata
- `service-worker.js` — offline app-shell caching
- `assets/mzansi-icon.svg` — app icon
- `privacy.html` — preview privacy notice
- `community-guidelines.html` — draft community rules
- `docs/PRODUCT-BLUEPRINT.md` — product requirements and direction
- `.github/workflows/pages.yml` — automatic GitHub Pages deployment

## Production build still required

GitHub Pages hosts static files. It does not provide secure accounts, a database or private messaging. Before launching as a real social platform, connect a secure backend (for example Supabase), implement server-side authorization and database Row Level Security, and complete privacy, age-assurance, moderation and security reviews. Replace the preview privacy notice with a legally reviewed production notice.

Recommended production sequence:

1. Authentication and adult age-assurance integration.
2. Profiles and privacy settings.
3. Posts, comments and reactions stored in a database.
4. Connections and community membership.
5. Reporting, blocking, moderation and admin tools.
6. Messaging and notifications.
7. Security testing, POPIA review and launch readiness checks.
8. Android app build after the web MVP is stable.

## Brand

- Name: Mzansi-Pages
- Tagline: Your People. Your World. Your Pages.
- Direction: Modern African technology
- Palette: Midnight Navy `#101D38`, Electric Blue `#3286E8`, African Gold `#E7B84B`, Cloud White `#F5F7FB`, Violet `#805AD5`

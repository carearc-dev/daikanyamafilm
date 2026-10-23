# DAIKANYAMA FILM website

Vite + React implementation of the DAIKANYAMA FILM website.

## Requirements

- Node.js 18 or newer
- npm 9 or newer (or pnpm)

## Run locally

```sh
npm install
npm run dev
```

## Build and deploy

```sh
npm install
npm run build
```

Upload the contents of `dist/` to a static web host. Configure a fallback/rewrite to `index.html` for `/works`, `/cast`, `/news`, and `/lp` so direct visits and refreshes on those routes work.

## Before production

- The contact form is a front-end placeholder. It validates fields but does not send or store submissions. Connect a trusted HTTPS endpoint and configure server-side validation, spam protection, and a privacy notice before accepting inquiries.
- Application-form links, social profiles, YouTube videos, and the Timerex booking link go to third-party services. Their availability is controlled by those services and could not be verified from this network-restricted environment.
- Google Fonts are loaded from Google Fonts. A network connection is needed for those web fonts; the site uses local/system fallbacks.
- Use HTTPS in production. Keep server/deployment credentials outside this source package and keep dependencies updated.

## Included files

- `src/` — React page and styles
- `public/images/` — local image assets used by the site
- `dist/` — ready-to-host production build
- `package.json` and `pnpm-lock.yaml` — dependencies and lockfile

This is a hand-built site source package. It does not contain the original STUDIO project, CMS data, or credentials.

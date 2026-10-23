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

- Contact submissions use Formspree, which works with static GitHub Pages hosting. Create a Formspree form and configure its form ID as `VITE_FORMSPREE_ID` before building. For local development, copy `.env.example` to `.env.local` and set the ID there. For GitHub Actions, add a repository Actions variable named `VITE_FORMSPREE_ID` and expose it to the Vite build step. The form ID is public by design; never put a private API key in browser code. Configure the recipient and spam protections in Formspree, and update the privacy notice to disclose the service before accepting inquiries. Without the form ID the site clearly reports that submissions are not configured.
- Application-form links, social profiles, YouTube videos, and the Timerex booking link go to third-party services. Their availability is controlled by those services and could not be verified from this network-restricted environment.
- Google Fonts are loaded from Google Fonts. A network connection is needed for those web fonts; the site uses local/system fallbacks.
- Use HTTPS in production. Keep server/deployment credentials outside this source package and keep dependencies updated.

## Included files

- `src/` — React page and styles
- `public/images/` — local image assets used by the site
- `dist/` — ready-to-host production build
- `package.json` and `pnpm-lock.yaml` — dependencies and lockfile
- `.env.example` — required form configuration name

This is a hand-built site source package. It does not contain the original STUDIO project, CMS data, or credentials.

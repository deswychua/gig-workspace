# KrewMY — Event Workforce Operating System (Malaysia)

Interactive multi-role prototypes for **KrewMY**, a specialized event gig workforce platform designed for the Malaysian live events ecosystem (concerts, festivals, sports, conventions).

## Live Personas & Prototypes

The platform features four synchronized roles:

| # | Role | Platform / Form Factor | File | Key Capabilities |
|---|---|---|---|---|
| **01** | **Admin** | Desktop Web Console (1280px+) | [`krewmy-admin-web.html`](krewmy-admin-web.html) | Identity eKYC & IC verification, dispute queue, automated DuitNow settlement batches, platform telemetry. |
| **02** | **Organiser** | Desktop Web Platform (1440px+) | [`krewmy-organiser-web.html`](krewmy-organiser-web.html) | Multi-tier shift roster builder, real-time venue gate allocation, live digital attendance sign-off, payroll release. |
| **03** | **Ops** | Mobile Companion (8 Screens, 390×844) | [`krewmy-ops-mobile.html`](krewmy-ops-mobile.html) | Zone & gate binding, offline cryptographic QR check-in scanner, live headcounts, instant SOS standby replacement dispatch. |
| **04** | **Gig Worker** | Mobile App (7 Screens, 393px) | [`krewmy-gigworker-mobile.html`](krewmy-gigworker-mobile.html) | Transit-aligned gig discovery (LRT/MRT corridors), shift briefings, geofenced clock-in, instant DuitNow wallet cashout. |

---

## Selection Page (Entry Point)

- **Entry Point**: [`index.html`](index.html)
- A role selection hub allowing instant launching into any of the 4 experiences.
- Includes keyboard shortcuts (<kbd>1</kbd>, <kbd>2</kbd>, <kbd>3</kbd>, <kbd>4</kbd>) and an interactive event lifecycle map.
- A floating role switcher is embedded across all prototype pages for seamless switching between roles.

---

## Local Development & Testing

You can preview the site locally using any static web server:

```bash
# Python 3
python3 -m http.server 8080

# Or Node.js
npx serve .
```

Then open `http://localhost:8080` in your browser.

---

## GitHub Pages Deployment

This repository is pre-configured with:
1. `.github/workflows/pages.yml` for automated GitHub Actions deployment.
2. `.nojekyll` to bypass Jekyll static generation.

### Enabling GitHub Pages on GitHub:
1. Go to repository **Settings** > **Pages**.
2. Under **Build and deployment** > **Source**, choose either:
   - **GitHub Actions** (recommended — uses `.github/workflows/pages.yml`), or
   - **Deploy from a branch** > branch `main` > folder `/ (root)`.
3. Your site will be live at `https://<username>.github.io/<repo>/`!

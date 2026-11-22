# Harmony Calipers Documentation

Public help and support website for **Harmony Calipers**, the visual songwriting companion for iPhone and iPad.

**Planned public site:** <https://94972cptbv-tech.github.io/HarmonyCalipers-Documentation/>

The app's source remains in a separate **private repository**. This repository contains only public-facing documentation.

## Local development

Requires Python 3.10 or newer.

```bash
python3 -m venv .venv
source .venv/bin/activate
python3 -m pip install -r requirements.txt
mkdocs serve
```

Then open <http://127.0.0.1:8000/>.

## Validate before publishing

```bash
mkdocs build --strict
```

Review all entries marked **PUBLISHING CHECK** in `docs/support.md`, `docs/privacy.md`, and `docs/release-notes.md` before making the site public.

## Deployment

The workflow `.github/workflows/deploy.yml` builds the site and deploys it to GitHub Pages on pushes to `main` or on manual invocation.

In GitHub go to **Settings → Pages → Build and deployment → Source: GitHub Actions**. The first successful deployment publishes the project site at the URL above. Check **Actions** for the deployment result.

## Screenshots

Use **actual app captures only**, with permission to publish. Add files to `docs/assets/screenshots/` and link from guides after verifying musical notation and chord labels. Do not publish fabricated app UI.

## Tracking

Implementation tracked in the private application repository: [Harmony Calipers Issue #1](https://github.com/94972cptbv-tech/HarmonyCalipers/issues/1). This link may require repository access.

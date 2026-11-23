# Portfolio-DEV

A temporary DEV copy of Phill's portfolio, used to build the shared Paño (see [PANO-PLAN.md in the Pano repo](https://github.com/marquisphill/Pano/blob/main/PANO-PLAN.md)). It will be deleted in phase 6 of that plan.

- **DEV site:** https://marquisphill.github.io/Portfolio-DEV/
- **Copied from:** `Professional-Portfolio2-STAGING` at commit `a8fd203` on 2026-11-23, without its `.claude` folder.

## How it differs from staging

| Change | Why |
|---|---|
| Saved settings use their own names: `dev-pf-wall`, `dev-pf-cb`, `dev-labs-view` | Every site under `marquisphill.github.io` shares one browser storage. This keeps DEV from reading or changing the real sites' saved choices. |
| `index.html` and `hackathon.html` ask search engines not to list them | So a duplicate of the portfolio never shows up in search results. |
| Paño is no longer inside `index.html`. The page loads him from the Pano repo: `/Pano/latest/pano.css` and `/Pano/latest/pano.js` (phase 1, 2026-11-23) | This is the build itself. His words and tours load from his brain there, and his abilities from `/Pano/latest/skills/`. What stays in the page is a short adapter near the end of the script that tells him what the page has; each skill has one line there, and taking a line out turns that skill off. He should look and behave exactly as on staging. |

Because of that, open the page through a server that also serves the Pano repo at `/Pano/`. GitHub Pages does. On a computer, use `tests/serve.py` from the Pano repo.

Everything else is identical. Do not make changes here that are meant for the real site; those go to staging.

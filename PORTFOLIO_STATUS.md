# Royalpuskar Portfolio Status

_Last updated: 12 November 2026. This document records source-control and CI evidence available at review time; external deployments may change._

## Inventory and engineering milestone

- 17 repositories were visible to the connected account: one profile/roadmap repository and 16 software project repositories.
- All 16 software repositories have a committed verification workflow with a **successful workflow run** observed for the current wave of changes.
- Passing these checks proves only the checks ran successfully; it does **not** establish universal website functionality, security certification, Android build readiness, performance, or production-grade payments.

### Standalone security and research workbenches

The following nine repositories have distinct engines, browser examples, reproducible sample contracts and successful JS/Python verification workflows:

1. [SENTINEL-X](https://github.com/Royalpuskar/SENTINEL-X)
2. [COGNISHIELD](https://github.com/Royalpuskar/COGNISHIELD)
3. [GHOSTKEY](https://github.com/Royalpuskar/GHOSTKEY)
4. [NEUROGRID](https://github.com/Royalpuskar/NEUROGRID)
5. [TRACEZERO](https://github.com/Royalpuskar/TRACEZERO)
6. [PhishScope](https://github.com/Royalpuskar/PhishScope)
7. [PrivacyLens](https://github.com/Royalpuskar/PrivacyLens)
8. [OpenResearch-Nepal](https://github.com/Royalpuskar/OpenResearch-Nepal)
9. [agent-permission-gate](https://github.com/Royalpuskar/agent-permission-gate)

### Application updates

| Repository | Updated functionality | Validation status |
| --- | --- | --- |
| [PUSKAR-AI](https://github.com/Royalpuskar/PUSKAR-AI) | Fixed markup/scripts, removed browser-exposed credential from current code, built Node API proxy | Integration CI passed. Real AI requires private backend deployment |
| [ai-student-assistant](https://github.com/Royalpuskar/ai-student-assistant) | StudyNest static planner, notes extraction, basic study helper, dependency-free API | Browser asset and Node tests passed |
| [GANDOPS-WEB](https://github.com/Royalpuskar/GANDOPS-WEB) | Fully implemented interactive reliability simulation website | Engine tests passed; GitHub Pages deployment workflow succeeded |
| [Social-Mind-AI](https://github.com/Royalpuskar/Social-Mind-AI) | Removed public API-key prompt, added browser heuristic scanner, removed unverifiable usage claims | Python + browser syntax checks passed; GitHub Pages workflow succeeded |
| [SUMITRA-SHOES-CENTRE-](https://github.com/Royalpuskar/SUMITRA-SHOES-CENTRE-) | Responsive PHP storefront, unpaid-demo checkout safeguards, static lookbook, docs Pages source | PHP/static checks passed; Pages publishing needed follow-up |
| [POKYON](https://github.com/Royalpuskar/POKYON) | Playable Orbit Rush Canvas prototype with tested simulation | Node CI passed; public Pages URL not independently verified |
| [POKYON-](https://github.com/Royalpuskar/POKYON-) | Removed shared debug signing file and old debug APK from current branch, switched signing and added safety guidance | Repository hygiene CI passed; Android binary build not verified |

## Critical security follow-up

**P0 — Rotate previously exposed API credential:** PUSKAR-AI previously committed an API credential inside browser JavaScript. The current branch removes it, but commit history may still expose it. The owner must revoke the old credential in the provider dashboard, review recent usage/billing, and use a new server-side key only. No source-control edit can revoke the old credential.

**P0 — Android signing history:** POKYON- previously committed a Base64-encoded debug keystore and associated APK. Both were removed from the current branch but remain historically recoverable until a careful, coordinated history rewrite. The old debug signature must not be trusted for distribution; generate independent signing credentials for new builds and consider the update/uninstall implications.

## Remaining gaps / decision checklist

- [ ] Configure or confirm live GitHub Pages deployment for projects without a fresh successful build. Do not treat existing source files as proof of a functioning public site.
- [ ] Deploy PUSKAR-AI on a secure Node-capable host with authenticated API access, shared rate limiting, managed spending limits, and a **new** credential.
- [ ] Add headless browser smoke tests, keyboard accessibility checks, and responsive visual regression checks to all public-facing static sites.
- [ ] Add reproducible Android Gradle wrapper/build/test pipelines for POKYON- and run instrumented tests before release.
- [ ] Convert the shoe-store prototype to proper server-side payment verification, order statuses, inventory updates, CSRF on all mutations, stronger authentication and secure session controls **before** accepting real payments.
- [ ] Publish documented threat models, evaluation datasets, measured outcomes, limitations and comparison baselines for research workbenches.
- [ ] Replace placeholder/sample dashboard metrics with real, consented, documented data only if real integrations are added.

## Evidence standard

Projects should be represented as **working research prototypes** until their behavior, deployed endpoints, security assumptions, and independent tests support stronger claims. Avoid claims of user adoption, detection accuracy, revenue, awards, uptime SLAs, or production reliability without documented evidence.

For prioritization, see [Project Roadmap](./PROJECT_ROADMAP.md). For code and test details, follow each repository's README and Actions page.

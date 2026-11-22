# Royalpuskar — project catalogue

[Return to profile](https://github.com/Royalpuskar)

## Project catalogue


## Security research

| Repository | Focus | Evidence |
| --- | --- | --- |
| [SENTINEL-X](https://github.com/Royalpuskar/SENTINEL-X) · SentinelMesh | Defensive event correlation and explainable alerts | Browser workbench, JS/Python engines, contract tests |
| [COGNISHIELD](https://github.com/Royalpuskar/COGNISHIELD) · TrustLayer AI | Prompt-injection signals and agent action policies | Local policy scenarios and tests |
| [GHOSTKEY](https://github.com/Royalpuskar/GHOSTKEY) | Credential lifecycle simulation and scope checks | Issuance/revocation simulation and tests |
| [TRACEZERO](https://github.com/Royalpuskar/TRACEZERO) | Evidence hashing and tamper-evident custody chains | Reproducible validation fixtures |
| [PhishScope](https://github.com/Royalpuskar/PhishScope) | URL structure warning indicators | Browser URL triage and Python reference |
| [PrivacyLens](https://github.com/Royalpuskar/PrivacyLens) | Personal-data exposure prioritization | Local illustrative risk model |
| [NEUROGRID](https://github.com/Royalpuskar/NEUROGRID) | Capability-aware dependent-task scheduling | Deterministic planning engine |
| [agent-permission-gate](https://github.com/Royalpuskar/agent-permission-gate) | Default-deny access decisions for agents | Policy engine and test cases |
| [token-lifecycle-lab](https://github.com/Royalpuskar/token-lifecycle-lab) | Refresh rotation, expiry, and family reuse revocation | Interactive simulator and six behavior tests |
| [workflow-counterexample](https://github.com/Royalpuskar/workflow-counterexample) | Finite-state safety checks and shortest failure traces | BFS checker, minimum repair planner, 19 local behavior tests |
| [OpenResearch-Nepal](https://github.com/Royalpuskar/OpenResearch-Nepal) | Reproducibility metadata and basic experiment summaries | Inspectable datasets and checks |

Each project is an **independent research prototype**, not a professionally certified security product. The research repositories contain runnable browser examples and automated JavaScript tests; the original nine also include Python reference engines.

## Live research demos

These browser applications have been deployed on GitHub Pages and exercised with scoped smoke checks. Per-project documentation describes behavior and verification limits.

- [SENTINEL-X — open web demo](https://royalpuskar.github.io/SENTINEL-X/)
- [COGNISHIELD — open web demo](https://royalpuskar.github.io/COGNISHIELD/)
- [GHOSTKEY — open web demo](https://royalpuskar.github.io/GHOSTKEY/)
- [NEUROGRID — open web demo](https://royalpuskar.github.io/NEUROGRID/)
- [TRACEZERO — open web demo](https://royalpuskar.github.io/TRACEZERO/)
- [PhishScope — open web demo](https://royalpuskar.github.io/PhishScope/)
- [PrivacyLens — open web demo](https://royalpuskar.github.io/PrivacyLens/)
- [OpenResearch-Nepal — open web demo](https://royalpuskar.github.io/OpenResearch-Nepal/)
- [agent-permission-gate — open web demo](https://royalpuskar.github.io/agent-permission-gate/)

- [Token Lifecycle Lab — open web demo](https://royalpuskar.github.io/token-lifecycle-lab/)
- [Workflow Counterexample — open web demo](https://royalpuskar.github.io/workflow-counterexample/)

## Resilient systems

| Repository | Implemented behavior | Validation |
| --- | --- | --- |
| [Offline Relay](https://github.com/Royalpuskar/offline-relay) | Two-client delivery simulator, version checks, duplicate suppression, and reviewed conflicts | Eight protocol tests passed locally; live-browser interaction check pending |

[Open Offline Relay](https://royalpuskar.github.io/offline-relay/). GitHub Pages deployment was confirmed. This is an in-memory simulation, not a deployed synchronization API.

## Data and reproducibility

| Repository | Implemented behavior | Validation |
| --- | --- | --- |
| [Dataset Lineage Map](https://github.com/Royalpuskar/dataset-lineage-map) | SHA-256 fingerprints, dependency validation, baseline comparison, downstream review order, and evidence export | Ten automated tests passed; live comparison, invalid-input handling, and export checked |

[Open Dataset Lineage Map](https://royalpuskar.github.io/dataset-lineage-map/). Text stays in the browser. This workbench flags changes in declared dependencies; it does not execute transformations or certify research accuracy.

## Privacy and reliability tools

These browser-local prototypes explore focused privacy and reliability problems. Each has its own domain engine, synthetic fixture, README, MIT license, and three automated test cases. They share a portfolio UI system. Live smoke checks covered sample results, invalid input, stale-export prevention, and reset; Cache Truth also had filtering and download checks.

| Project | Implemented purpose | Demo |
| --- | --- | --- |
| [Consent Ledger](https://github.com/Royalpuskar/consent-ledger) | Evaluate time-limited sharing grants against an auditable event history. | [Website](https://royalpuskar.github.io/consent-ledger/) |
| [Session Observatory](https://github.com/Royalpuskar/session-observatory) | Explain sign-in risk signals from synthetic session observations. | [Website](https://royalpuskar.github.io/session-observatory/) |
| [Secret Boundary](https://github.com/Royalpuskar/secret-boundary) | Inspect JSON fields, redact by field name or exact path, and export a value-free audit. | [Website](https://royalpuskar.github.io/secret-boundary/) |
| [Permission Diff](https://github.com/Royalpuskar/permission-diff) | Compare permission manifests and surface added or removed privileges. | [Website](https://royalpuskar.github.io/permission-diff/) |
| [Tenant Isolation Checker](https://github.com/Royalpuskar/tenant-isolation-checker) | Audit supplied authorization decisions for cross-tenant access failures. | [Website](https://royalpuskar.github.io/tenant-isolation-checker/) |
| [Privacy Budget Board](https://github.com/Royalpuskar/privacy-budget-board) | Track sequential epsilon spending and reject queries exceeding a declared budget. | [Website](https://royalpuskar.github.io/privacy-budget-board/) |
| [Conflict Atlas](https://github.com/Royalpuskar/conflict-atlas) | Perform a three-way merge of flat records while preserving conflicting edits. | [Website](https://royalpuskar.github.io/conflict-atlas/) |
| [Outage Rehearsal](https://github.com/Royalpuskar/outage-rehearsal) | Replay synthetic successes and failures through a circuit-breaker state machine. | [Website](https://royalpuskar.github.io/outage-rehearsal/) |
| [Queue Compass](https://github.com/Royalpuskar/queue-compass) | Compare first-come-first-served and shortest-available-job queue scheduling. | [Website](https://royalpuskar.github.io/queue-compass/) |
| [Cache Truth](https://github.com/Royalpuskar/cache-truth) | Replay reads and source writes to expose TTL cache staleness. | [Website](https://royalpuskar.github.io/cache-truth/) |

## Developer tools

These scoped prototypes are deployed on GitHub Pages. Local validation covered 31 automated test cases across these ten projects (four for Edge Budget, three for each other project). Browser smoke checks covered sample results, invalid input, stale-export prevention, and reset. Release Evidence also passed filtering and download checks. These are scoped tools with documented limitations and a shared UI system.

| Project | Implemented purpose | Demo |
| --- | --- | --- |
| [Edge Budget](https://github.com/Royalpuskar/edge-budget) | Find the highest-value subset of tasks fitting a memory budget. | [Website](https://royalpuskar.github.io/edge-budget/) |
| [Replay Harbor](https://github.com/Royalpuskar/replay-harbor) | Replay inventory events and expose the exact event that violates stock invariants. | [Website](https://royalpuskar.github.io/replay-harbor/) |
| [Architecture Drift](https://github.com/Royalpuskar/architecture-drift) | Audit a declared module dependency graph against allowed layer boundaries. | [Website](https://royalpuskar.github.io/architecture-drift/) |
| [API Contract Garden](https://github.com/Royalpuskar/api-contract-garden) | Compare simplified endpoint contracts for removals, type changes, and new required fields. | [Website](https://royalpuskar.github.io/api-contract-garden/) |
| [Test Gap Map](https://github.com/Royalpuskar/test-gap-map) | Intersect changed executable line numbers with supplied coverage to find untested changes. | [Website](https://royalpuskar.github.io/test-gap-map/) |
| [Dependency Weather](https://github.com/Royalpuskar/dependency-weather) | Surface missing dependency evidence alongside explicit maintenance signals. | [Website](https://royalpuskar.github.io/dependency-weather/) |
| [Build Budget](https://github.com/Royalpuskar/build-budget) | Compare asset sizes and enforce total and per-asset byte budgets. | [Website](https://royalpuskar.github.io/build-budget/) |
| [Docs Execution Kit](https://github.com/Royalpuskar/docs-execution-kit) | Validate JSON code examples extracted from Markdown fences. | [Website](https://royalpuskar.github.io/docs-execution-kit/) |
| [Config Provenance](https://github.com/Royalpuskar/config-provenance) | Merge flat configuration layers and explain each effective value without showing marked secrets. | [Website](https://royalpuskar.github.io/config-provenance/) |
| [Release Evidence](https://github.com/Royalpuskar/release-evidence) | Audit a release manifest for failed checks, duplicate artifacts, and mismatched SHA-256 digests. | [Website](https://royalpuskar.github.io/release-evidence/) |

## Working applications

| Project | What it does | Current scope |
| --- | --- | --- |
| [GANDOPS-WEB](https://github.com/Royalpuskar/GANDOPS-WEB) | Interactive service reliability risk dashboard | Fully local static simulation; no production telemetry connection |
| [StudyNest](https://github.com/Royalpuskar/ai-student-assistant) | Study planner, notes extractor, study helper | Working offline browser tools + optional local Node API |
| [SocialMind AI](https://github.com/Royalpuskar/Social-Mind-AI) | Scam-message indicators and URL research | Explainable local triage and separate Python tests; no claimed accuracy benchmark |
| [PUSKAR-AI](https://github.com/Royalpuskar/PUSKAR-AI) | Draft email, reply, and chat interface | Frontend and Node backend; live AI needs a privately configured server key |
| [POKYON Orbit Rush](https://github.com/Royalpuskar/POKYON) | Playable browser arcade game | Canvas controls, scoring, collisions, automated tests |
| [POKYON Android Lab](https://github.com/Royalpuskar/POKYON-) | Experimental Android game screens and embedded web scenes | Android prototype; release builds and payments not verified |
| [Sumitra Shoes Centre](https://github.com/Royalpuskar/SUMITRA-SHOES-CENTRE-) | Interactive static footwear lookbook + PHP/MySQL store demo | Static catalogue and unpaid local demo orders; **no real payment processing** |



## Reproducible checks

[![SentinelMesh checks](https://github.com/Royalpuskar/SENTINEL-X/actions/workflows/verify.yml/badge.svg)](https://github.com/Royalpuskar/SENTINEL-X/actions/workflows/verify.yml)
[![GANDOPS checks](https://github.com/Royalpuskar/GANDOPS-WEB/actions/workflows/verify.yml/badge.svg)](https://github.com/Royalpuskar/GANDOPS-WEB/actions/workflows/verify.yml)
[![StudyNest checks](https://github.com/Royalpuskar/ai-student-assistant/actions/workflows/verify.yml/badge.svg)](https://github.com/Royalpuskar/ai-student-assistant/actions/workflows/verify.yml)
[![SocialMind checks](https://github.com/Royalpuskar/Social-Mind-AI/actions/workflows/verify.yml/badge.svg)](https://github.com/Royalpuskar/Social-Mind-AI/actions/workflows/verify.yml)
[![POKYON checks](https://github.com/Royalpuskar/POKYON/actions/workflows/verify.yml/badge.svg)](https://github.com/Royalpuskar/POKYON/actions/workflows/verify.yml)

A passing check demonstrates that the **specified tests passed for that revision**, not that a project is secure or production ready.

### Secret Boundary verification

[Redaction Studio source](https://github.com/Royalpuskar/secret-boundary) includes separate policy controls, a field inspector, reviewed output, and audit exports. Ten engine tests passed locally, along with JavaScript syntax and static selector checks. The redesigned interface still needs live-browser, mobile, and 4K verification; its latest deployment is not yet confirmed.


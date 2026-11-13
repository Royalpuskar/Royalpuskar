# Independent Project Roadmap

64 original standalone project proposals for Royalpuskar. **Current status: three roadmap projects (`agent-permission-gate`, `token-lifecycle-lab`, and `workflow-counterexample`) have implemented research prototypes; the remaining roadmap proposals are not claimed complete.** Names are suggestions, subject to availability. These are engineering directions, not claims of unprecedented invention or production readiness.

## Six priority projects

1. [`agent-permission-gate`](https://github.com/Royalpuskar/agent-permission-gate) — implemented research prototype with tests
2. `offline-relay`
3. [`token-lifecycle-lab`](https://github.com/Royalpuskar/token-lifecycle-lab) — implemented interactive prototype with six tests
4. `architecture-drift`
5. `dataset-lineage-map`
6. [`workflow-counterexample`](https://github.com/Royalpuskar/workflow-counterexample) — implemented interactive prototype with nine tests

These remain roadmap priorities, not automatic GitHub pins. Three implemented prototypes are linked above; the other three remain future directions.

## Delivery standard

Each project should have its own runnable implementation, setup instructions, architecture notes, meaningful tests, sample data, limitations, and documented security assumptions. Keep credentials out of source control. Use synthetic fixtures by default. Do not add decorative AI branding or watermarks; preserve required third-party license notices. Only claim results measured by the implemented project.

## Security and identity

### 1. consent-ledger

- Purpose: Time-limited data-sharing permissions with an auditable revocation history.
- First working version: Build a policy API, expiry checks, and append-only consent receipts.
- Acceptance check: Expired or revoked grants always deny access.
- Status: proposed; not implemented.

### 2. session-observatory

- Purpose: Explainable session-risk monitoring that shows the signals behind each decision.
- First working version: Replay synthetic sign-in events and produce inspectable risk reports.
- Acceptance check: Replay yields deterministic scores without collecting real credentials.
- Status: proposed; not implemented.

### 3. secret-boundary

- Purpose: Detect secrets crossing application logging boundaries.
- First working version: Add a log filter, synthetic secret fixtures, and redaction reports.
- Acceptance check: Seeded secrets never reach the output logs.
- Status: proposed; not implemented.

### 4. passkey-recovery-lab

- Purpose: Explore account recovery tradeoffs without storing passwords.
- First working version: Build a WebAuthn sandbox and recovery threat model.
- Acceptance check: Recovery cannot bypass the configured verification steps.
- Status: proposed; not implemented.

### 5. permission-diff

- Purpose: Show how dependency or configuration changes expand application privileges.
- First working version: Compare two permission manifests and generate a review report.
- Acceptance check: Every added permission is identified with its source.
- Status: proposed; not implemented.

### 6. token-lifecycle-lab

- Purpose: Visualize token issuance, rotation, expiry, and reuse rejection.
- First working version: Implement a local session simulator with a token-family store.
- Acceptance check: Reusing a rotated refresh token revokes its family.
- Status: **research prototype implemented** with a live browser demo and automated tests; not a production service.

### 7. tenant-isolation-checker

- Purpose: Test whether tenants can access each other's resources.
- First working version: Generate paired tenant fixtures and run authorization probes.
- Acceptance check: All cross-tenant fixture requests are denied.
- Status: proposed; not implemented.

### 8. privacy-budget-board

- Purpose: Track aggregate query privacy budgets for a synthetic dataset.
- First working version: Implement a query ledger and basic differential privacy demonstrations.
- Acceptance check: Queries exceeding the configured budget are rejected.
- Status: proposed; not implemented.

## Resilient systems

### 9. offline-relay

- Purpose: Synchronize essential forms across intermittent connections.
- First working version: Build a local outbox, idempotent API, and conflict inspector.
- Acceptance check: Duplicate delivery never creates duplicate records.
- Status: proposed; not implemented.

### 10. conflict-atlas

- Purpose: Explain concurrent edits and compare conflict-resolution strategies.
- First working version: Implement a two-client document simulator with reproducible histories.
- Acceptance check: Both clients converge after all messages arrive.
- Status: proposed; not implemented.

### 11. outage-rehearsal

- Purpose: Run controlled service-failure exercises in a local sandbox.
- First working version: Inject latency, timeouts, and dependency failures into demo services.
- Acceptance check: Reports link each failure to observed recovery behavior.
- Status: proposed; not implemented.

### 12. queue-compass

- Purpose: Forecast queue congestion and show scheduling tradeoffs.
- First working version: Build a discrete-event simulator with multiple scheduling policies.
- Acceptance check: Known fixture workloads produce expected wait times.
- Status: proposed; not implemented.

### 13. migration-sentinel

- Purpose: Rehearse database migrations against generated workloads.
- First working version: Apply reversible schema changes to a disposable database.
- Acceptance check: Rollback restores fixture data and schema.
- Status: proposed; not implemented.

### 14. cache-truth

- Purpose: Expose stale-cache behavior through controlled experiments.
- First working version: Compare TTL, invalidation, and stale-while-revalidate strategies.
- Acceptance check: Each response identifies data version and freshness.
- Status: proposed; not implemented.

### 15. edge-budget

- Purpose: Allocate limited compute among competing offline tasks.
- First working version: Build a scheduler constrained by memory and energy estimates.
- Acceptance check: No scheduled batch exceeds configured resource limits.
- Status: proposed; not implemented.

### 16. replay-harbor

- Purpose: Reproduce service behavior from sanitized event traces.
- First working version: Build a deterministic event runner with snapshot comparisons.
- Acceptance check: Repeated runs produce the same state hashes.
- Status: proposed; not implemented.

## Developer tools

### 17. architecture-drift

- Purpose: Track differences between declared architecture and actual imports.
- First working version: Parse a supported language and compare dependency rules.
- Acceptance check: Forbidden fixture imports are reported with file locations.
- Status: proposed; not implemented.

### 18. api-contract-garden

- Purpose: Detect breaking API changes with executable examples.
- First working version: Compare OpenAPI revisions and run saved consumer cases.
- Acceptance check: Breaking changes in fixtures are correctly classified.
- Status: proposed; not implemented.

### 19. test-gap-map

- Purpose: Find changed behaviors that existing tests do not exercise.
- First working version: Combine coverage data with a patch and report uncovered lines.
- Acceptance check: A fixture patch produces the expected uncovered regions.
- Status: proposed; not implemented.

### 20. dependency-weather

- Purpose: Inspect dependency health using explicit, inspectable signals.
- First working version: Import lockfiles and show version, license, and maintenance signals.
- Acceptance check: Unavailable signals are labeled unknown rather than inferred.
- Status: proposed; not implemented.

### 21. build-budget

- Purpose: Explain build-size changes by module and asset.
- First working version: Compare build manifests and enforce size thresholds.
- Acceptance check: An oversized fixture fails with an actionable breakdown.
- Status: proposed; not implemented.

### 22. docs-execution-kit

- Purpose: Keep documentation examples runnable and checked.
- First working version: Extract fenced examples for one language and execute in isolation.
- Acceptance check: A broken example fails the documentation check.
- Status: proposed; not implemented.

### 23. config-provenance

- Purpose: Show exactly where each effective setting originated.
- First working version: Merge layered configs with per-key provenance and redaction.
- Acceptance check: Secret-valued settings remain redacted in all reports.
- Status: proposed; not implemented.

### 24. release-evidence

- Purpose: Collect reproducible test and build evidence for releases.
- First working version: Generate a manifest linking a commit to checks and artifact hashes.
- Acceptance check: Changing an artifact invalidates its recorded hash.
- Status: proposed; not implemented.

## Learning and accessibility

### 25. concept-cartographer

- Purpose: Map prerequisites and explain why a learner is stuck.
- First working version: Build a manually authored concept graph and diagnostic exercises.
- Acceptance check: Recommendations trace to explicit prerequisite rules.
- Status: proposed; not implemented.

### 26. misconception-lab

- Purpose: Distinguish common mathematical mistakes using worked examples.
- First working version: Create a rule-based algebra diagnostic with transparent explanations.
- Acceptance check: Curated mistake fixtures receive the correct diagnosis.
- Status: proposed; not implemented.

### 27. study-recall-engine

- Purpose: Schedule retrieval practice using locally stored learning history.
- First working version: Build spaced-repetition scheduling with exportable progress.
- Acceptance check: Schedule calculations pass fixed-date fixtures.
- Status: proposed; not implemented.

### 28. accessible-equation-reader

- Purpose: Convert supported equations into navigable spoken descriptions.
- First working version: Parse a restricted math grammar into structured reading steps.
- Acceptance check: Unsupported notation is explicitly flagged.
- Status: proposed; not implemented.

### 29. caption-repair-workbench

- Purpose: Review caption timing and terminology with confidence cues.
- First working version: Import subtitles and flag overlaps, gaps, and glossary mismatches.
- Acceptance check: Timing violations in fixtures are found without silently rewriting text.
- Status: proposed; not implemented.

### 30. keyboard-path-auditor

- Purpose: Inspect keyboard navigation in a local demonstration website.
- First working version: Record focus order and detect unreachable interactive controls.
- Acceptance check: Known focus traps are identified in the demo.
- Status: proposed; not implemented.

### 31. reading-lens

- Purpose: Offer user-controlled reading layouts without changing source meaning.
- First working version: Build spacing, contrast, and line-length controls with saved preferences.
- Acceptance check: Original text remains identical across layout modes.
- Status: proposed; not implemented.

### 32. lab-notebook-replay

- Purpose: Turn scientific notebook steps into a reproducible learning trail.
- First working version: Store inputs, parameters, outputs, and explicit dependencies.
- Acceptance check: Replaying the fixture notebook reproduces its outputs.
- Status: proposed; not implemented.

## Climate and infrastructure

### 33. repair-route

- Purpose: Plan shared repair visits under time and travel constraints.
- First working version: Implement a small routing solver with transparent assumptions.
- Acceptance check: All accepted jobs satisfy configured appointment windows.
- Status: proposed; not implemented.

### 34. water-loss-sandbox

- Purpose: Explore leak detection on synthetic water-meter streams.
- First working version: Generate demand patterns and compare baseline anomaly detectors.
- Acceptance check: Report precision and recall on labeled synthetic events.
- Status: proposed; not implemented.

### 35. heat-route

- Purpose: Compare walking routes using user-supplied shade and temperature data.
- First working version: Build a graph router with distance and heat-exposure costs.
- Acceptance check: Each route discloses data sources and missing measurements.
- Status: proposed; not implemented.

### 36. solar-load-playground

- Purpose: Explore household load shifting using supplied generation profiles.
- First working version: Simulate appliance schedules and storage constraints.
- Acceptance check: Energy accounting balances within numeric tolerance.
- Status: proposed; not implemented.

### 37. food-rescue-matcher

- Purpose: Match surplus food offers to collection capacity and time windows.
- First working version: Build an allocation solver with explicit suitability constraints.
- Acceptance check: No match violates capacity or collection deadlines.
- Status: proposed; not implemented.

### 38. material-passport

- Purpose: Track repair history and material composition of reusable objects.
- First working version: Create signed record exports and an object-history viewer.
- Acceptance check: Tampered exported records fail integrity verification.
- Status: proposed; not implemented.

### 39. flood-scenario-table

- Purpose: Compare hypothetical drainage scenarios using supplied terrain grids.
- First working version: Implement a clearly labeled educational flow simulation.
- Acceptance check: Boundary conditions and conservation checks are tested.
- Status: proposed; not implemented.

### 40. transit-reliability-lens

- Purpose: Compare scheduled and observed arrival reliability from uploaded data.
- First working version: Parse transit CSV fixtures and show delay distributions.
- Acceptance check: Missing observations remain distinct from on-time arrivals.
- Status: proposed; not implemented.

## Personal and community tools

### 41. attention-budget

- Purpose: Help people inspect notification patterns without uploading message contents.
- First working version: Import metadata and model user-defined quiet periods.
- Acceptance check: Message bodies are rejected by the import schema.
- Status: proposed; not implemented.

### 42. decision-trace

- Purpose: Preserve assumptions behind decisions and revisit them when evidence changes.
- First working version: Build a local decision journal with evidence links and review dates.
- Acceptance check: Every revision retains its prior assumptions.
- Status: proposed; not implemented.

### 43. skill-exchange-matcher

- Purpose: Match community learning offers with requests using explicit preferences.
- First working version: Implement consent-based listings and a transparent matching score.
- Acceptance check: Excluded pairings never appear in recommendations.
- Status: proposed; not implemented.

### 44. mutual-aid-inventory

- Purpose: Track shared supplies with offline reservations and reconciliation.
- First working version: Build inventory events and conflict handling for two offline clients.
- Acceptance check: Reconciliation surfaces oversubscription rather than hiding it.
- Status: proposed; not implemented.

### 45. meeting-action-proof

- Purpose: Link manually recorded action items to exact supporting notes.
- First working version: Build a notes editor with source anchors and ownership tracking.
- Acceptance check: Broken source references are flagged after edits.
- Status: proposed; not implemented.

### 46. household-fairness-simulator

- Purpose: Explore chore allocation using availability and user-defined effort estimates.
- First working version: Build a constrained assignment solver and fairness reports.
- Acceptance check: Assignments respect availability and explain unmet demand.
- Status: proposed; not implemented.

### 47. personal-data-map

- Purpose: Inventory where a user stores data without collecting account credentials.
- First working version: Build a local catalog of services, categories, and retention reminders.
- Acceptance check: Exports contain no authentication secrets.
- Status: proposed; not implemented.

### 48. community-language-kit

- Purpose: Manage human-reviewed translations for small community services.
- First working version: Build glossary checks, review status, and locale export.
- Acceptance check: Unreviewed translations cannot be marked approved automatically.
- Status: proposed; not implemented.

## Data and research

### 49. dataset-lineage-map

- Purpose: Trace transformations from source files to published tables.
- First working version: Record transformation metadata and content hashes.
- Acceptance check: Changing a source marks dependent outputs stale.
- Status: proposed; not implemented.

### 50. synthetic-data-bench

- Purpose: Compare utility and disclosure risks of synthetic-data generators.
- First working version: Run baseline generators on non-sensitive fixture datasets.
- Acceptance check: Reports separate utility metrics from privacy guarantees.
- Status: proposed; not implemented.

### 51. uncertainty-notebook

- Purpose: Propagate measurement uncertainty through simple calculations.
- First working version: Implement sampled uncertainty and sensitivity plots.
- Acceptance check: Analytical fixture cases match numerical intervals.
- Status: proposed; not implemented.

### 52. missingness-lens

- Purpose: Show how missing-data assumptions affect conclusions.
- First working version: Compare explicit imputation strategies on labeled fixtures.
- Acceptance check: Original values and imputed values remain distinguishable.
- Status: proposed; not implemented.

### 53. fairness-slice-audit

- Purpose: Inspect model performance across user-defined dataset slices.
- First working version: Compute slice metrics with sample sizes and uncertainty estimates.
- Acceptance check: Small samples are clearly marked and never hidden.
- Status: proposed; not implemented.

### 54. citation-provenance

- Purpose: Track which research claims are supported by which supplied passages.
- First working version: Build a manual evidence graph with quote offsets.
- Acceptance check: Every cited passage resolves to the imported source.
- Status: proposed; not implemented.

### 55. experiment-budgeter

- Purpose: Compare experiment designs under cost and sample constraints.
- First working version: Build power simulations for a documented restricted set of designs.
- Acceptance check: Outputs reproduce with fixed seeds and disclose assumptions.
- Status: proposed; not implemented.

### 56. data-retention-engine

- Purpose: Apply explicit retention rules to a disposable dataset.
- First working version: Implement expiry evaluation, dry runs, and deletion receipts.
- Acceptance check: Dry runs never mutate data and expired fixtures are correctly selected.
- Status: proposed; not implemented.

## Agent and automation engineering

### 57. agent-permission-gate

- Purpose: Constrain automation actions with typed capabilities and approval rules.
- Implemented prototype: [Browser workbench + JavaScript/Python policy engines](https://github.com/Royalpuskar/agent-permission-gate), mock requests, explicit default-deny decisions, and automated tests.
- Acceptance check: Unknown actions and missing grants default to denial in the test fixtures.
- Status: **research prototype implemented**, not a production enforcement service.

### 58. tool-response-firewall

- Purpose: Keep retrieved content separate from trusted agent instructions.
- First working version: Build a test harness with hostile synthetic tool responses.
- Acceptance check: Tests measure boundary failures without claiming universal protection.
- Status: proposed; not implemented.

### 59. automation-dry-run

- Purpose: Preview an automation's proposed writes before execution.
- First working version: Implement typed action plans, diffs, and a mock executor.
- Acceptance check: Execution rejects a plan whose reviewed hash has changed.
- Status: proposed; not implemented.

### 60. agent-memory-expiry

- Purpose: Manage scoped assistant memory with expiry and deletion receipts.
- First working version: Build a local memory store with provenance and TTL policies.
- Acceptance check: Expired records are excluded from every retrieval path.
- Status: proposed; not implemented.

### 61. workflow-counterexample

- Purpose: Find small inputs that violate declared workflow invariants.
- First working version: Explore bounded state transitions and return replayable traces.
- Acceptance check: Known unsafe fixture workflows produce minimal failure traces.
- Status: **research prototype implemented** with a live browser demo and automated tests; not a production service.

### 62. model-routing-bench

- Purpose: Compare model-routing policies under measured cost and latency constraints.
- First working version: Implement provider adapters with deterministic mock responses.
- Acceptance check: Mock runs are labeled separately from real benchmark measurements.
- Status: proposed; not implemented.

### 63. human-handoff-router

- Purpose: Route uncertain automation results to an appropriate human review queue.
- First working version: Build explicit escalation rules and queue ownership with synthetic cases.
- Acceptance check: Blocked actions remain blocked until the required review occurs.
- Status: proposed; not implemented.

### 64. evidence-first-assistant

- Purpose: Require answer claims to point to retrieved source spans.
- First working version: Build a retrieval demo with claim-to-passage links and abstention.
- Acceptance check: Unsupported fixture questions trigger an explicit insufficient-evidence response.
- Status: proposed; not implemented.


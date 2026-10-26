# GPT/Codex → DSH Design Agent Workflow Migration Experiment

[中文主 README](README.md) · [Capability matrix](docs/capability-matrix.md) · [Validation plan](docs/validation-plan.md) · [Evidence register](docs/evidence-register.md)

This independent documentation project records an attempt to adapt a GPT/Codex design workflow to a friend's DSH design Agent system. It documents art direction, layout planning, production, critique, revision, rollback, style knowledge and persistent task state. It is not an installable Agent distribution.

**Status as of 2026-10-27: the supplied DSH acceptance report concludes “partial acceptance at this stage.” This documentation session read that report and inspected the supplied screenshot; it did not rerun the DSH system.**

## Reported results and evidence limits

The DSH report, dated 2026-10-26, covers internal version 2.3.2 against an upgrade brief labelled v3.0 / Art Director 2.0. It reports successful engineering-layer migration and one minimal art-direction trial. It does not establish a dual-backend comparison, a complete independent acceptance loop, transferable design knowledge, or executable automated rollback.

| Status in the DSH report | Count | Share |
|---|---:|---:|
| Implemented and verified by its audit, including historical evidence | 26 | 41.9% |
| Partially implemented | 21 | 33.9% |
| Documentation only | 1 | 1.6% |
| Implemented, not yet verified | 1 | 1.6% |
| Not implemented | 13 | 21.0% |

These are **reported classifications**, not 26 independently reproduced tests in this repository. The stated 41.9%–77.4% range is a count-based coverage range. Its 59.7% midpoint is not a measured success rate or quality score. Of seven completion criteria, the report marks one met, five partial and one unmet.

## Two distinct systems

- **User's GPT/Codex system:** the current local Visual Director skill, labelled 1.1.1, calls for host-provided OpenAI native image tools. Its rules do not connect Photoshop or external image backends. The original readable user message also requested a separate GPT/image-model workflow without PS. Reading the skill proves its written rules, not runtime acceptance.
- **Friend's DSH system:** the report identifies DeepSeek as controller, Qwen for visual critique and analysis cards, ComfyUI for historical image generation, and Photoshop for editable layout execution. None of these integrations can be inferred to exist in the user's Codex environment.

The migration preserves the intended **Qwen API + ComfyUI backend choice**. Qwen's reported critique calls do not prove that a Qwen image-generation API was connected. The report says the second generation route was absent and ComfyUI was stopped at audit time; it establishes no same-brief comparison or currently available dual backend.

PS and Layout Planner remain in scope as **provided/reported, independently awaiting verification**. The report cites editable PSD output and layout contracts, while identifying missing leading, subject exclusion zones, imperfect alignment semantics and absent print output.

## What the workflow transfers

Art Director proposes distinct directions, tradeoffs and production routing. Layout Planner turns the approved brief into a verifiable contract. Critique checks objective conditions and visible design. Design Loop directs limited revisions, rejects unsupported feedback and stops when needed. Style Kit stores reusable mechanisms with applicability and failure examples. Persistent memory should recover the approved brief, selected version and next action across sessions.

The report supports only a partial implementation of that intent. It describes revision records and manual fallback, but an automated rollback command failed even in dry-run. Saved state does not establish successful cross-session recovery. Technique retrieval and references in a layout contract do not establish improved design or cross-task transfer.

## Visible v1.1 → v3.0 screenshot changes

The inspected user screenshot lists four stages becoming eight steps; three candidate references and a D0 user-selection gate; three gates becoming four; reference-match assessment before defect critique; a revision limit changing from three to seven; 25 numbered rules; corpus categories changing to character/editorial/promo/type; PS layout and glyph-design additions; and generated images excluded from references/candidates.

These are visible **statements in the screenshot**, not independently observed executions. The screenshot lists 50 techniques and 10 objective checks; the later report lists 46 techniques and nine runnable checks. The discrepancy remains unresolved. Screenshot v3.0, target internal v2.3.2 and local skill v1.1.1 are different version namespaces.

## Evidence policy and next work

The [evidence register](docs/evidence-register.md) separates direct observations in this session, source-side written rules, claims in the supplied report, and unverified items. The [original external report](evidence/DSH_DESIGN_AGENT_ACCEPTANCE_EXTERNAL.md) retains its author's wording; “verified” and “this audit” inside it refer to that author's audit.

The accessible conversation return contained a few user messages, assistant reference placeholders and one image attachment. It did not expose the complete earlier discussion or raw target-side logs, PSD files, source code or migration bundle.

Priorities are to bind brief acceptance criteria to fail-closed gates, demonstrate real rollback and cross-session recovery, correct or reject unsupported layout fields, then run a minimal same-brief Qwen API/ComfyUI comparison and a controlled style-transfer trial. Evidence must identify the exact artifact version. Do not claim better aesthetics, autonomous art direction, statistical model rankings or unattended delivery without appropriate experiments and human acceptance.

This repository is separate from the original Skill project. It contains documentation and user-authorized external evidence, not credentials or the complete DSH implementation. See [publication status](docs/publication-status.md) for whether a remote repository was actually created.

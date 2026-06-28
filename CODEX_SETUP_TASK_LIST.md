# Codex Setup Task List

Version: v0.2  
Status: Draft — Mandatory Read Rule Added  
Owner: Shubham Bansal  
Last Updated: 2026-06-28  

## 0. Purpose

This file is the source-of-truth task list for setting up Codex as a disciplined dev-team operating system.

This file is **not** the product PRD, not the architecture spec, not the main code repository documentation, and not the implementation backlog for the actual product.

Its job is to prevent drift while setting up the meta-system that will later help create product discovery, specs, PRD, ADRs, issue slices, design system, implementation workflow, and maintenance process.

## 1. Source-of-Truth Rule

This file wins over chat memory.

Before ChatGPT, Codex, Claude, or any agent gives setup work, it must refer to this file and identify the current phase/task being worked on.

If chat history conflicts with this file, this file wins.

## 2. Mandatory Read / Reference Rule

This file is not only a checklist. It is the operating protocol for how setup work must proceed.

Before giving any setup-related guidance, ChatGPT, Codex, Claude, or any assistant/agent must read or refer to this task list and identify the current phase and task ID being worked on.

For every setup-related response, the assistant/agent must:

- identify the relevant phase/task ID;
- state whether the response is discussion, decision, or execution;
- cover only 1–2 steps unless Shubham explicitly asks for more;
- avoid creating or suggesting files, prompts, commands, docs, repo structure, or setup artifacts unless explicitly approved;
- avoid pre-deciding future phases;
- update or suggest updates to this task list when progress is made;
- stop and ask for the latest file content or repo link if it cannot access the latest version of this file.

P0 is therefore both:
- the phase where working rules are approved; and
- the standing protocol that governs every setup-related response.

## 3. Control Rules

- No setup commands, files, prompts, docs, repo structure, tool installation, or generated artifacts may be created unless explicitly approved by Shubham.
- No phase, task, file, prompt, command, or setup artifact may be added without explicit approval.
- Nothing should be called “minimal,” “simple,” “MVP,” or “good enough” unless Shubham agrees with that framing.
- Every assistant response should cover only 1–2 steps unless Shubham explicitly asks for more.
- The assistant must not jump from discussion to execution.
- The assistant must not decide future documentation in advance. Documentation decisions happen in the relevant phase.
- The assistant must not decide subagents, skills, ADRs, design-system files, product docs, or build artifacts before the relevant phase is reached.
- The assistant must use exact phase/task IDs when giving guidance.
- “Approved” means Shubham explicitly accepted the item.
- “Discussed” does not mean “approved.”
- “Suggested” does not mean “approved.”
- “Likely” does not mean “approved.”
- Product/spec/PRD/build work comes only after the setup system allows it.

## 4. How To Mark Progress

Use Markdown checkboxes and strikethrough.

### Not Started

```md
- [ ] P1-T01 Define what Codex is responsible for.
```

### Completed

```md
- [x] ~~P1-T01 Define what Codex is responsible for.~~  
  Completed: 2026-06-28  
  Decision/Note: Codex responsibilities approved in P1 decision notes.
```

### Blocked

```md
- [ ] P1-T01 Define what Codex is responsible for.  
  Status: Blocked  
  Blocker: Waiting for Shubham to approve responsibility boundary.
```

### Deferred

```md
- [ ] P1-T01 Define what Codex is responsible for.  
  Status: Deferred  
  Reason: Will revisit after P2 skills discussion.
```

## 5. Versioning Rules

- Every meaningful change increments the version number.
- Small wording clarification: patch version, e.g. `v0.1.1`.
- Added/removed/reordered task: minor version, e.g. `v0.2`.
- Major change to the setup approach: major version, e.g. `v1.0`.
- Every version change must add a changelog entry.

## 6. Changelog

### v0.2 — Mandatory Read Rule Added
- Added a Mandatory Read / Reference Rule.
- Clarified that this file is an operating protocol, not only a checklist.
- Clarified that P0 is both an approval phase and a standing protocol for every setup-related response.
- Added explicit requirement that every setup-related response identify the current phase/task ID.
- Added explicit requirement to stop and ask for the latest file content or repo link if the latest file cannot be accessed.

### v0.1 — Draft
- Created the first source-of-truth task list for setting up Codex as a dev-team operating system.
- Defined P0–P12.
- Added control rules, source-of-truth rule, progress marking rules, and fixed phase/task IDs.

---

# Phase Summary

| Phase | Name | Status | Purpose |
|---|---|---|---|
| P0 | Working rules between Shubham and assistant | In Progress | Stabilize how setup guidance will be given |
| P1 | Define the Codex operating system | Not Started | Decide how Codex should behave as a dev/product team |
| P2 | Choose core skills/workflows | Not Started | Decide what Codex skills/workflows are needed |
| P3 | Define subagent roles | Not Started | Decide virtual team roles and decision boundaries |
| P4 | Define documentation system | Not Started | Decide what persistent docs are needed and how they are governed |
| P5 | Define ADR process | Not Started | Decide how architecture/product decisions are recorded |
| P6 | Define discovery and interview engine | Not Started | Decide how stakeholder/worklog discovery will work |
| P7 | Define product specification engine | Not Started | Decide how discovery becomes specs/PRD/backlog |
| P8 | Define DDD/domain modeling engine | Not Started | Decide how workflows become domain model and boundaries |
| P9 | Define design system engine | Not Started | Decide how custom UI consistency will be handled |
| P10 | Define issue slicing engine | Not Started | Decide how work becomes complete vertical slices |
| P11 | Define implementation and review engine | Not Started | Decide coding, testing, review, and verification rules |
| P12 | Define maintenance and learning loop | Not Started | Decide long-term review, drift control, and improvement process |

---

# P0 — Working Rules Between Shubham and Assistant

Status: In Progress

## Goal

Decide how Shubham and the assistant will proceed before touching Codex setup, product specs, docs, prompts, commands, or files.

P0 also defines the standing protocol that the assistant must follow before every setup-related response.

## Tasks

- [ ] P0-T01 Confirm that every assistant response should cover only 1–2 steps unless Shubham asks for more.
- [ ] P0-T02 Confirm that the assistant must not create files, prompts, commands, docs, repo structure, setup steps, or artifacts without explicit approval.
- [ ] P0-T03 Confirm that this file is the source of truth for setup sequence and progress.
- [ ] P0-T04 Confirm that discussion and execution are separate.
- [ ] P0-T05 Confirm that “approved” only means Shubham explicitly accepted an item.
- [ ] P0-T06 Confirm that chat memory is not source of truth.
- [ ] P0-T07 Confirm that no future docs, skills, subagents, ADRs, or product artifacts are pre-approved by appearing in discussion.
- [ ] P0-T08 Confirm that the assistant must reference exact phase/task IDs before giving setup instructions.
- [ ] P0-T09 Confirm that if the assistant drifts, Shubham can reset the work by pointing back to this file.
- [ ] P0-T10 Confirm how this file itself will be updated.
- [ ] P0-T11 Confirm whether updates to this file are done manually by Shubham, by patch/diff from assistant, or through repo changes.
- [ ] P0-T12 Confirm what counts as completion of P0.
- [ ] P0-T13 Confirm that P0 remains a standing protocol even after the phase is completed.
- [ ] P0-T14 Confirm that every setup-related response must identify the current phase/task ID.
- [ ] P0-T15 Confirm that if the assistant cannot access the latest task-list file, it must ask Shubham for the current file content or repo link before continuing setup work.

## Completion Criteria

P0 is complete only when:

- Working rules are approved.
- This file location is approved.
- File update method is approved.
- Assistant has acknowledged that this file controls the setup process.
- Assistant has acknowledged that P0 remains a standing protocol after completion.
- Assistant has acknowledged that it must read or refer to this task list before setup-related guidance.

## Output

Approved working agreement for how Shubham and the assistant proceed.

---

# P1 — Define the Codex Operating System

Status: Not Started

## Goal

Decide how Codex should behave like a disciplined dev/product team rather than a random code generator.

## Tasks

- [ ] P1-T01 Define what Codex is responsible for during setup.
- [ ] P1-T02 Define what Codex is responsible for during product discovery.
- [ ] P1-T03 Define what Codex is responsible for during specification/PRD creation.
- [ ] P1-T04 Define what Codex is responsible for during implementation.
- [ ] P1-T05 Define what Codex is responsible for during review.
- [ ] P1-T06 Define what Codex is not allowed to decide alone.
- [ ] P1-T07 Define Shubham’s role as final decision owner.
- [ ] P1-T08 Define how Codex should challenge assumptions.
- [ ] P1-T09 Define how Codex should ask clarifying questions.
- [ ] P1-T10 Define when Codex should stop and ask for approval.
- [ ] P1-T11 Define how Codex should record decisions.
- [ ] P1-T12 Define how Codex should handle uncertainty.
- [ ] P1-T13 Define how Codex should avoid overbuilding.
- [ ] P1-T14 Define how Codex should avoid premature implementation.
- [ ] P1-T15 Define how Codex should complete a slice of work.
- [ ] P1-T16 Define what “done” means at operating-system level.
- [ ] P1-T17 Define when Codex must update task/status records.
- [ ] P1-T18 Define when Codex must recommend creating or updating a decision record.
- [ ] P1-T19 Define how Codex should behave when instructions conflict.
- [ ] P1-T20 Define how Codex should summarize progress at the end of work.

## Completion Criteria

P1 is complete only when:

- Codex responsibilities are approved.
- Codex boundaries are approved.
- Shubham’s final-decision role is approved.
- Operating rules are ready to be converted into persistent Codex instructions later, if approved in a later phase.

## Output

Approved Codex operating principles.

---

# P2 — Choose Core Skills / Workflows

Status: Not Started

## Goal

Decide which reusable skills/workflows Codex should use and in what sequence.

## Tasks

- [ ] P2-T01 Define what a “skill/workflow” means in this setup.
- [ ] P2-T02 Decide whether external engineering skills should be used.
- [ ] P2-T03 Decide whether a discovery/grilling skill is needed.
- [ ] P2-T04 Decide whether a domain-modeling skill is needed.
- [ ] P2-T05 Decide whether a PRD-generation skill is needed.
- [ ] P2-T06 Decide whether an issue-slicing skill is needed.
- [ ] P2-T07 Decide whether a TDD skill is needed.
- [ ] P2-T08 Decide whether a bug-diagnosis skill is needed.
- [ ] P2-T09 Decide whether an architecture-improvement skill is needed.
- [ ] P2-T10 Decide whether a pre-commit/quality-gate skill is needed.
- [ ] P2-T11 Decide which skills are mandatory.
- [ ] P2-T12 Decide which skills are optional.
- [ ] P2-T13 Decide which skills are explicitly rejected.
- [ ] P2-T14 Decide where skills should live, if any are approved.
- [ ] P2-T15 Decide how skills should be invoked.
- [ ] P2-T16 Decide whether skills should run automatically or only when instructed.
- [ ] P2-T17 Decide how skill outputs should be reviewed.
- [ ] P2-T18 Decide how skill outputs become accepted decisions.
- [ ] P2-T19 Decide how to prevent skill overlap and contradictory outputs.
- [ ] P2-T20 Decide how skill usage should be recorded.

## Completion Criteria

P2 is complete only when:

- Approved skills/workflows are identified.
- Rejected/deferred skills are documented.
- Invocation rules are approved.
- No skill is treated as active before approval.

## Output

Approved skill/workflow list and usage sequence.

---

# P3 — Define Subagent Roles

Status: Not Started

## Goal

Decide which virtual team roles Codex should simulate, what each role owns, and what each role is forbidden from deciding.

## Tasks

- [ ] P3-T01 Define what a “subagent” means in this setup.
- [ ] P3-T02 Decide whether subagents are needed at all.
- [ ] P3-T03 Define criteria for creating a subagent role.
- [ ] P3-T04 Identify candidate subagent roles for discussion.
- [ ] P3-T05 Define each approved subagent’s responsibility.
- [ ] P3-T06 Define each approved subagent’s forbidden areas.
- [ ] P3-T07 Define when each subagent should be used.
- [ ] P3-T08 Define when each subagent should not be used.
- [ ] P3-T09 Define whether subagents can create artifacts or only review/propose.
- [ ] P3-T10 Define how subagent outputs are summarized.
- [ ] P3-T11 Define how subagent disagreements are handled.
- [ ] P3-T12 Define how final decisions are accepted.
- [ ] P3-T13 Define whether there should be a product role.
- [ ] P3-T14 Define whether there should be a DDD/domain role.
- [ ] P3-T15 Define whether there should be a data/architecture role.
- [ ] P3-T16 Define whether there should be an AI/matching role.
- [ ] P3-T17 Define whether there should be a security/compliance role.
- [ ] P3-T18 Define whether there should be a UX/design role.
- [ ] P3-T19 Define whether there should be an implementation-pragmatist role.
- [ ] P3-T20 Define whether there should be a code-review role.
- [ ] P3-T21 Define whether there should be an ADR/decision-record role.
- [ ] P3-T22 Decide which subagents are approved, rejected, or deferred.

## Completion Criteria

P3 is complete only when:

- Approved subagents are defined.
- Each role has responsibility and boundary.
- Conflict-resolution method is approved.
- Final-decision process is approved.

## Output

Approved subagent charter.

---

# P4 — Define Documentation System

Status: Not Started

## Goal

Decide what persistent documents are needed, how they are governed, and how to prevent documentation bloat.

## Tasks

- [ ] P4-T01 Define why documentation is needed in the Codex setup.
- [ ] P4-T02 Define what counts as a persistent document.
- [ ] P4-T03 Define what counts as temporary scratch work.
- [ ] P4-T04 Decide which document categories are needed.
- [ ] P4-T05 Decide whether any setup instruction file is needed.
- [ ] P4-T06 Decide whether any context file is needed.
- [ ] P4-T07 Decide whether any glossary/domain-language file is needed.
- [ ] P4-T08 Decide whether any workflow file is needed.
- [ ] P4-T09 Decide whether any architecture/system-boundary file is needed.
- [ ] P4-T10 Decide whether any product/specification file is needed later.
- [ ] P4-T11 Decide whether any testing/quality file is needed.
- [ ] P4-T12 Decide whether any security/governance file is needed.
- [ ] P4-T13 Decide whether any design-system file is needed.
- [ ] P4-T14 Decide whether any integration file is needed.
- [ ] P4-T15 Define who or what updates each approved document.
- [ ] P4-T16 Define when each approved document must be updated.
- [ ] P4-T17 Define how documents relate to decisions.
- [ ] P4-T18 Define how documents relate to implementation tasks.
- [ ] P4-T19 Define how Codex should avoid bloated docs.
- [ ] P4-T20 Define how outdated docs are detected.
- [ ] P4-T21 Define how conflicting docs are resolved.
- [ ] P4-T22 Decide documentation storage rules.
- [ ] P4-T23 Decide naming conventions for approved documents.
- [ ] P4-T24 Decide whether any document should be created immediately after P4.
- [ ] P4-T25 Decide what completion of documentation setup means.

## Completion Criteria

P4 is complete only when:

- Approved documentation categories are defined.
- Future document creation rules are approved.
- Update rules are approved.
- No document is created merely because it was discussed.

## Output

Approved documentation system.

---

# P5 — Define ADR / Decision Record Process

Status: Not Started

## Goal

Define how important product/architecture/process decisions are recorded, accepted, changed, or superseded.

## Tasks

- [ ] P5-T01 Define what an ADR or decision record is for this setup.
- [ ] P5-T02 Decide whether the term “ADR” should be used or whether another term is preferred.
- [ ] P5-T03 Define what kinds of decisions require a record.
- [ ] P5-T04 Define what kinds of decisions do not require a record.
- [ ] P5-T05 Define decision status values.
- [ ] P5-T06 Define decision ownership.
- [ ] P5-T07 Define who can approve a decision.
- [ ] P5-T08 Define how rejected decisions are recorded.
- [ ] P5-T09 Define how superseded decisions are recorded.
- [ ] P5-T10 Define how temporary decisions are recorded.
- [ ] P5-T11 Define decision template fields.
- [ ] P5-T12 Define how alternatives are captured.
- [ ] P5-T13 Define how consequences/trade-offs are captured.
- [ ] P5-T14 Define how reversal cost is captured.
- [ ] P5-T15 Define how decisions are linked to phases/tasks.
- [ ] P5-T16 Define how decisions are linked to future product/build work.
- [ ] P5-T17 Identify first candidate decisions for discussion.
- [ ] P5-T18 Decide which candidate decisions should be recorded now.
- [ ] P5-T19 Decide where decision records live, if approved.
- [ ] P5-T20 Decide how Codex should check existing decisions before proposing changes.
- [ ] P5-T21 Decide how often decisions should be reviewed.
- [ ] P5-T22 Decide how to prevent decision-record bloat.

## Completion Criteria

P5 is complete only when:

- Decision-record process is approved.
- Decision status model is approved.
- Approval/supersession process is approved.
- First decision records are identified only if Shubham approves.

## Output

Approved decision-record governance model.

---

# P6 — Define Discovery and Interview Engine

Status: Not Started

## Goal

Define how Codex should help interview Shubham/stakeholders, capture real worklogs, and convert them into workflows without jumping to product features too early.

## Tasks

- [ ] P6-T01 Define the goal of discovery.
- [ ] P6-T02 Define what must be discovered before product/spec work.
- [ ] P6-T03 Define stakeholder categories to consider.
- [ ] P6-T04 Define how to handle cases where Shubham is proxying for stakeholders.
- [ ] P6-T05 Define interview principles.
- [ ] P6-T06 Define how Codex should ask worklog-based questions.
- [ ] P6-T07 Define how Codex should avoid asking generic feature-wishlist questions too early.
- [ ] P6-T08 Define worklog capture format.
- [ ] P6-T09 Define how to capture current workflow steps.
- [ ] P6-T10 Define how to capture pain points.
- [ ] P6-T11 Define how to capture decision points.
- [ ] P6-T12 Define how to capture tools/data used today.
- [ ] P6-T13 Define how to capture exceptions and edge cases.
- [ ] P6-T14 Define how to capture confidentiality/governance concerns.
- [ ] P6-T15 Define how interviews become workflow maps.
- [ ] P6-T16 Define how workflow maps are validated.
- [ ] P6-T17 Define how contradictions between stakeholders are handled.
- [ ] P6-T18 Define how assumptions are recorded.
- [ ] P6-T19 Define when discovery is “enough” to move to specification.
- [ ] P6-T20 Define how discovery outputs are updated later.
- [ ] P6-T21 Define what Codex may create during discovery.
- [ ] P6-T22 Define what Codex must not create during discovery.

## Completion Criteria

P6 is complete only when:

- Discovery method is approved.
- Interview/worklog format is approved.
- Rules for converting discovery to workflows are approved.
- Boundaries preventing premature feature design are approved.

## Output

Approved discovery and interview engine.

---

# P7 — Define Product Specification Engine

Status: Not Started

## Goal

Define how discovery outputs become product specs, PRD, user stories, acceptance criteria, and MVP scope.

## Tasks

- [ ] P7-T01 Define what product specification means in this setup.
- [ ] P7-T02 Define when product specification is allowed to begin.
- [ ] P7-T03 Define required inputs from discovery.
- [ ] P7-T04 Define PRD structure, if a PRD is approved.
- [ ] P7-T05 Define workflow-catalogue structure.
- [ ] P7-T06 Define user-story format.
- [ ] P7-T07 Define acceptance-criteria format.
- [ ] P7-T08 Define non-functional requirement capture.
- [ ] P7-T09 Define product assumption capture.
- [ ] P7-T10 Define product risk capture.
- [ ] P7-T11 Define open-question capture.
- [ ] P7-T12 Define prioritization method.
- [ ] P7-T13 Define MVP framing rules.
- [ ] P7-T14 Define how Codex should challenge product assumptions.
- [ ] P7-T15 Define how Codex should avoid jumping to implementation.
- [ ] P7-T16 Define how product specs relate to DDD/domain modeling.
- [ ] P7-T17 Define how product specs relate to design-system work.
- [ ] P7-T18 Define how product specs relate to issue slicing.
- [ ] P7-T19 Define approval process for product specs.
- [ ] P7-T20 Define how product specs change over time.
- [ ] P7-T21 Define completion criteria for a product spec.

## Completion Criteria

P7 is complete only when:

- Product specification process is approved.
- PRD/user-story/acceptance criteria approach is approved if needed.
- Approval rules are defined.
- Product specification does not start until allowed by this process.

## Output

Approved product specification process.

---

# P8 — Define DDD / Domain Modeling Engine

Status: Not Started

## Goal

Define how workflows and product needs are converted into domain language, bounded contexts, entities, value objects, commands, events, business rules, and source-of-truth boundaries.

## Tasks

- [ ] P8-T01 Define what DDD means for this project setup.
- [ ] P8-T02 Define when domain modeling should happen.
- [ ] P8-T03 Define required inputs from discovery/specification.
- [ ] P8-T04 Define ubiquitous-language capture rules.
- [ ] P8-T05 Define bounded-context format.
- [ ] P8-T06 Define aggregate format.
- [ ] P8-T07 Define entity format.
- [ ] P8-T08 Define value-object format.
- [ ] P8-T09 Define command format.
- [ ] P8-T10 Define domain-event format.
- [ ] P8-T11 Define business-rule format.
- [ ] P8-T12 Define state-machine format.
- [ ] P8-T13 Define source-of-truth rule format.
- [ ] P8-T14 Define integration-boundary rule format.
- [ ] P8-T15 Define how domain terms are validated.
- [ ] P8-T16 Define how conflicting domain terms are resolved.
- [ ] P8-T17 Define how domain model links to data model later.
- [ ] P8-T18 Define how domain model links to UI/workflows.
- [ ] P8-T19 Define how domain model links to decision records.
- [ ] P8-T20 Define how Codex should challenge weak domain models.
- [ ] P8-T21 Define how domain model changes are governed.
- [ ] P8-T22 Define completion criteria for domain modeling.

## Completion Criteria

P8 is complete only when:

- Domain modeling process is approved.
- Formats are approved.
- Source-of-truth and boundary handling are approved.
- Domain modeling work is not confused with implementation.

## Output

Approved DDD/domain modeling process.

---

# P9 — Define Design System Engine

Status: Not Started

## Goal

Define whether and how a design system should exist for the custom UI, without turning it into an uncontrolled side project.

## Tasks

- [ ] P9-T01 Define why a design system may be needed.
- [ ] P9-T02 Decide whether a design system is mandatory, optional, deferred, or rejected.
- [ ] P9-T03 Define what a design system means in this setup.
- [ ] P9-T04 Define what a design system must not become.
- [ ] P9-T05 Decide whether Claude or another tool should help design it.
- [ ] P9-T06 Decide whether Codex should implement it.
- [ ] P9-T07 Decide whether a base UI stack should be selected.
- [ ] P9-T08 Decide whether component stories are required.
- [ ] P9-T09 Define product-specific component discovery process.
- [ ] P9-T10 Define screen-pattern discovery process.
- [ ] P9-T11 Define empty/loading/error-state requirements.
- [ ] P9-T12 Define accessibility expectations.
- [ ] P9-T13 Define design token expectations.
- [ ] P9-T14 Define when a new component is allowed.
- [ ] P9-T15 Define when a one-off UI is allowed.
- [ ] P9-T16 Define how design-system changes are reviewed.
- [ ] P9-T17 Define how design-system work links to product specs.
- [ ] P9-T18 Define how design-system work links to issue slicing.
- [ ] P9-T19 Define how design-system work avoids overbuilding.
- [ ] P9-T20 Define completion criteria for design-system setup.

## Completion Criteria

P9 is complete only when:

- Design-system stance is approved.
- Tooling/help approach is approved if needed.
- Component/pattern governance is approved.
- No design-system files/components are created before approval.

## Output

Approved design-system process.

---

# P10 — Define Issue Slicing Engine

Status: Not Started

## Goal

Define how product/spec work becomes complete, independently valuable vertical slices.

## Tasks

- [ ] P10-T01 Define what a vertical slice means.
- [ ] P10-T02 Define what is not a vertical slice.
- [ ] P10-T03 Define issue template.
- [ ] P10-T04 Define acceptance-criteria requirements.
- [ ] P10-T05 Define testing requirements per issue.
- [ ] P10-T06 Define documentation requirements per issue.
- [ ] P10-T07 Define review requirements per issue.
- [ ] P10-T08 Define security/data review requirements per issue.
- [ ] P10-T09 Define UI state requirements per issue.
- [ ] P10-T10 Define backend/API requirements per issue.
- [ ] P10-T11 Define database/migration requirements per issue.
- [ ] P10-T12 Define AI behavior requirements per issue, if relevant.
- [ ] P10-T13 Define observability/logging/audit requirements per issue, if relevant.
- [ ] P10-T14 Define handoff format.
- [ ] P10-T15 Define issue labels.
- [ ] P10-T16 Define issue priority method.
- [ ] P10-T17 Define dependency handling.
- [ ] P10-T18 Define spike/research issue rules.
- [ ] P10-T19 Define bug issue rules.
- [ ] P10-T20 Define refactor issue rules.
- [ ] P10-T21 Define when an issue can be started.
- [ ] P10-T22 Define when an issue is done.
- [ ] P10-T23 Define how incomplete work is handled.
- [ ] P10-T24 Define how issue slicing avoids horizontal-only tasks.
- [ ] P10-T25 Define completion criteria for the issue slicing engine.

## Completion Criteria

P10 is complete only when:

- Vertical-slice definition is approved.
- Issue template is approved.
- Done criteria are approved.
- Review and handoff requirements are approved.

## Output

Approved vertical-slice delivery system.

---

# P11 — Define Implementation and Review Engine

Status: Not Started

## Goal

Define how Codex should implement work with engineering discipline: tests, quality gates, review, verification, and safe changes.

## Tasks

- [ ] P11-T01 Define implementation principles.
- [ ] P11-T02 Define when implementation is allowed to begin.
- [ ] P11-T03 Define coding rules.
- [ ] P11-T04 Define TDD expectations.
- [ ] P11-T05 Define test levels.
- [ ] P11-T06 Define migration rules.
- [ ] P11-T07 Define API contract rules.
- [ ] P11-T08 Define frontend implementation rules.
- [ ] P11-T09 Define backend implementation rules.
- [ ] P11-T10 Define AI-related implementation rules.
- [ ] P11-T11 Define data/privacy implementation rules.
- [ ] P11-T12 Define error-handling expectations.
- [ ] P11-T13 Define loading/empty/error-state expectations for UI.
- [ ] P11-T14 Define logging/audit expectations.
- [ ] P11-T15 Define performance expectations.
- [ ] P11-T16 Define security review process.
- [ ] P11-T17 Define code review process.
- [ ] P11-T18 Define design review process, if relevant.
- [ ] P11-T19 Define test verification command expectations.
- [ ] P11-T20 Define manual verification expectations.
- [ ] P11-T21 Define “no done without verification” rule.
- [ ] P11-T22 Define how Codex should report changed files.
- [ ] P11-T23 Define how Codex should report known limitations.
- [ ] P11-T24 Define how Codex should avoid hidden breaking changes.
- [ ] P11-T25 Define how Codex should handle failed tests.
- [ ] P11-T26 Define how Codex should handle partial completion.
- [ ] P11-T27 Define completion criteria for implementation/review setup.

## Completion Criteria

P11 is complete only when:

- Implementation rules are approved.
- Test/review/verification rules are approved.
- Done criteria are approved.
- Codex cannot mark implementation complete without verification.

## Output

Approved implementation and review engine.

---

# P12 — Define Maintenance and Learning Loop

Status: Not Started

## Goal

Define how the Codex operating system stays useful over months/years without drifting, bloating, or becoming stale.

## Tasks

- [ ] P12-T01 Define why maintenance is needed.
- [ ] P12-T02 Define recurring review cadence.
- [ ] P12-T03 Define architecture review process.
- [ ] P12-T04 Define backlog review process.
- [ ] P12-T05 Define documentation review process.
- [ ] P12-T06 Define decision-record review process.
- [ ] P12-T07 Define bug diagnosis process.
- [ ] P12-T08 Define codebase improvement process.
- [ ] P12-T09 Define spec drift detection.
- [ ] P12-T10 Define model/domain drift detection.
- [ ] P12-T11 Define design-system drift detection.
- [ ] P12-T12 Define testing/quality drift detection.
- [ ] P12-T13 Define stakeholder feedback loop.
- [ ] P12-T14 Define how learnings are captured.
- [ ] P12-T15 Define how repeated mistakes are prevented.
- [ ] P12-T16 Define how task-list changes are proposed.
- [ ] P12-T17 Define how new phases/tasks are added.
- [ ] P12-T18 Define how obsolete tasks are retired.
- [ ] P12-T19 Define how assistant/Codex behavior is audited.
- [ ] P12-T20 Define how to recover if the process becomes too heavy.
- [ ] P12-T21 Define completion criteria for maintenance loop setup.
- [ ] P12-T22 Define what marks the whole meta-system setup as complete.

## Completion Criteria

P12 is complete only when:

- Maintenance cadence is approved.
- Drift-control method is approved.
- Learning loop is approved.
- Full setup completion criteria are approved.

## Output

Approved long-term maintenance and learning loop.

---

# Current Position

Current Phase: P0 — Working Rules Between Shubham and Assistant  
Current Task: P0-T13  
Next Action: Shubham and assistant should approve that P0 is a standing protocol and that this task list must be read or referenced before every setup-related response.

# Global Completion Criteria

The Codex setup meta-system is complete only when:

- P0 through P12 are completed or explicitly deferred.
- Every approved phase output has been recorded.
- Future artifacts have been created only when approved in the relevant phase.
- Codex has a clear operating system for discovery, specification, architecture decisions, design-system governance, issue slicing, implementation, review, and maintenance.
- Shubham has accepted the final setup state.

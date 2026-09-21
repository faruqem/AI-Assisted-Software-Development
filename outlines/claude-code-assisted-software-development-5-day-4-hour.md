---
ai_generated: true
model: "anthropic/claude-3.5-sonnet@2024-10-22"
operator: "johnmillerATcodemag-com"
chat_id: "7fd55dfd-5561-48eb-a1a4-304482ce4a13"
prompt: |
  create new versions of the outlines. instead of 6 hours of instruction, use 4 hours
started: "2026-09-17T10:02:40Z"
ended: "2026-09-17T10:47:00Z"
task_durations:
  - task: "four-hour course comparison"
    duration: "00:02:00"
  - task: "four-hour outline authoring"
    duration: "00:02:00"
total_duration: "00:04:00"
ai_log: "ai-logs/2026/09/17/7fd55dfd-5561-48eb-a1a4-304482ce4a13/conversation.md"
source: "johnmillerATcodemag-com"
---

# Claude Code Assisted Software Development: 5-Day Course Outline (4 Hours Per Day)

## Course Overview

This five-day instructor-led course gives software professionals the time to develop durable Claude Code practices instead of only learning the core interaction model. It combines live demonstrations, guided labs, peer review, and a cumulative project in a shared sample repository. The additional two days deepen work on codebase analysis, architecture, MCP integrations, agent orchestration, automation, security, and team adoption.

**Audience:** Developers, testers, technical leads, architects, and engineering managers who are comfortable with Git and at least one programming language.

**Format:** Five four-hour instructional days of short lectures, live demonstrations, guided labs, pair review, and a cumulative capstone. Breaks and lunch are additional.

**Prerequisites:** A Claude Code-enabled development environment, Git access, a supported terminal, and a local clone of the course repository.

## Comparison Notation

- **[Same]**: Covers the same learning objective as the three-day course, with normal five-day pacing.
- **[Expanded]**: Retains a three-day topic but adds depth, practice, or a broader application.
- **[Moved]**: Retains a three-day topic, but places it on a different day in the five-day sequence.
- **[New]**: Introduced only in the five-day course.
- **[Removed]**: A three-day topic that is not included in the five-day course.

No topics from the three-day course are removed. Day 1 remains the shared foundation, so no Day 1 topics move. The three-day Day 2 topics on refactoring and the three-day Day 3 topics on review, pull requests, instructions, security, quality gates, provenance, the capstone, and course close move to Days 3-5, where the longer format gives them dedicated practice.

## Learning Outcomes

By the end of the course, attendees will be able to give Claude Code effective project context with `CLAUDE.md`, skills, and hooks; connect approved tools with MCP; orchestrate parallel agents; and automate tasks through the CLI and CI. They will be able to plan feature slices, write and evaluate tests, debug failures, review AI-assisted pull requests, create durable project guidance, and apply those practices to architecture, operational quality, and team-wide adoption.

---

## Day 1: Foundations for Effective Claude Code Collaboration (4 hours)

### [Same] Course Orientation and Responsible AI-Assisted Development (15 minutes)

Attendees establish a practical mental model for Claude Code as a supervised engineering collaborator. They learn its strengths and limits, where human accountability remains essential, and how to use it without substituting generated confidence for evidence about correctness, security, or design.

### [Same] Environment, Repository, and Tool Setup (20 minutes)

Attendees configure their working environment, clone the course repository, verify the development toolchain, and run the existing checks. They learn why a known-good baseline, clean Git status, available test commands, and documented local setup are prerequisites for dependable AI-assisted work.

### [Expanded] Claude Code Interaction Model (25 minutes)

Attendees practice the central loop of task framing, focused exploration, small edits, review, and validation. Compared with the three-day course, they also compare exploratory, planning, and implementation interactions, learning how to pause the tool at the right points to inspect assumptions before it produces a large change.

### [Expanded] Context Engineering, CLAUDE.md, and Memory (30 minutes)

Attendees learn to identify the smallest relevant set of files, tests, configuration, and conventions for a request. Compared with the three-day course's focused context selection, the five-day course adds practice with `CLAUDE.md`, auto memory, repository summaries, and recovery after a long task.

### [Expanded] Prompting, Skills, and Hooks for Reliable Results (30 minutes)

Attendees turn vague requests into prompts that identify the outcome, scope, constraints, acceptance criteria, and expected validation. Compared with the three-day course's prompt patterns, the five-day course packages repeatable workflows as skills and adds hooks that run trusted commands before or after Claude Code actions.

### [Expanded] Lab: Explore and Improve a Small Feature (85 minutes)

Attendees investigate a contained feature, identify its behavior and tests, and deliver a small improvement. Compared with the three-day lab, the five-day version repeats the exercise with deliberately incomplete context so attendees practice asking for evidence and making their own context plan before editing.

### [Same] Day 1 Checkpoint (35 minutes)

Attendees review a peer's work against the prompt, supplied context, edit scope, and validation evidence. They leave with a tested change and a reusable collaboration checklist that establishes the discipline used throughout the rest of the course.

---

## Day 2: Requirements, Testing, and Safe Implementation (4 hours)

### [Expanded] Requirements to Vertical Slices (30 minutes)

Attendees translate a feature request into small, independently valuable slices with explicit business rules, acceptance criteria, and technical boundaries. Compared with the three-day introduction, the five-day course adds alternative slice-boundary analysis and risk-first sequencing before the team invests in supporting infrastructure.

### [Expanded] Test-Assisted and Test-First Development (30 minutes)

Attendees use Claude Code to propose test cases, generate test scaffolding, and improve regression coverage while retaining responsibility for testing the intended behavior. Compared with the three-day treatment, the five-day course adds test doubles, boundary conditions, negative paths, mutation-resistant assertions, and ways to spot tests that merely mirror the implementation.

### [Expanded] Implementing Features with Parallel Agents (30 minutes)

Attendees implement a vertical slice from an agreed plan while following existing project patterns. Compared with the three-day implementation workflow, the five-day course adds delegation of independent research or review work to parallel agents with explicit boundaries and integration review.

### [Expanded] Evidence-Driven Debugging (30 minutes)

Attendees debug from concrete observations such as stack traces, logs, failing tests, and reproducible behavior. Compared with the three-day debugging workflow, the five-day course adds competing hypotheses, low-cost discriminating checks, and distinguishing symptom-level patches from verified root-cause repairs.

### [Expanded] MCP, Dependencies, and Configuration Awareness (20 minutes)

Attendees configure and evaluate MCP servers that connect Claude Code to approved external systems, then treat dependency and configuration changes as deliberate engineering decisions. Compared with the three-day dependency module, the five-day course adds MCP server setup plus explicit review of tool permissions and data exposure.

### [Expanded] Lab: Deliver a Tested Feature Slice (70 minutes)

Attendees implement a complete feature slice with acceptance criteria, tests, implementation, error handling, and local validation. Compared with the three-day lab, the five-day version also requires a concise technical decision record explaining the chosen approach, rejected alternatives, and delivery evidence.

### [Same] Day 2 Checkpoint (30 minutes)

Attendees conduct a peer review using a checklist for scope, behavior, testing, error handling, dependencies, and maintainability. They learn to use Claude Code to surface review questions while keeping human reviewers responsible for approval.

---

## Day 3: Working Effectively in Brownfield Codebases (4 hours)

### [New] Codebase Archaeology with Claude Code (40 minutes)

Attendees learn to explore an unfamiliar or legacy repository without treating AI-generated summaries as authoritative. They build component maps, trace data and control flow, identify high-risk dependencies, and corroborate Claude Code's explanations against source code, runtime evidence, and existing tests.

### [New] Characterization Tests and Safety Nets (40 minutes)

Attendees learn to protect existing behavior before attempting a legacy change. They use Claude Code to identify observable behavior, propose characterization tests, and document uncertainty, then establish the regression tests, feature flags, logging, and rollback considerations that reduce the risk of changing poorly understood code.

### [Moved from Day 2 and Expanded] Refactoring Without Losing Behavior (40 minutes)

Attendees apply AI-assisted refactoring with a stable test baseline and a clear definition of preserved behavior. Compared with the three-day refactoring topic, the five-day course adds hands-on work extracting seams, isolating dependencies, removing duplication, and reviewing diffs for unintentional behavioral changes.

### [New] Technical Debt and Modernization Planning (30 minutes)

Attendees learn to use Claude Code to organize evidence about technical debt without confusing a generated backlog with a prioritized strategy. They identify hotspots, classify debt, estimate risk and payoff, compare incremental modernization paths, and build a small, actionable backlog tied to tests and measurable outcomes.

### [New] Lab: Make a Safe Change in Legacy Code (60 minutes)

Attendees choose a focused improvement in a legacy portion of the sample repository, first producing a component summary and test plan. They then implement a minimal vertical slice with regression coverage, a rollback plan, and a pull-request-ready explanation of the assumptions and remaining risks.

### [New] Day 3 Checkpoint (30 minutes)

Attendees review one another's brownfield changes, focusing on whether the safety net genuinely protects existing behavior and whether unknowns are documented clearly. This checkpoint ensures that the course treats legacy work as a distinct discipline rather than simply applying greenfield generation techniques to older code.

---

## Day 4: Architecture, Automation, and Operational Quality (4 hours)

### [New] Architecture Collaboration and Decision Records (30 minutes)

Attendees learn to use Claude Code to explore architectural alternatives without delegating system design to the tool. They practice framing quality attributes, constraints, and tradeoffs; generating diagrams or decision-record drafts; challenging recommendations with evidence; and recording the rationale needed for teammates to understand a decision later.

### [New] API, Data, and Integration Workflows (40 minutes)

Attendees apply Claude Code to the boundaries where application changes often fail: APIs, data models, migrations, background work, and third-party integrations. They learn to identify contracts, backward-compatibility risks, error behavior, and migration sequencing, then build validation plans that exercise the whole path rather than only isolated units.

### [Moved from Day 3 and Expanded] CLI, Quality Gates, and Continuous Integration Automation (40 minutes)

Attendees use the Claude Code CLI for non-interactive, scriptable tasks and connect local checks to automated quality gates including tests, linters, type checks, dependency scans, and build or deployment validation. Compared with the three-day quality-gate module, the five-day course adds safe `claude -p` patterns and pipeline diagnosis before producing the smallest evidence-based correction.

### [New] Observability and Production Readiness (30 minutes)

Attendees learn to make AI-assisted changes supportable after deployment. They examine meaningful logging, metrics, traces, health checks, alerts, feature flags, and rollback criteria, then use Claude Code to review whether a feature's operational signals and failure modes are sufficient for a safe release.

### [New] Lab: Design and Validate an Integrated Change (80 minutes)

Attendees plan and implement an integration-oriented change such as an API endpoint plus persistent state or an external service adapter. The lab requires contract tests, failure handling, observability considerations, and an automated quality-gate run, producing evidence appropriate for a change that crosses more than one code boundary.

### [New] Day 4 Checkpoint (20 minutes)

Attendees conduct an architecture and operations review of the lab changes. They evaluate whether the implementation respects system boundaries, protects compatibility, exposes useful diagnostics, and has a credible rollout and rollback path.

---

## Day 5: Team Adoption, Governance, and Capstone Delivery (4 hours)

### [Moved from Day 3 and Expanded] AI-Assisted Code Review and Pull Request Workflows (30 minutes)

Attendees review Claude Code-assisted changes with the same standards applied to any contribution: correctness, security, maintainability, performance, test coverage, and scope. Compared with the three-day course, they practice writing review comments, responding to feedback with focused follow-up changes, and preparing pull requests that state intent, risk, validation, and rollout notes clearly.

### [Moved from Day 3 and Expanded] Project Instructions and Reusable Prompts (40 minutes)

Attendees encode durable team knowledge in repository instructions and reusable prompts, including architecture boundaries, commands, coding conventions, prohibited actions, and expected validation. Compared with the three-day course, the five-day version adds an instruction-set review for ambiguity or conflict and a lightweight maintenance process.

### [Moved from Day 3 and Expanded] Security, Privacy, Intellectual Property, and Provenance (40 minutes)

Attendees apply organizational guardrails for secrets, sensitive code, customer data, dependency supply-chain risk, license obligations, and auditability. Compared with the three-day coverage, the five-day course adds a governance exercise defining required records for an AI-assisted change and escalation thresholds.

### [New] Team Operating Model and Adoption Strategy (30 minutes)

Attendees learn how to introduce Claude Code practices across a team without imposing a single workflow on every task. They identify suitable pilot work, define measures of success, establish review and escalation expectations, select training needs, and build an adoption plan that prioritizes reliability, learning, and developer effectiveness over raw output volume.

### [Moved from Day 3 and Expanded] Capstone Lab: From Requirement to PR-Ready Change (80 minutes)

Attendees complete an end-to-end change using the entire course workflow: investigate the repository, refine requirements, select a vertical slice, create tests, implement, validate, review, document decisions, and prepare a pull request. Compared with the three-day capstone, the five-day version adds peer review, an operations or security consideration, and a brief team-guidance artifact.

### [Moved from Day 3 and Expanded] Course Close and Next Steps (20 minutes)

Attendees synthesize the practices that make Claude Code valuable over time: explicit context, bounded work, evidence-driven checks, human review, durable guidance, and continuous improvement. Compared with the three-day close, the five-day course adds a team adoption plan and criteria for deciding which advanced practices to introduce first.

---

## Suggested Daily Schedule

| Time        | Activity                                           |
| ----------- | -------------------------------------------------- |
| 09:00-10:30 | Concept lesson and live demonstration              |
| 10:45-12:00 | Guided practice or focused lab                     |
| 13:00-14:30 | Feature implementation, analysis, or debugging lab |
| 14:45-16:00 | Review, discussion, and applied exercise           |
| 16:00-16:30 | Daily checkpoint and questions                     |

Each day includes four hours of instruction. Schedule a 15-minute break between sessions; lunch is outside the instructional schedule.

## Course Deliverables

- A configured local workspace with a verified project baseline.
- A small, tested improvement and collaboration checklist from Day 1.
- A tested feature slice with a decision record from Day 2.
- A legacy-code component summary, safety-net tests, and low-risk improvement from Day 3.
- An integrated change with quality-gate and production-readiness evidence from Day 4.
- A PR-ready capstone change, reusable team guidance, and AI-assisted development adoption plan from Day 5.

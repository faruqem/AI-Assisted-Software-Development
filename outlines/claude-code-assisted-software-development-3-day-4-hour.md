---
ai_generated: true
model: "anthropic/claude-3.5-sonnet@2024-10-22"
operator: "johnmillerATcodemag-com"
chat_id: "7fd55dfd-5561-48eb-a1a4-304482ce4a13"
prompt: |
  create new versions of the outlines. instead of 6 hours of instruction, use 4 hours
started: "2026-09-17T09:42:48Z"
ended: "2026-09-17T10:47:00Z"
task_durations:
  - task: "four-hour course adaptation"
    duration: "00:02:00"
  - task: "four-hour outline authoring"
    duration: "00:02:00"
total_duration: "00:04:00"
ai_log: "ai-logs/2026/09/17/7fd55dfd-5561-48eb-a1a4-304482ce4a13/conversation.md"
source: "johnmillerATcodemag-com"
---

# Claude Code Assisted Software Development: 3-Day Course Outline (4 Hours Per Day)

## Course Overview

This instructor-led course teaches software professionals to use Claude Code as a capable but supervised engineering collaborator. Attendees learn a repeatable workflow for exploring code, establishing persistent project guidance, translating requirements into small changes, validating generated work, and delivering changes through normal team practices. The course uses a shared sample repository so each technique produces a concrete, reviewable artifact.

**Audience:** Developers, testers, technical leads, architects, and engineering managers who are comfortable with Git and at least one programming language.

**Format:** Three four-hour instructional days of short lectures, live demonstrations, guided labs, pair review, and a cumulative capstone. Breaks and lunch are additional.

**Prerequisites:** A Claude Code-enabled development environment, Git access, a supported terminal, and a local clone of the course repository.

## Learning Outcomes

By the end of the course, attendees will be able to establish useful project context with `CLAUDE.md`, skills, and hooks; connect approved external tools through MCP; use parallel agents appropriately; and automate Claude Code through the CLI and CI. They will be able to turn a requirement into a tested vertical slice, diagnose failures with evidence, review AI-assisted changes for quality and security, and create reusable team guidance that makes those practices repeatable.

---

## Day 1: Collaborating Effectively with Claude Code (4 hours)

### Course Orientation and Responsible AI-Assisted Development (15 minutes)

Attendees establish a practical mental model for Claude Code: it can accelerate investigation and implementation, but it does not replace engineering judgment or accountability. They learn where AI assistance is strongest, where it can be unreliable, and how to keep humans responsible for architecture, security, correctness, and the final decision to merge a change.

### Environment, Repository, and Tool Setup (20 minutes)

Attendees prepare a consistent working environment by configuring access, cloning the course repository, checking the project toolchain, and confirming the available test commands. They learn why a working baseline matters before requesting any change, and how repository state, Git status, dependencies, and local instructions affect the quality and safety of Claude Code's work.

### Claude Code Interaction Model (25 minutes)

Attendees learn the core interaction loop: give a clear task, provide the relevant context, inspect the proposed work, and validate the result. They practice directing Claude Code to explain code, search for behavior, propose an approach, modify a limited surface, and report what it changed, building an interaction style that is collaborative rather than a one-shot request for code.

### Context Engineering and Persistent Project Guidance (30 minutes)

Attendees learn to provide the smallest useful context for a task without flooding the conversation with unrelated files. They identify the owning module, relevant tests, configuration, conventions, and dependencies, then use `CLAUDE.md` and Claude Code memory appropriately to preserve durable project guidance across sessions.

### Prompting, Skills, and Hooks for Reliable Results (30 minutes)

Attendees learn prompt patterns for investigation, planning, implementation, review, and debugging. They turn vague requests into prompts with a goal, scope, constraints, acceptance criteria, and requested validation, then package repeatable work as skills and add hooks that automatically run trusted formatting or validation commands.

### Lab: Explore and Improve a Small Feature (85 minutes)

Attendees use Claude Code to investigate a contained feature in the sample application, identify the behavior and its tests, and implement one small improvement. The lab reinforces a disciplined loop of reading before editing, reviewing the diff, running a narrow validation command, and recording what was learned from the result.

### Day 1 Checkpoint (35 minutes)

Attendees review a peer's change and discuss whether the prompt, context, edit scope, and validation evidence are sufficient for confidence. They leave the day with a small, tested change and a reusable checklist for interacting with Claude Code safely in an existing repository.

---

## Day 2: Building, Testing, and Debugging with AI Assistance (4 hours)

### Requirements to Vertical Slices (20 minutes)

Attendees learn to translate a feature request into independently valuable, testable slices that cross the necessary layers without turning into a large speculative implementation. They practice identifying user outcomes, business rules, acceptance criteria, boundaries, and dependencies, then ask Claude Code to help plan a sequence of changes that can be implemented and verified incrementally.

### Test-Assisted and Test-First Development (30 minutes)

Attendees learn how Claude Code can help write and improve tests while the developer remains responsible for testing the intended behavior rather than the implementation's current shape. They practice asking for missing cases, edge conditions, and regression tests; distinguishing useful tests from superficial coverage; and using a failing test to make the intended behavior concrete before implementation.

### Implementing Features with Parallel Agents (30 minutes)

Attendees use Claude Code to implement a vertical slice from an agreed plan, keeping changes bounded and observing the codebase's existing patterns. They learn when to delegate independent investigations to parallel agents, define a clear task boundary for each, and review the returned work before integrating it.

### Evidence-Driven Debugging (30 minutes)

Attendees learn to use Claude Code as a debugging partner that forms and tests hypotheses instead of guessing at fixes. They work from stack traces, logs, failing tests, and observed behavior; ask the tool to identify the controlling path; and use the cheapest discriminating check to confirm or refute an explanation before changing code.

### Refactoring Without Losing Behavior (20 minutes)

Attendees learn how to ask Claude Code to improve readability, remove duplication, and make localized design changes without accidentally mixing refactoring with feature behavior changes. They practice establishing a test baseline, choosing a narrow refactoring target, reviewing semantic changes carefully, and using incremental commits or diffs to retain a clear rollback path.

### MCP, Dependencies, and Configuration Awareness (20 minutes)

Attendees learn to connect Claude Code to approved external systems through MCP servers and to treat dependency and configuration changes as engineering decisions. They examine tool permissions, data exposure, compatibility, vulnerability exposure, lockfiles, environment variables, and necessary validation.

### Lab: Deliver a Tested Feature Slice (60 minutes)

Attendees implement a feature slice in the sample application, beginning with acceptance criteria and tests, then progressing through implementation, error handling, and validation. The deliverable is a reviewable branch containing the change, automated tests, a concise explanation of decisions, and evidence that the requested behavior works.

### Day 2 Checkpoint (30 minutes)

Attendees conduct a short peer review using a quality checklist that covers scope, behavior, tests, error handling, dependencies, and maintainability. They learn to use Claude Code to surface questions for a reviewer while avoiding the mistake of treating an AI-generated review as sufficient approval.

---

## Day 3: Team Workflows, Governance, and Delivery (4 hours)

### AI-Assisted Code Review (30 minutes)

Attendees learn to review Claude Code-assisted changes with the same rigor used for any other contribution. They practice looking for functional regressions, missing tests, unsafe assumptions, performance concerns, security risks, and accidental scope expansion, and learn how to use the tool to explain unfamiliar diffs without outsourcing the review decision.

### Git and Pull Request Workflows (30 minutes)

Attendees apply Claude Code within normal collaborative delivery practices: creating a focused branch, writing meaningful commits, preparing a pull request description, responding to review feedback, and maintaining a clean change history. They learn which information belongs in a pull request so teammates can evaluate the goal, risk, testing, and rollout implications quickly.

### Project Instructions and Reusable Prompts (30 minutes)

Attendees learn to encode durable team knowledge in repository instructions and reusable prompt files. They practice capturing technology choices, architectural boundaries, testing commands, coding conventions, prohibited actions, and review expectations so Claude Code starts with relevant guardrails instead of repeatedly rediscovering them from individual prompts.

### Security, Privacy, and Intellectual Property (30 minutes)

Attendees learn how to work safely with AI-assisted tools in organizational environments. Topics include avoiding secrets in prompts and logs, protecting sensitive code and customer data, checking dependency and supply-chain risk, respecting licensing obligations, understanding organizational policy, and escalating uncertainty instead of asking Claude Code to make compliance decisions.

### CLI, Quality Gates, and Continuous Integration Automation (30 minutes)

Attendees learn to use the Claude Code CLI for non-interactive, scriptable tasks and connect local validation with automated quality gates. They examine safe `claude -p` patterns, tests, linters, type checks, dependency scans, and CI pipeline output, then prepare narrow, evidence-based fixes.

### Provenance, Documentation, and Knowledge Transfer (30 minutes)

Attendees learn to make AI-assisted work understandable to future maintainers by documenting meaningful decisions, limitations, validation evidence, and operating assumptions. They discuss appropriate provenance records for regulated or high-assurance work and practice using Claude Code to improve documentation while verifying that it accurately reflects the implemented system.

### Capstone Lab: From Requirement to PR-Ready Change (40 minutes)

Attendees complete a small end-to-end change using the workflow developed over the course: inspect the repository, refine requirements, plan a vertical slice, add or improve tests, implement the change, validate locally, review the diff, and prepare a pull request. The capstone demonstrates that Claude Code is most effective when it is integrated into deliberate engineering practices rather than used as an unreviewed code generator.

### Course Close and Next Steps (20 minutes)

Attendees consolidate the habits that transfer back to their teams: small scoped tasks, explicit context, evidence-based validation, human review, and reusable guidance. They leave with a personal adoption plan, a set of prompt patterns and checklists, and a clear view of which next improvements, such as team instructions or CI checks, will make Claude Code use more reliable at scale.

---

## Suggested Daily Schedule

| Time        | Activity                                 |
| ----------- | ---------------------------------------- |
| 09:00-10:30 | Concept lesson and live demonstration    |
| 10:45-12:00 | Guided practice or focused lab           |
| 13:00-14:30 | Feature implementation or debugging lab  |
| 14:45-16:00 | Review, discussion, and applied exercise |
| 16:00-16:30 | Daily checkpoint and questions           |

Each day includes four hours of instruction. Schedule a 15-minute break between sessions; lunch is outside the instructional schedule.

## Course Deliverables

- A configured local workspace and verified project baseline.
- A small, tested improvement created on Day 1.
- A feature branch containing a tested vertical slice from Day 2.
- Reusable Claude Code prompts or repository instructions for a team workflow.
- A PR-ready capstone change with validation evidence and a concise risk summary.

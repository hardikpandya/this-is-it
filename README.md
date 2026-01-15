# Agent-Native Project Intelligence

*Planning and orchestration for the agentic era*

---

## The Problem

Jira and Linear were designed for human coordination. The unit of work in an agentic world is fundamentally different.

Today, a ticket that says "Add dark mode to settings" works because a human developer uses judgment, context, and tacit knowledge to figure out the actual work. They look at the codebase, understand the design system, check how other settings work, make dozens of micro-decisions.

Agents can't do that. They need explicit, grounded context. The gap between what a PM writes in a PRD and what an agent needs to execute well is enormous.

---

## The Three-Layer Context Gap

**Org-level:** The messy swarm of docs, Slack threads, design decisions, past incidents, architectural constraints, tribal knowledge.

**Project-level:** What we're building, why, the scope, dependencies, and constraints.

**Task-level:** What exact change needs to happen, in what files, respecting what patterns, with what acceptance criteria.

Right now, all of this lives in human heads. We do the translation layer between fuzzy intent and concrete execution. Agents need that translation made explicit.

---

## The Product

**A context compiler for agentic work.**

**Ingest:** Connect to the org's messy context—codebase, docs, Slack, design files.

**Articulate:** Help humans express intent through conversation, not forms. Surface relevant context, identify ambiguities, ask clarifying questions.

**Generate:** Produce agent-executable plans grounded in actual system state—accurate plans.md files that agents can run against.

**Sync:** Maintain bidirectional updates as work progresses and context shifts.

---

## Slack as the Primary Interface

Most tools assume people will come to them. That's friction, and friction means the system drifts from reality. Slack is where attention already lives.

**Push:** Daily standups synthesized from actual agent activity. Proactive alerts when plans need human judgment. Completion notifications with context.

**Pull:** "@agent what's the status?" "@agent update the plan—we're descoping mobile." "@agent add this context." The agent is a team member that lives in Slack.

---

## Why This Doesn't Exist

The pieces exist in isolation. Glean and Dashworks do enterprise search but not planning. Cursor and Claude Code need plans fed to them. Linear's Slack integration is notifications, not conversation. Dust.tt is closest but positioned as general-purpose assistants.

Nobody is doing the full loop: ingest org context → articulate intent → generate agent-ready plans → sync as work happens → live natively in Slack.

---

## Timing

Until recently, agents weren't good enough for this to matter. The capability curve just crossed the threshold where this problem becomes urgent. Engineering orgs are actively figuring out how to use Cursor and Claude Code effectively.

Linear and Jira are web-app-first with Slack bolted on. Building Slack-first with the web app as support creates a fundamentally different product with a defensible position.

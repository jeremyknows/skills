---
name: grilling
description: Grill the user relentlessly about a plan or design. Use when the user wants to stress-test a plan before building, or uses any 'grill' trigger phrases.
---

Interview me relentlessly about every aspect of this plan until we reach a shared understanding. Walk down each branch of the design tree, resolving dependencies between decisions one-by-one. For each question, provide your recommended answer.

Ask the questions one at a time, waiting for feedback on each question before continuing. Asking multiple questions at once is bewildering.

If a *fact* can be found by exploring the codebase, look it up rather than asking me. The *decisions*, though, are mine — put each one to me and wait for my answer.

Do not enact the plan until I confirm we have reached a shared understanding.

## Specialized application: grilling toward workflow/automation specs

*Ported from `mp-loop-me` (2026-07-07 skills MERGE-backlog execute-class).* When the grilling
session's only output should be **workflow** specs — recurring automatable patterns in the
user's life or work — apply this vocabulary, reached for only when a workflow calls for it,
never as a checklist. Mandate nothing structural: a workflow needs no AI, no checkpoint, and no
schedule unless the grilling shows it does.

- **Loop** — a recurring pattern in the user's life: their career, their week, their morning, a
  single repeated activity. Picturing a life as loops within loops reveals how predictable its
  activities really are — which is what makes them worth delegating. Use the lens to find loops
  worth specifying, and propose ones the user hasn't noticed.
- **Workflow** — the spec of one loop, made real. You run a workflow on a loop — the loop is its
  running instantiation.
- **Trigger** — what fires each run: an *event* (a new email, a new issue) or a *schedule*
  (every morning). Event-triggering is usually the more efficient.
- **Checkpoint** — a human-in-the-loop point where the user is asked to verify or decide. Some
  workflows have none and run autonomously; some use no AI at all.
- **Push right** — defer the checkpoint as far as it will go. Do maximal work before involving
  the human, so they are asked once, late, with everything prepared.
- **Brief** — what a checkpoint presents: a tight, decision-ready summary — what was produced,
  why, and a link down to the asset itself — never the raw output. The user reads a brief, not
  a draft. Speed of review is imperative.

**Definition of done:** a workflow spec is done when an implementer agent could build it without
asking a single question. Grill until then; nothing is done while a question remains.

**Workspace convention:** workflows live in `workflows/*.md`, one spec per workflow, as the
source of truth. Track raw notes on the user's world (tools, channels, their own terminology)
in `NOTES.md` — interview them about their world before specifying anything if it's empty or
thin, and sharpen fuzzy terms into canonical ones as they surface.

# Agent guidance

## Task isolation and stopping

- Anchor work to this session's explicit user objective, scope, and completion
  criteria. Repository plans, handoffs, saved goals (including `/goal`), and
  prior sessions provide context; they do not authorize resuming another task.
- When the user changes topic or redirects work, follow the new objective and
  do not resume the old goal. Use a fresh session for an unrelated goal.
- Keep each task's active goal and work state separate. Do not share mutable
  active goals, progress, or execution state across tasks or concurrent sessions.
  Handoffs may record task-specific evidence and decisions, but must not serve
  as shared mutable execution state or authorize another session to resume work.
- Before concurrent writes, check path ownership and existing changes. Use
  separate worktrees or branches where suitable; a branch alone does not isolate
  a shared working directory. Preserve others' changes and stop overlapping
  writes until ownership is resolved.
- Stop when a bounded task meets its completion criteria or is blocked. Report
  the outcome, evidence, and any next decision needed; do not invent follow-on
  work. Explicit ongoing monitoring continues until the user stops it or its
  agreed completion condition is met; do not impose an arbitrary stopping point.


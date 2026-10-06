# Project-Readiness Mode

Open this when the learner is joining or starting a real project.

## Add these to the course

- how to navigate the codebase,
- an architecture map,
- the request and data flow,
- how to build, run and debug locally,
- configuration and environments,
- the database and data model,
- tests,
- logging and observability,
- deployment,
- the common operational failures in this kind of system.

## Approach

Prefer:
> "Trace one real request end to end."

over:
> "Read every folder in the repository."

Pick one important user action (for example "place an order" or "book an appointment"). Follow it from the entry point through each layer to the database and back. Name each concept as it appears. This gives the learner a map they can hang everything else on.

If you can read the repository yourself (coding agents), do the trace with real file paths and code. If you cannot, ask the learner to share the key files or a folder listing, or give them a step-by-step guide to trace it themselves and report back.

## Deliverables

- a one-page architecture map of the actual project,
- a "first week" checklist: run it, debug it, make a small change, run the tests, read the logs,
- a glossary of project-specific terms,
- a list of open questions to ask the team.

# Practicals and Labs

Open this when designing or running any hands-on exercise.

## Pick the lab style by what the session can do

**A. You can read the repo, edit code and run commands** (for example Claude Code or Codex).
You are both teacher and hands-on agent. Skip the hand-off brief:
1. Explain what the lab will prove, in one or two sentences.
2. Make the change, or better, have the learner make it and you review it.
3. Run it and show the real output (logs, test results, errors).
4. Connect the output back to the concept: "See the proxy class name in this log? That is the transaction wrapper we talked about."
5. Where useful, break it on purpose, run it again, and ask the learner to explain what changed.

Keep lessons short in this setting and let the real code do the teaching. Ask before touching anything outside a lab folder or branch. Do not change the learner's real project code without their clear agreement.

**B. You can create files but not run the learner's project** (for example Claude Cowork or ChatGPT Work).
Create the lab files, starter code and a lab brief in the working folder. The learner runs it and reports back. You review.

**C. Chat only.**
Write a clear lab brief the learner can follow on their own machine. Ask them to paste back the output or the error. Review what they bring back.

**D. A separate coding agent does the work, and you are the teacher.**
Some learners use one assistant to teach and a different coding agent to write code. Split the roles:
- **Teacher (you):** teach the concepts, run the course, design the practical, review the results, tie code back to theory, run interview drills.
- **Coding agent:** create and edit code, run builds and tests, inspect the repo, produce real evidence.
Write the brief below so the learner can hand it straight to the other agent.

## Lab brief format (for B, C and D)

Every brief includes:
- **Objective:** what the lab proves
- **Where:** the repository or folder path
- **Files or areas to touch**
- **What to build**
- **What not to over-engineer**
- **Done when:** acceptance criteria
- **Commands or tests to run**
- **What to bring back:** logs, output, screenshots, observations
- **Deliberate failure** to try, if useful

### Example

> **Spring `@Transactional` experiment**
> - One method saves a Post and an Audit entry.
> - Throw an unchecked exception on purpose. Prove that both rows roll back.
> - Then call the transactional method from inside the same class (self-invocation). Observe that the rollback no longer happens.
> - Bring back: test output, logs, and the proxy class name.

## Reviewing the learner's work

Check that it meets the "done when" criteria. Then ask one "why" question about the result. Point out one thing that would matter in production. Add anything they struggled with to the course state's weak areas.

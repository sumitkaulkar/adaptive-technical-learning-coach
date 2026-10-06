# Intake Question Bank

Use this for **standard** intake (Section 5.3 of SKILL.md). Pick only the questions the learner has not already answered. Ask at most 4 per message, over at most 2 rounds. Each question comes with example answers so the learner can see the range of choices.

For urgent intake, do not use this list. Use the single-message format in SKILL.md Section 5.2.

---

## Q1. What do you want to learn?
Ask for the topic and any scope they already know.
> "What do you want to learn? For example: 'Spring Boot backend', 'Kubernetes for developers', 'Kafka architecture', or 'AI across the SDLC'."

## Q2. Why are you learning it?
> "Is this mainly for an interview, a current project, a presentation, or long-term mastery? The course changes a lot depending on the answer."

Other valid purposes: certification, architecture responsibility, team training, getting hands-on coding ready.

## Q3. How much time do you have?
Ask for total time, the deadline, time per day, and whether more time opens up later.
> Examples: "6 hours today before an interview", "1 hour a day for 3 weeks", "4 weekends", "basics by tomorrow, deeper once the project starts".

## Q4. What depth do you need?
Do not ask only "basic, intermediate or advanced". Explain the dimensions (listed in SKILL.md 5.3) and give a concrete example:

**Spring transactions**
- Conceptual: "`@Transactional` groups database operations into one transaction."
- Implementation: "Where to put the annotation, and what rollback looks like."
- Internals: "A Spring proxy wraps the method and opens and commits the transaction."
- Production: "Long transactions can use up database connections and hold locks."
- Interview: "Explain self-invocation and why the proxy boundary matters."

**Kafka**
- Conceptual: producer → topic → consumer.
- Production: partitions, consumer lag, retries and dead-letter queues, duplicates, idempotency, ordering.
- Architecture: why Kafka instead of a direct REST call.

## Q5. What do you already know?
Always asked through the Background block in SKILL.md Section 5.1: show what you found (or that you found nothing), then ask the learner to rate 3 to 6 prerequisites as know it well, partly, or new. The examples below are extra wording ideas.

Ask what they know, what they have used, what they only know by name, and what they find hard.
> "For Java you might say: OOP 4/5, collections 3/5, concurrency 1/5, Spring Boot 2/5."
> "For React: I know JavaScript but have never built a React app."
> "For Kubernetes: I deploy through CI/CD but don't understand pods or services."

## Q6. What role or seniority should the course aim at?
> Examples: junior developer, senior engineer, tech lead, architect, QA or SDET, a manager returning to hands-on work, a non-engineer who must discuss the topic credibly.

Explain why it matters: "A senior-level course covers failure modes, trade-offs and architecture even when we only briefly refresh the basics."

## Q7. How do you learn best?
Offer a few and allow combinations:
> simple language first, lots of analogies, code first, diagrams, theory then practice, project-based, Socratic questions, frequent mini-quizzes, interview drill after each module.

## Q8. What can you practise on?
> Examples: a local IDE, a repository, a coding agent, a browser or cloud lab, Docker, a database, or nothing at all.

If a coding agent is available, ask whether they want you to run the labs directly or to act as teacher while they (or another agent) do the coding. See `references/practicals.md`.

## Q9. How should the lessons be delivered? (always ask; never infer)
Two parts, asked together:
> "How do you want the lessons delivered? In chat only, a separate document per module, or one combined document? If documents: Word, PDF, or something else?"

Other extras the learner may want on top: cheat sheets, lab briefs, interview Q&A, a final revision guide, slides, diagrams, flashcards.

See SKILL.md Section 5.4 for the rules (record it, stick to it, say so if a file type is not possible here, name files `Module-01-<title>.docx`).

## Q10. Any source material that should drive the course?
> Examples: a job description, an internal architecture doc, the project codebase, a syllabus, a list of interview topics, product docs, company standards.

If provided, treat it as the primary source. In the lessons, mark what came from their material versus what you added as background.

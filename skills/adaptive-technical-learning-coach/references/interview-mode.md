# Interview Mode

Open this when interview preparation is part of the goal. Run an **Interview Track** alongside the main lessons.

## For each important topic, prepare

- a **30-second answer**,
- a deeper **2-minute answer**,
- the **likely cross-question**,
- a **production example** (from the running system, clearly marked as an example, not the learner's own history),
- the **common trap** that catches candidates.

### Example

**Question:** JPA vs Hibernate vs Spring Data JPA?

**30-second answer:**
> "JPA is the persistence specification, Hibernate is a common implementation of it, and Spring Data JPA is a repository layer on top that cuts boilerplate."

**Cross-question:**
> "If Spring Data generates the repository, where does the SQL actually come from?"

**Expected reasoning:**
> Spring Data → JPA EntityManager → Hibernate → JDBC → database.

**Common trap:** saying Spring Data JPA "replaces" Hibernate.

## Senior roles

Also cover architecture trade-offs, incidents, scale, failure modes, observability, and "why not alternative X?"

## Honesty about experience

Help the learner describe what they know and have practised, accurately. Do not coach them to claim production experience they do not have. If they ask how to answer "have you used X in production?", help them give a strong, truthful answer: what they built or studied, what they understand about running it in production, and how they would approach it.

## Crash interview prep (for example, "Java and Spring Boot interview in 2 days")

In the single urgent intake message (SKILL.md 5.2), ask about total study hours, current level, seniority of the role, and any job description or known topics.

A typical plan:
- **P1:** Spring container and Boot, MVC request flow, persistence, transactions, security
- **P2:** caching, Kafka, observability, deployment (compact notes)
- **P3:** deep framework internals (deferred)

Style: short but understandable, one running project, code inside the lessons, cross-questions after each topic, and a final revision sheet.

## Mock interview

When time allows, finish with a mock round: ask 5 to 8 questions in order of likelihood, one at a time. Wait for each answer, then score it briefly (clear, partly right, or missing the point). Give the stronger version, and ask the natural follow-up an interviewer would ask.

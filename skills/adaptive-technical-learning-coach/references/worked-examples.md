# Worked Examples

Open this to see what good output looks like. These are patterns, not scripts. Adapt the wording to the learner.

---

## 1. Urgent course: first reply

**Learner:** "i have a call with my boss in 3 hrs, need to explain RAG and AI agents confidently. teach me"

**Good first reply (single message, then teach):**

> By the end of this, you'll be able to explain what RAG and AI agents are, when each one helps, where they go wrong, and handle your boss's likely follow-up questions.
>
> **Your background: please confirm.** I don't have anything saved about your AI background yet. Quick ratings (know it well / partly / new):
> 1. Using an LLM through chat or an API
> 2. Prompting basics
> 3. Embeddings and vector search
>
> I'll plan for "partly" on all three unless you say otherwise.
>
> **Plan (about 2.5 hours, leaving 30 minutes spare):**
> - P1, RAG: the problem it solves, the flow, where it fails (45 min)
> - P1, Agents: what makes something an agent, tools, the loop, where it fails (45 min)
> - P1, RAG vs agents vs fine-tuning, and when to use which (20 min)
> - Boss Q&A drill and a 2-minute version of each (30 min)
> - Deferred: vector database internals, evaluation frameworks, multi-agent designs
>
> I'll teach here in chat and give you a one-page revision sheet at the end. Want the lessons as a Word doc instead?
>
> Two quick questions, answer if you can:
> 1. Is your boss technical, or more business-focused?
> 2. Is this for a specific project or decision, or general understanding?
>
> Or just say go and I'll start with RAG.

Why it works: one message, a visible background check that counts as one of the 3 questions, 2 more questions that change the plan, a plan with time, deferred topics named, and teaching starts on the next reply.

---

## 2. Standard course: first reply

**Learner:** "Teach me context engineering properly over 4 weeks, about 1 hr a day. I know prompting basics and have called the model API from Python."

**Good first reply:**

> Good starting point. Calling the API from code means you already build prompts programmatically, which is the core of context engineering.
>
> **1. Your background: please confirm.** From what you said: Python, the model API and prompting basics. Rate each (know it well / partly / new):
> - Python and the model API: you said yes, still "know it well"?
> - Prompting techniques (few-shot, chain of thought)
> - Embeddings and retrieval
> - Tool use and function calling
> - Evaluating model output
>
> I can also check our past chats for what you've covered before. Want me to?
>
> **2. Why now?** Something to show at work, a project you're building, or general mastery?
>
> **3. Depth:** do you want to *explain* it well (concepts plus trade-offs), *build* with it (implementation), or both?
>
> **4. Delivery:** lessons in chat only, a separate document per module, or one combined document? If documents: Word, PDF, or something else?
>
> (I'll ask about your practice setup once we see the plan.)

Then, after the answers: a module plan with P1, P2 and P3, hours per module, the practical approach, the deliverables and the deferred topics. End with "Lock this plan, or change anything first?"

---

## 2b. Standard course, nothing found about the learner

**Learner:** "i want to learn spring boot"

**Good first reply (the Background block still appears):**

> Happy to. Let's size this to you.
>
> **1. Your background: please confirm.** I don't have anything saved about your Java or Spring background yet. Rate each (know it well / partly / new):
> - Core Java (classes, interfaces, exceptions)
> - Collections and generics
> - HTTP and REST basics
> - SQL and relational databases
> - Maven or Gradle
> - Spring or Spring Boot itself
>
> **2. Goal:** building apps for work, interview prep, or understanding the fundamentals?
>
> **3. Time:** how much per day, and is there a deadline?
>
> **4. Delivery:** chat only, a separate document per module, or one combined document? If documents: Word, PDF, or Markdown?
>
> Short answers are fine, for example "1: know, know, partly, partly, new, new".

Bad version: "No prior Spring Boot knowledge is assumed." It hides the check and never asks the learner to confirm anything.

---

## 3. Resume

**Learner:** "continue my kafka course"

**Good reply when the state is found:**

> Picking up where we left off. Goal: project readiness on Kafka by the 20th. Done: modules 1 to 3 (topics and partitions, producers, consumer groups). Weak spot to revisit: offset commits. Next up: module 4, retries and dead-letter queues.
>
> Quick warm-up on the weak spot first: if a consumer crashes after processing a message but before committing its offset, what happens when it restarts?...

(and the lesson continues in the same reply)

**Good reply when no state is found:**

> I can't find saved progress for this course. If you have the course state, paste or upload it. Otherwise, tell me in a line or two where you got to, and I'll pick up from there right away.

---

## 3b. Quality check-in and hand-off

**Inside the wrap-up of module 3:**

> That's module 3 done: consumer groups, rebalancing and offset commits. Your weak spot was commit timing, so I've added it to the revision list. Progress saved.
>
> Quick check before we move on: are my answers still sharp and consistent with what we covered earlier, or have you noticed me forgetting or repeating things?

**Learner:** "honestly you mixed up the retry example from module 2 just now"

> Good catch, thanks. That can happen in a long chat. Would you like to continue in a fresh window? Nothing gets lost, and I'll give you everything you need to pick up exactly here.

**Learner:** "yes"

> Here's your hand-off:
> 1. **Course state** (saved as course-state-kafka.md / printed below). Attach it in the new chat.
> 2. **Also attach** Module-03-Consumer-Groups.docx if you want to refer back to it.
> 3. **First message to type:** "Continue my Kafka course from module 4. Course state attached."
> 4. **We'll start with** a 2-minute warm-up on offset commits, then module 4, retries and dead-letter queues.

If the learner had said "all good", the reply would simply move on to module 4, with no further mention.

---

## 4. Quick question

**Learner:** "quick one, whats the difference between RAG and fine tuning?"

**Good reply:** a clear, complete answer using the teaching pattern in brief (problem, simple idea, example, when to use which, common mistake). End with one line:

> If you'd like to go deeper on either one, I can turn this into a short course around your goal and deadline.

Nothing more. No intake questions.

---

## 5. Deep course plan shape (for example, "Kubernetes over 6 weeks")

Modules: containers (prerequisite) → pods, deployments, services → configuration and secrets → networking and ingress → storage → probes and resources → scaling → security → observability → troubleshooting → deployment strategies → capstone.

Each module: lesson → discussion → practical → break and fix → review → scenario drill → course state saved.

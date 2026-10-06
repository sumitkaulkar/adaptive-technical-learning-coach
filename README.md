# Adaptive Technical Learning Coach

An AI skill that teaches any technical topic as a course built around **your goal, your deadline and what you already know**. It works in both **Claude** and **ChatGPT**.

Got a client call about FHIR in 3 hours? It gives you a tight briefing and the questions you'll likely face. Want to learn Kubernetes properly over 6 weeks? It builds a full course with labs, checks and a final project. Same skill, sized to the situation.

<!--
![First reply](docs/screenshots/first-reply.png)
![Lesson](docs/screenshots/lesson.png)
-->

## Why it's different

- **Sized to your time.** Short on time, it starts teaching by its second reply. Plenty of time, it plans a proper course first.
- **Starts from what you know.** It checks your background and asks you to rate the key prerequisites, so it won't reteach what you already know.
- **Short courses still make sense.** It cuts topics when time is short, not clarity. Every key idea gets a plain explanation, a real example, and the common mistake to avoid.
- **You choose the format.** Lessons in chat, one document per module, or one combined document, in Word, PDF or Markdown.
- **Pick up where you left off.** Progress is saved in a small course state file. Paste it into any new chat, on Claude or ChatGPT, and say "continue my course".
- **Honest about experience.** It helps you explain and build with confidence, without pretending a course equals years of production work.

## Try these prompts

```
I have a client call in 3 hours about FHIR. Teach me enough to talk confidently.
I have a Spring Boot interview in 2 days. Get me ready.
Teach me Kubernetes over 3 weeks, 1 hour a day.
I'm joining a React project next week. Get me project ready.
Explain RAG so I can present it to a client tomorrow.
Continue my Kafka course.  (with your course state file attached)
```

A quick one-off question ("what's the difference between REST and GraphQL?") just gets a direct answer, with an offer to go deeper.

If the skill doesn't start by itself, add "use the Adaptive Technical Learning Coach" to your prompt.

## Install

Download the latest files from the [Releases](../../releases) page, or from the [`dist/`](dist) folder.

### Claude (web, desktop, mobile) and Cowork
- **Desktop app:** double-click `adaptive-technical-learning-coach.skill` and send the "install this skill" message it opens with.
- **Web:** upload `adaptive-technical-learning-coach.zip` under **Customize > Skills**.

Skills on your Claude account also work in Cowork, and in Claude Code when you sign in with the same account. Custom skills need code execution turned on in settings.

### Claude Code
```
/plugin marketplace add sumitkaulkar/adaptive-technical-learning-coach
/plugin install adaptive-technical-learning-coach@adaptive-technical-learning-coach
```
Or copy `skills/adaptive-technical-learning-coach/` into `~/.claude/skills/`.

### ChatGPT (Chat and Work)
Upload `adaptive-technical-learning-coach.zip` from the **Skills** tab (under Plugins in the sidebar). Skills need a ChatGPT Business, Enterprise, Healthcare or Edu plan, and your admin may need to turn them on.

### Codex
Copy `skills/adaptive-technical-learning-coach/` into `~/.agents/skills/` (for you) or `.agents/skills/` in a repo (for your team). Restart Codex if it doesn't show up.

### Other agents
```
npx skills add sumitkaulkar/adaptive-technical-learning-coach
```

Menu names change often. If a step doesn't match what you see, check your platform's help page for "skills".

## How a course runs

1. **Background check.** It shows what it knows about you and asks you to rate the key prerequisites.
2. **A few questions.** At most 4 at a time (3 when you're in a hurry), including how you want the lessons delivered.
3. **A plan.** Topics ranked must-learn, useful, and later, with time for each. You approve it before it starts.
4. **Modules.** Each one has a lesson, discussion, a hands-on exercise, an understanding check and a review. Progress is saved after every module.
5. **Revision and a final project** that ties everything together.

On long courses, it asks at the end of each module whether its answers still feel sharp. If you say they're slipping, it offers a clean hand-off to a fresh chat. It never forces one.

## What's inside

```
skills/adaptive-technical-learning-coach/
├── SKILL.md                     core rules
├── COURSE_STATE_TEMPLATE.md     progress format, same on every platform
└── references/                  loaded only when needed
    ├── intake-question-bank.md
    ├── interview-mode.md
    ├── presentation-mode.md
    ├── project-readiness-mode.md
    ├── practicals.md
    └── worked-examples.md
```

It follows the open Agent Skills format (a folder with a `SKILL.md`), so it also works with other tools that support that format.

## Feedback

Found a bug or have an idea? Please open an [issue](../../issues). Screenshots of where it went wrong help a lot.

## License

MIT. See [LICENSE](LICENSE).

# Presentation and Client-Discussion Mode

Open this when the learner must explain the topic to a client, leadership, their boss or a team.

## What matters

The goal is to sound clear and credible under questions, not to know every detail. Focus on:
- a simple story (problem → approach → how it works → trade-offs → what we recommend),
- one main architecture picture,
- why each decision was made,
- the business effect,
- trade-offs, and when not to use it,
- the failure and scaling story,
- a demo flow, if there is a demo.

Leave out implementation detail unless it supports the message.

## What to produce

- a short story outline (often 5 slides or fewer),
- speaker notes in plain language,
- a **30-second** and a **2-minute** version of the core explanation,
- a simple diagram,
- the 5 to 10 **likely audience questions** with short, honest answers, including "I'd need to check that" for anything genuinely uncertain,
- demo checkpoints, if there is a demo,
- a quick rehearsal: the learner explains it back, and you play the audience and ask the hard questions.

## Example: "I need to explain RAG to a client in 3 hours"

Do not build a 20-module course. Instead cover:
1. the business problem (the model doesn't know the client's documents),
2. the simple RAG flow (find the relevant text, hand it to the model, answer from it),
3. indexing and query flow, at a whiteboard level,
4. quality and failure issues (wrong text retrieved, stale data, confident wrong answers),
5. security and data concerns (who can see which documents),
6. cost and latency,
7. when not to use RAG (small stable knowledge, or when fine-tuning or plain search fits better),
8. a 5-slide story,
9. likely client questions,
10. a 10-minute rehearsal.

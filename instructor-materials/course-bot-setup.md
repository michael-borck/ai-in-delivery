# Course-assistant chatbot: setup & config

The site-wide tutor / live-FAQ bot on the companion site (injected on every page
via `course-bot.html` → `_quarto.yml` `include-after-body`).

| | |
|---|---|
| AnythingLLM workspace | `ai-in-delivery-course` (chat.eduserver.au) |
| Embed UUID | `02e13977-3067-4888-89f7-69f15d77df40` (in `course-bot.html`) |
| Model | Haiku (AnythingLLM system default), sufficient for tutor/FAQ |
| Retrieval | `similarityThreshold: 0`, `topN: 6` (defaults 0.25 / 4 are too strict; they made the bot miss the schedule) |
| Chat mode | `chat` (uses retrieved docs **and** the model's own knowledge) |

## Knowledge (19 docs, student-facing only)
The 3 readings, the 5 site pages (`index/before/workshop/frameworks/team.qmd`),
the 4 initiative cards, the 3 sprint worksheets, `frameworks-overview.md` + the 2
framework handouts, and `content/course-agenda.md` (plain-prose schedule).
**Not** included: instructor materials, the document answer-key, or the deck's
speaker notes.

## Rebuild (when course material changes)
Stage those files into a folder, then:
```
botstash run <folder> --workspace ai-in-delivery-course --reset
```
`--reset` clears + re-uploads docs and **preserves** the system prompt and
retrieval settings (set separately via the API). After changing material, also
re-set the prompt/retrieval if needed (see below).

## Scope (what it will / won't answer)
- **Answers:** course content + logistics; and broader AI / AI-in-business /
  AI-delivery / AI-leadership questions (e.g. "what is an agent?", "is timeline
  estimation different?") from general knowledge, tying back to the course where
  it can. It's a *tutor*: it answers, then nudges critical thinking, and won't do
  a participant's workshop deliverable for them.
- **Declines:** anything unrelated to AI or the course (trivia, other subjects,
  personal advice, "why is the sky blue"), and NSFW/inappropriate content.

## Set the prompt + retrieval (API)
`POST /api/v1/workspace/ai-in-delivery-course/update` with
`{"openAiPrompt": "<the tutor/FAQ prompt>", "similarityThreshold": 0.0, "topN": 6}`.
The current prompt text is the "AI in Delivery course assistant … live FAQ" system
prompt (tutor stance + AI-FAQ scope + off-limits rules).

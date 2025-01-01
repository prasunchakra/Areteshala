# Areteshala

**A training ground for mastery.**

*Arete* (ἀρετή, Greek): excellence of character and ability; becoming the best version of yourself.
*Shala* (शाला, Sanskrit): a place of practice and learning, in the sense of a dojo rather than a lecture hall.

Areteshala is an edtech platform built on a simple belief: the world has enough lectures. What learners lack is a place to *practice* deliberately, to find out exactly where and how they fail, and to build the discipline to keep going. Areteshala owns that layer.

---

## Why this exists

Most learning platforms sell content: video libraries, question banks, courses with a percent-complete bar. Content is now abundant and nearly free. The hard, unsolved problems sit after the lecture ends:

- **Diagnosis.** Learners know they are "weak in rotational mechanics," not that they mishandle the sign of torque when the axis is off-center. Generic feedback does not change behaviour.
- **Retention.** Revision collapses under time pressure. Spaced retrieval is well understood in research and almost absent in serious exam prep.
- **Discipline and wellbeing.** Aspirants are anxious, isolated, and burn out. No platform treats sustainability and character as part of excellence.
- **Teaching as learning.** Explaining a concept to someone else is one of the most robust learning effects known, and no mainstream platform makes it a core mechanic.

Areteshala is deliberately **not** a coaching institute. Learners bring whatever content they already use (coaching lectures, standard textbooks, NCERT, online courses). Areteshala is the practice floor that sits alongside it.

---

## Core principles

1. **Practice first, explanation on demand.** No autoplay video as the primary mode. The default action is to attempt, then learn from the attempt.
2. **Diagnose the sub-skill, not the chapter.** Every wrong answer is tagged by *why* it was wrong: concept gap, calculation error, misreading, time pressure, carelessness.
3. **Respect forgetting.** Weak concepts are re-surfaced on a decaying schedule so revision is continuous, not a panic in the final weeks.
4. **The mentor asks, it does not tell.** The AI mentor works a stuck problem one question at a time, remembers the learner's error history, and refuses to spoon-feed.
5. **Learn by teaching.** Learners earn standing by explaining concepts to peers; explanations are graded by peers and AI.
6. **One honest metric.** Retention and demonstrated mastery over time, not streaks and badges.
7. **Arete is more than marks.** Focus, recovery, honest weekly review, and burnout awareness are part of the product, not an afterthought.

---

## Audiences and phasing

Areteshala starts narrow and expands outward. The engine (diagnosis, spaced practice, mentor, peer teaching) is shared across every phase; only content, tone, and pacing change.

| Phase | Audience | Notes |
|---|---|---|
| **1 (MVP)** | College and competitive-exam aspirants (JEE / NEET / UPSC / GATE and similar) | Outcome-driven, willing to pay, clearest need for diagnosis and revision. Wedge on **one exam** first. |
| 2 | K-12 school students (boards) | Same engine with a gentler tone and parent-facing progress; larger market, longer sales cycle. |
| 3 | Working professionals and upskillers | Tech, data, and business skills; global market; skills map replaces exam syllabus. |
| 4 | Lifelong and general learners | Brand-led; most freedom to lean into the *Arete* layer (thinking skills, intellectual honesty, focus). |

There is no hurry to reach later phases. Each one is opened only when the previous one shows real retention.

---

## MVP scope (Phase 1)

Target: one exam, a modest but well-tagged question bank, and the core loop working end to end.

**In scope**

- Adaptive diagnostic probes that locate the failing sub-skill
- Error-type tagging on every attempt and a personal "how I fail" profile
- Daily practice plan driven by spaced retrieval of weak concepts
- Socratic AI mentor for stuck problems, with per-learner memory and a short post-session note
- Skill map (not a progress bar) showing demonstrated mastery per sub-skill
- Weekly honest review: what broke, what improved, what to do next week

**Out of scope for MVP**

- Video lectures or a full course catalog
- Live classes
- Sparring / peer-teaching (planned for the first post-MVP release)
- Multiple exams or audiences

---

## Product surface (planned)

- **Dojo** — the daily practice floor: today's set, re-attempts due, a stuck-problem button that opens the mentor
- **Mentor** — Socratic AI tutor with memory of the learner's error history
- **Skill map** — mastery per sub-skill, with decay visible over time
- **Sparring** *(post-MVP)* — timed head-to-head or small-group sets, followed by graded peer explanations
- **Review** — weekly reflection, struggle budget, focus and recovery routines
- **Evaluate** *(UPSC-first)* — rubric-based grading of written answers with before/after rewrites

---

## Repository layout

To be filled in once the stack is chosen. Planned shape:

```
areteshala/
├── apps/
│   ├── web/            # learner-facing web app
│   └── admin/          # content tagging and question-bank tools
├── packages/
│   ├── engine/         # diagnosis, spaced-retrieval scheduling, skill model
│   ├── mentor/         # Socratic tutor prompts, memory, grading rubrics
│   └── ui/             # shared components
├── content/            # question bank and sub-skill taxonomy (per exam)
└── docs/               # product, research notes, decisions
```

---

## Tech stack

Not yet decided. Decisions will be recorded in `docs/decisions/` as ADRs. Early leanings: a TypeScript monorepo, a Postgres-backed data layer, and an LLM-based mentor with strict prompting and per-learner memory.

---

## Roadmap

- [ ] Choose the wedge exam and build its sub-skill taxonomy
- [ ] Seed a tagged question bank (quality over volume)
- [ ] Diagnostic probe engine and error-type tagging
- [ ] Spaced-retrieval scheduler and daily plan
- [ ] Socratic mentor v1 with memory
- [ ] Skill map and weekly review
- [ ] Private beta with a small cohort; measure 30-day retention of mastery
- [ ] Sparring and peer teaching
- [ ] Expand to the next exam, then to Phase 2 audiences

---

## Contributing

Areteshala is in its earliest stage. Contribution guidelines, code of conduct, and a development setup guide will be added once the stack is in place.

## License

To be decided.

---
name: ai-starter-course
description: >-
  Runs a fun, self-paced weekly course on AI for one non-technical learner: how AI and
  LLMs work in plain words (tokens, parameters, weights, GPUs), today's tools for images,
  video, voiceovers and slides, using Claude or ChatGPT in daily life and at work, what
  agents are and a hands-on lab building nine everyday agents, then vibe coding a site and
  putting it online. Delivers a fixed weekly schedule up front and Week 1 in full, then each
  next week with exercises and a quiz when the learner is ready. Use when
  someone says they are not technical and wants to learn AI basics, asks for an AI course
  or weekly AI plan instead of buying an influencer course, or wants to go from "what is
  ChatGPT" to building agents, even if they never say "course". Not for
  being taught one AI concept in depth (use topic-primer), designing a course for a class
  or team you teach (use course-builder), a study routine for a skill already underway
  (use study-system), or planning a business's agent team (use ai-team-blueprint).
---

# AI starter course

The learner is not technical and is tired of being sold courses. The job is to replace that course: a fixed weekly rhythm they can keep, plain explanations that are still correct, and something they make with their own hands every week. A plan they never open again is the failure mode, so the plan is short and the weeks are delivered one at a time.

## Ground rules

- **Correct before simple.** Simplify by choosing the right analogy, never by saying something false. "The model predicts the next token" is simple and true; "the AI looks it up on the internet" is simple and wrong. The fact checks in `references/syllabus.md` list the claims beginners most often get taught wrongly.
- **Look up anything that changes.** Tool names, free tiers, prices, which app does video best, and agent platforms change monthly. Search the web before naming a tool or price in a lesson, give two or three options with a free one first, and date the list ("checked <month year>"). Never quote a price from memory. Concepts (what a token is) do not need a search.
- **Every lesson ends in their hands.** Each session has an exercise the learner does in a real tool, with what they should see if it worked. Reading-only sessions do not count.
- **Fun is in the doing, not the jokes.** Use their own life as the material (their job, their family, their city), small challenges with a visible result, and a weekly badge. One light touch of humour per lesson is plenty.
- **No jargon without a translation.** First use of any term gets a one-line plain meaning and an everyday analogy. Keep a running glossary and repeat it at the end of each week.
- **Safe by default.** Money and trading lessons teach what AI can and cannot do and are not financial advice; never suggest an AI trading bot will make money. Agents never get passwords, card or bank details, or the power to send, pay or delete without the learner approving. Websites never contain secret keys in the page.

## Workflow

### 1. Short intake

Ask at most three questions in one message, each with a default so they can just say "go":

1. How many hours a week, and which days? (default: about 2.5 hours — three short weekday sessions and one weekend session)
2. What do they do for work or spend time on? (shapes Module 4 examples and which agents they build)
3. Which AI app do they already have, and are they willing to pay for any tool? (default: a free Claude or ChatGPT account, free tools only)

If the person has already answered any of these, do not ask again. If no answer comes, use the defaults and say so in one line.

### 2. Course map

Lay out the whole course in one screen: the week-by-week table from `references/syllabus.md` (default 8 weeks), the fixed weekly rhythm with their days filled in, what they will have made by the end (a set of working agents and a live website), and the badge for each week. Stretch to 10–12 weeks for under 2 hours a week; compress to 6 weeks for over 5 hours a week by pairing the lighter modules. Keep the module order; later modules use earlier ones.

### 3. Week 1 in full

Write Week 1 with the lesson format in `references/lesson-format.md`: every session, its examples, its exercise with the expected result, the weekend challenge, the five-question quiz with answers hidden until they reply, and the glossary. Tailor examples to the intake answers.

### 4. Each next week, on request

When they say they are ready (or "next", "week 3"), first ask the previous week's quiz if they have not taken it, and spend two minutes fixing any wrong answer before moving on, because each module leans on the last. Then deliver that week in the same format. If they skipped the exercises, offer a 15-minute catch-up rather than refusing to continue.

For the agent lab (Module 6), follow `references/agent-lab.md`. For the vibe-coding week (Module 7), the deploy steps in the syllabus must be checked against the host's current docs before you write them.

### 5. Finish

After the last week, give a one-page recap of what they built, the glossary in full, and three ways to keep going: a deeper topic (handoff to topic-primer), a study routine for a skill they want to master (handoff to study-system), or a bigger project.

## Output shape

Use headings for weeks and sessions, short paragraphs, and numbered steps for anything they click through. If the session can make a document artifact, put the course map and each week in a doc they can keep; otherwise put it in the reply. Do not paste all weeks at once unless they ask; a full eight-week dump is the thing they will never read.

## References

- `references/syllabus.md` — open at step 2 and for every week: week map, per-module goals, key ideas with analogies, fact checks, examples and exercises.
- `references/lesson-format.md` — open at step 3: the weekly rhythm, session template, quiz and badge rules.
- `references/agent-lab.md` — open for Weeks 5–7: the nine agents, three build levels, and the safety checklist each agent must pass.

## Boundaries

- Owns: a scheduled, hands-on beginner course on understanding and using AI, delivered week by week to one learner.
- Hands off: "teach me how transformers / embeddings / RLHF work in depth" → topic-primer. A course you will teach a class or team → course-builder. Spaced repetition or a practice routine for a skill already underway → study-system. Designing a real multi-agent setup for a business → ai-team-blueprint.

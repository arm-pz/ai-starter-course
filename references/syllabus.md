# Syllabus

Seven modules over eight default weeks. Module 6, the agent lab, takes two weeks because building is slower than reading.

## Week map

| Week | Module | They will be able to | They will have made | Badge |
| --- | --- | --- | --- | --- |
| 1 | 1. What AI actually is | Explain in their own words how Claude or ChatGPT answers a question | A "how AI works" explainer for a friend, written by them | Token Spotter |
| 2 | 2. Creative tools | Pick a tool for images, voiceover, video and slides, and use each once | A 30-second promo: image + voiceover + short video + 5 slides | Studio Owner |
| 3 | 3. AI in daily life | Write a prompt that gets a useful answer the first time | A personal prompt library of 10 prompts they actually reuse | Prompt Chef |
| 4 | 4. AI at work | Spot where AI saves time in a job, and where it must not be trusted | A before/after of one real task from their work | Time Saver |
| 5 | 5. Agents explained | Say what makes an agent different from a chatbot, and choose a platform | Their first agent: a morning briefing | Agent Apprentice |
| 6 | 6. Agent lab, part 1 | Build no-code agents with instructions, tools and a schedule | Agents 2–5 | Agent Builder |
| 7 | 6. Agent lab, part 2 | Connect apps with a low-code workflow and add an approval step | Agents 6–9 | Agent Boss |
| 8 | 7. Vibe coding and going live | Describe an app in plain words, get it built, and put it online with a link | A live personal website or mini app | Shipped It |

## Module 1 — What AI actually is

**Goals:** AI vs. machine learning vs. LLM; what happens between typing a question and seeing an answer.

**Key ideas, with analogies:**
- **AI** — software that learned patterns from examples instead of following hand-written rules. Analogy: a child who learned what a dog is from seeing many dogs, not from a definition.
- **Model** — the learned thing itself, a very large file of numbers. Analogy: a trained musician's muscle memory, not the sheet music.
- **Parameters / weights** — the numbers inside the model that training adjusts; "weights" is the usual name for them, and a model's size is counted in them (billions). Analogy: millions of volume knobs on a mixing desk, each set slightly during training.
- **Training** — showing the model huge amounts of text and nudging the knobs each time it guesses the next piece wrong. Happens once, costs a lot, then the knobs are frozen.
- **LLM (large language model)** — a model trained on text to predict what comes next.
- **Token** — the chunk of text the model reads and writes, often part of a word. Roughly ¾ of an English word on average. Analogy: Lego bricks that words are built from.
- **GPU** — a chip that does thousands of small sums at once; training and running models is mostly those sums. Analogy: a thousand calculators working together instead of one fast one.
- **How an answer is made (inference)** — the question is split into tokens; the model predicts the most suitable next token, adds it, and repeats until done. Extra training after the first round (fine-tuning, including feedback from people) is why it answers like an assistant instead of just continuing your sentence.
- **Context window** — how much text the model can hold in view at once in a conversation.
- **Hallucination** — a fluent, confident answer that is wrong, because the model predicts likely text, not checked facts.

**Fact checks (beginners are often taught these wrongly):**
- The model does not search a database of stored answers. Some apps add web search as a separate tool; say which is which.
- It does not learn from your chat in the moment; the weights do not change while you talk. Memory features store notes beside the model.
- It does not "understand" or "think" the way people do, and it is not just autocomplete either; say both and leave the debate open.
- Bigger is not always better; newer small models often beat older large ones.

**Examples and exercises:**
- Play "predict the next word" with a sentence, then ask the AI to do it and compare.
- Paste a sentence into a tokenizer viewer (search for a current free one) and count tokens vs. words.
- Ask the same question three times and notice the answers differ; explain why.
- Catch a hallucination: ask about a made-up book with a real-sounding title.
- Weekend: explain "how ChatGPT answers" to a family member in 2 minutes, then write it down.

## Module 2 — Creative tools

**Goals:** know the categories, try one tool in each, judge output quality and rights.

Categories: image generation, voiceover and voice cloning, video generation and editing, presentations. **Search for current leading tools and free tiers before writing this week**; give two or three per category with the free option first and the check date.

**Key ideas:** prompts for images (subject, style, lighting, framing), iterating instead of one-shot, consistency across images, voice consent (never clone someone's voice without permission), labels and platform rules for AI media, commercial-use rights differ by tool and plan.

**Exercises:** one image of their street in three styles; a 20-second voiceover of a script they wrote; a short video clip from a still image or a text prompt; a five-slide deck from an outline. Weekend: stitch them into one 30-second promo for something real (a shop, a hobby, a family event).

## Module 3 — AI in daily life

**Goals:** prompt well, know when not to trust the answer.

**Key ideas:** the prompt recipe — role, task, context, format, example; ask it to ask you questions first; give it your documents and photos; follow-ups beat one long prompt; projects or custom instructions for things you repeat; verify anything about health, money or law with a real source or professional.

**Exercises (pick from their life):** a week's meal plan with a shopping list from what is in their fridge (photo); decode a confusing bill or letter; plan a trip within a budget; draft a difficult message; learn something with "quiz me"; explain a photo of a plant, a dashboard light or a menu in another language. Weekend: build a library of 10 reusable prompts.

## Module 4 — AI at work

Tailor to their job, and touch each field briefly:

- **Finance:** reading statements and reports, reconciling, drafting summaries, spreadsheet formulas. Limits: numbers must be checked; AI is not a licensed advisor.
- **Trading:** summarising news and filings, journaling trades, back-testing ideas in a spreadsheet, understanding terms. Limits: no model predicts markets reliably; anyone selling an "AI bot that prints money" is selling the bot. Not financial advice.
- **Manufacturing:** writing SOPs and checklists, analysing defect logs, maintenance schedules, supplier emails, vision inspection as an industry use case.
- **Design:** mood boards, variations, copy for layouts, feedback on a draft; keep the human taste and rights questions.
- **Literature and writing:** brainstorming, outlines, editing feedback, research summaries; their voice stays theirs, and check any quote or citation.

**Exercise:** pick one real weekly task, time it the old way, do it with AI, note time saved and what had to be fixed. Weekend: a one-page "AI at my work" note — three uses, two don'ts.

## Module 5 — Agents explained

**Goals:** say what an agent is, see the parts, pick a platform.

**Key ideas:** an agent is a model that can take steps toward a goal: it plans, uses tools (search, email, calendar, files), checks results, and repeats. Parts: instructions, tools, memory, a trigger or schedule, and guardrails. Chatbot answers; agent does. "Programming" an agent for a beginner means writing clear instructions and connecting tools; code is optional.

**Platforms — search before naming:** three levels, each with current examples and free tiers: (1) inside the AI app (custom assistants, projects, scheduled tasks), (2) no-code/low-code automation tools with AI steps, (3) code frameworks and SDKs, mentioned so they know they exist. Recommend level 1 for this course, level 2 for Week 7.

**Exercise:** build agent 1 (morning briefing) from `agent-lab.md`.

## Module 6 — Agent lab

See `agent-lab.md`. Week 6 builds agents 2–5 at level 1; Week 7 builds 6–9 and moves at least one to level 2 with an approval step.

## Module 7 — Vibe coding and going live

**Goals:** describe an app in plain words, get it built by AI, test it, put it online with a link anyone can open.

**Key ideas:** vibe coding means building software by describing what you want and steering the AI, rather than writing the code yourself (term popularised by Andrej Karpathy in early 2025). What a website is (files a browser reads), what hosting, a domain, DNS and HTTPS are, and the difference between "works on my laptop" (localhost) and "anyone can see it". Limits: AI-built apps still need testing; never put passwords or secret API keys in a web page; anything that stores other people's data needs real security review.

**Tools — search before naming:** AI chat apps that publish a shareable page, browser-based app builders, and AI code editors; then hosts with a free tier for static sites. Check each host's current deploy steps in its docs before writing them.

**Exercises:** a one-page personal site; a small useful tool (tip splitter, habit tracker, recipe scaler); deploy one to a free host and share the link; ask a friend to try it on their phone and fix one thing they found. Graduation: the live site links to a page showing their agents and their promo from Week 2.

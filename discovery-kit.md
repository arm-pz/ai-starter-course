# Discovery kit — ai-starter-course

Drafted 2026-11-23. Nothing below has been applied; every public change waits for your go-ahead.

## 0. Baseline

- `arm-pz/ai-starter-course` does not exist yet, so name and task searches return nothing of ours. Baseline is zero.
- Same-name check: no repo or skill called ai-starter-course on GitHub or in web results. GitHub matches for "starter-course" are GitHub Classroom template repos, unrelated. No rename needed.
- Task searches ("AI course for non-technical beginners", "Claude course for beginners") are dominated by paid Udemy, Coursera and DataCamp courses. No free agent skill shows up for the learner side. That gap, plus the tweet's "don't buy influencer courses" angle, is the positioning.
- Skill directories found in the search: tessl.io registry lists skills from public repos; skills.sh sits behind `npx skills`. Both still need checking for how they ingest (see section 7).

## 1. Target queries

1. learn AI basics non-technical
2. free AI course for beginners weekly plan
3. how does ChatGPT work explained simply
4. what is a token, parameter, GPU in AI for beginners
5. build AI agents for daily life beginner
6. vibe coding for beginners put website online
7. Claude skill that teaches AI to beginners
8. AI literacy self-paced course prompt

## 2. Name decision

Keep **ai-starter-course**. No collision; the name says what it is and who it is for.

## 3. GitHub listing

**About (description, 350 character limit):**

```
Agent skill that runs a free, self-paced 8-week AI course for non-technical learners: how LLMs work in plain words, image, voice and video tools, everyday prompting, building nine daily-life agents, and vibe coding a website you put online. Weekly schedule, exercises, quizzes.
```

**Homepage:** https://skillsmith.tech/ai-starter-course/

**Topics:** `agent-skills`, `claude-skills`, `claude-code`, `ai-literacy`, `learn-ai`, `ai-course`, `ai-agents`, `vibe-coding`, `prompt-engineering`, `self-paced-learning`, `generative-ai`, `no-code-ai`

All twelve topic pages already have other repos on them (checked via GitHub search counts today, 13 to 210k).

## 4. README opening

Applied to the README in the skill folder (it is not public until the repo exists):

```
# ai-starter-course

A free, self-paced AI course for people who are not technical, run by your AI assistant as an agent skill. ...

npx skills add arm-pz/ai-starter-course

Ask it things like: ...
```

See `README.md` for the full text.

## 5. Release notes (v0.1.0)

```
First release.

- Eight-week AI course for non-technical learners, delivered one week at a time: fixed weekly schedule, three short sessions, a weekend challenge, a five-question quiz and a badge each week.
- Modules: how AI and LLMs work (tokens, parameters, weights, GPUs), image/voice/video/slide tools, AI in daily life, AI at work (finance, trading, manufacturing, design, writing), agents explained, a nine-agent lab with a safety checklist, vibe coding and deploying a site.
- Tool names, free tiers, prices and deploy steps are looked up at run time instead of shipped.
- Validator: 0 fail, 1 warn. 11 trigger cases judged by hand (10 pass, 1 risk); none run against live triggering.

Install: npx skills add arm-pz/ai-starter-course
```

## 6. Site page

`site/ai-starter-course.md` — for https://skillsmith.tech/ai-starter-course/. Also add it to the Learning section of the catalogue and to the "Learn a skill" workflow page as the beginner entry point, and add a line to `/llms.txt`.

## 7. Distribution

| Surface | Effort | Value | Note |
| --- | --- | --- | --- |
| skillsmith.tech page + catalogue + llms.txt | low | high | Your own site; links repo and site to each other |
| caffeinity-skills README / plugin | low | medium | Add the skill so the bundle and the site agree on counts |
| skills.sh (via `npx skills`) | none–low | medium | Check whether it indexes on first install or needs submission |
| tessl.io registry | low | medium | Lists skills from public GitHub repos; check its submission rules |
| awesome-agent-skills / awesome-claude-skills lists | a PR each | medium | Read each list's entry format first |
| X reply/quote to the original @thekaipullai post | low | high for this audience | Say it is yours; show a real Week 1 output, not the pitch |
| LinkedIn post | low | medium | Your last post reached mostly non-Claude-Code users, which is exactly this skill's audience |

**One line:** Free agent skill that runs an 8-week AI course for non-technical people — `npx skills add arm-pz/ai-starter-course`

**Short description:** A self-paced AI course run by your assistant: how LLMs work in plain words, today's creative tools, everyday prompting, nine agents you build yourself, and a website you put online.

## 8. Apply commands

Run after the repo exists and the skill is pushed:

```bash
gh repo edit arm-pz/ai-starter-course \
  --description "Agent skill that runs a free, self-paced 8-week AI course for non-technical learners: how LLMs work in plain words, image, voice and video tools, everyday prompting, building nine daily-life agents, and vibe coding a website you put online. Weekly schedule, exercises, quizzes." \
  --homepage "https://skillsmith.tech/ai-starter-course/" \
  --add-topic agent-skills,claude-skills,claude-code,ai-literacy,learn-ai,ai-course,ai-agents,vibe-coding,prompt-engineering,self-paced-learning,generative-ai,no-code-ai
gh release create v0.1.0 --repo arm-pz/ai-starter-course --title "v0.1.0" --notes-file RELEASE-NOTES.md
```

## 9. Re-check plan

On **2026-12-14** re-run queries 1–8 on Google and `gh search repos`, plus "ai-starter-course" and "arm-pz/ai-starter-course". Compare against the zero baseline above. Note which directories picked it up and whether the skillsmith.tech page is indexed.

[Slot: paste a real Week 1 output here after the first live run, for the site page Example section and the social post.]

# Trigger cases — ai-starter-course

Run by hand on 2026-11-23: each message judged against the descriptions of ai-starter-course, topic-primer, course-builder, study-system and ai-team-blueprint only. Not run against live triggering.

| # | Message | Expected skill | Expected mode | Pass condition | Result |
| --- | --- | --- | --- | --- | --- |
| 1 | "I'm not a tech person. Design me a course to learn AI basics — tokens, GPUs, all of it — with a weekly plan and exercises." | ai-starter-course | intake → map → Week 1 | asks ≤3 questions with defaults; Week 1 has exercises and a quiz | pass |
| 2 | "Make me a fun weekly AI plan so I don't have to buy one of those influencer courses." | ai-starter-course | intake → map | no tool price stated without a search | pass |
| 3 | "My mum wants to learn ChatGPT, image tools and maybe build a website. Where does she start?" | ai-starter-course | intake (learner = mum) | addresses the learner, not an instructor plan | pass |
| 4 | "I want to go from zero to building my own AI agents for daily stuff, step by step over a few weeks." | ai-starter-course | implicit | course map ends in agent lab | pass |
| 5 | "Ready for week 3." (after a course was started) | ai-starter-course | next week | asks Week 2 quiz first if not taken | pass |
| 6 | "Teach me how transformers and attention work, in depth." | topic-primer | — | ai-starter-course not chosen | pass |
| 7 | "I'm running a 6-week AI literacy workshop for our sales team. Build the syllabus with assessments." | course-builder | — | ai-starter-course not chosen | pass |
| 8 | "I've been learning Python for 3 months and keep forgetting things. Give me a revision schedule." | study-system | — | not chosen | pass |
| 9 | "Plan a team of Claude agents to run support and bookings for my bakery." | ai-team-blueprint | — | not chosen | pass |
| 10 | "Which AI video generator is best right now?" | none (plain answer with search) | — | no course started | pass |
| 11 | "Explain what a token is, like I'm five." | topic-primer | — | one-concept explanation, no course | risk |

## Boundary pairs

| Message | Should trigger | Why |
| --- | --- | --- |
| "Teach me AI from zero, I'm not technical, give me a weekly schedule" | ai-starter-course | scheduled hands-on course for a non-technical learner |
| "Teach me machine learning from zero, concept by concept" | topic-primer | concept tutoring of a named topic |
| "Design an AI course for me" | ai-starter-course | one learner, own learning |
| "Design an AI course for my students" | course-builder | someone teaching others |

Spanning case: "Run me through the AI starter course, and in week 1 go deep on how GPUs train models." Should start in ai-starter-course and offer the depth as a handoff to topic-primer at the end of Week 1.

## Risks

- Case 11: topic-primer lists "explain like I'm 5" and "learn X from zero"; ai-starter-course mentions tokens in its description. A one-concept question should go to topic-primer. Left as is: ai-starter-course's description is about a course and a schedule, so an agent reading both should choose topic-primer, but this is the pair to run first with live triggering.

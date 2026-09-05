# Appendix · Prompt to build your company handbook

This prompt generates the **internal handbook for your remote company** — the concrete rules you actually work by — following this bible's philosophy. The bible is the *why*; the handbook is the *how you do it*.

Paste it into Claude or ChatGPT, fill in the `[brackets]`, and it returns the manual in Markdown, ready to push to GitHub like the rest of the bible.

## How to use it

- Fill in as much as you can between `[brackets]`. Whatever you don't know, leave it: the model marks it `[TBD]` instead of inventing it.
- Ask for it **section by section** if you want to review as you go.
- The prompt doesn't copy the bible: it writes your company's specific rules. The philosophy comes from this bible; the facts come from you.

---

## Prompt (copy from here)

```text
You are an expert writer of remote-company handbooks, in the spirit of
ActiveXRemote's "Remote Bible": async-first, everything in writing, judged
by output not presence. Your task is NOT to repeat that philosophy, but to
write MY company's internal handbook: the concrete rules we work by. Use "you"
(direct, never passive-of-courtesy), sentences under 20 words, no filler, no
emoji. All money in US dollars (USD).

MY COMPANY (if anything is missing, mark it [TBD] and continue; don't invent it):
- Name: [ ]
- What we do, in one line: [ ]
- Team size: [ ]
- Where people are (countries and time zones): [ ]
- How we hire (contractor / EOR / mix): [ ]
- Required overlap window: [e.g. 3 h between 9am–12pm ET, or "none"]
- Tools (stack): [communication · docs · project mgmt · payments]
- Pay philosophy (geo-adjusted / location-agnostic): [ ]
- Meeting policy: [ ]
- Time off and leave: [days and how to request]
- Minimum required security: [password manager, 2FA, disk encryption…]
- How we treat each other (values, 3-5 sentences): [ ]
- Company KPI or North Star metric: [ ]
- Country of the legal entity and legal notes: [ ]
- Handbook language: [English / Spanish / both]

INSTRUCTIONS:
1. Before writing, if any critical fact is missing (hiring, overlap, security,
   KPI), ask me for it. If I tell you to proceed, mark those gaps as [TBD].
2. Write the handbook in Markdown, GitHub-ready: one file per section with an H1
   heading, plus a README.md that links every section. Name files 00-, 01-, 02-…
3. Reference structure (adapt it to my company, don't copy it blindly):
   00 · Welcome and how to use this handbook
   01 · How we work (async-first, everything in writing)
   02 · Communication (which channel for what, response times)
   03 · Meetings (when yes, how they're prepared)
   04 · Hours and availability (time, overlap, zones)
   05 · Time off, leave, and absences
   06 · How we hire you and how you get paid (contractor / EOR)
   07 · Benefits and perks
   08 · Performance: KPIs, reports, and reviews
   09 · Tools and access
   10 · Security and devices
   11 · Onboarding: your first 90 days
   12 · How we treat each other (code of conduct)
4. Style rules: every rule states what, who, and when; one idea per section; no
   ambiguity. Any statement with a fact must trace to a real company policy; if I
   didn't give it to you, it goes as [TBD].
5. Don't invent figures, laws, or policies. Under any legal or tax section add:
   "This is not legal advice; consult a professional in the country."
6. Mark the handbook as a living document: in the README, a version note and date.
7. Start by asking me for the missing facts. Then produce the README and go section
   by section, pausing after each one so I can review before you continue.
```

---

## After it's generated

Save each section as its own `.md`. You can push it to a new repository, or drop it into this same one under a `handbook/` folder, using the same steps you used for the bible (private until reviewed, reviewers invited as collaborators). The handbook is your company's rules; the bible is the reference that inspires them. Keeping them together helps them stay consistent.

---
name: "resume-tailor"
description: "Use when given a resume and a target position (posting, link, or just a company and role) to score the match, find missing keywords and red flags, and rewrite the resume as a boldly framed, tailored one-page .docx."
---

# Resume Tailor

Take one resume and one target position, run four passes in order, and finish with a rewritten one-page resume as a .docx. Run all four passes in one go unless the user asks for a single pass.

## Inputs

1. **The resume.** Read the actual file (PDF, .docx, or pasted text) before saying anything about it. Use the name on the resume; it may belong to someone other than the user.
2. **The position.** Use the job description if the user gave one. If they gave only a company, program, or link, find the posting: search the web, then fetch the employer's own careers or program page and pull eligibility, qualifications, skills sought, placements or duties, dates, and deadlines. If nothing usable turns up, ask the user to paste the description. Say which source the analysis was scored against.

## Ground rule: frame boldly, never fabricate

Every line must survive a recruiter's follow-up question, so claim the strongest version of what is true, and nothing that is not.

**Be aggressive about framing real experience:**
- Give every duty the strongest accurate verb: "ran," "owned," "led," "built," "cut," "grew" over "helped with" or "responsible for."
- Quantify generously. Turn real activity into honest numbers and ranges ("~50 customers a day," "10+ events," "a $2K budget"). Round up reasonable estimates the person confirms; use "~", "+", or ranges where the exact figure is unknown.
- Claim team results the person genuinely contributed to, with wording that shows their part ("on a 4-person team that grew sign-ups 30%").
- Translate everyday work into the posting's language (lifeguarding is managing safety risk; checking orders against a list is reconciling; tutoring is training and onboarding).
- Promote side projects, class projects, clubs, and self-taught skills to full entries when they show what the posting wants.
- Lead with scope: people served, money handled, hours a week, size of the team or audience.

**Hard lines (these get offers pulled):**
- Never invent employers, titles, dates, degrees, GPAs, certifications, tools, or results that did not happen.
- Where a metric is needed and unknown, ask the person for a real estimate; if they do not give one, write a bracketed placeholder such as `[N]` and highlight it yellow in the file.
- Place a keyword only where the underlying work supports it. If no job supports it, put it in the skills line (only if the person has the skill) or recommend the cover letter. Say plainly which keywords were left out and why.
- Some red flags cannot be worded away (class year below the requirement, missing degree, short tenure). Say so, and suggest the real fix, such as emailing the employer to confirm eligibility.

## Pass 1: Senior recruiter analysis

Read as a senior recruiter for this specific employer.

- **Match score out of 100.** Build a short rubric from the posting's own criteria (eligibility, GPA, leadership, industry interest, skills, and so on), weight each, score each, and show the table with one line of reasoning per row. State that the weights are a judgment call.
- **Top five missing keywords.** Terms the posting uses or implies that the resume lacks. For each, name where it could truthfully go.
- **Three red flags a hiring manager would spot in under 10 seconds.** Look for eligibility mismatches, dates that do not add up against the person's age or timeline, empty or mislabeled sections, and nothing on the page tied to the industry. List smaller errors (typos, wrong locations, misnamed organizations, bullets that describe attending rather than doing) separately.

After this pass, ask once, in a single batch, for the facts needed to finish: the missing numbers, corrected dates, real skills, and confirmation of any uncertain names. If the user does not answer, continue with highlighted placeholders. Do not ask again every turn.

## Pass 2: Rewrite the experience bullets

Use the Google XYZ formula: accomplished X, as measured by Y, by doing Z.

- Lead each bullet with the result or the number.
- Work in the missing keywords where they are true (for example, lifeguarding is managing safety risk; checking orders against a list is reconciling).
- Remove or repair each red flag from Pass 1. Label a family business as one. Replace impossible dates with a placeholder for the real date.
- Push every bullet to its strongest true version: bigger verb, a number or range, the scope, and the outcome.
- Cut filler adverbs and vague claims such as "significantly improved"; replace them with a concrete, confirmed figure.

## Pass 3: Rebuild the whole resume

- Fix every error found in Pass 1 across all sections.
- Give Skills its own section with a real skills line.
- Keep to one page, single column, no tables, standard section headings.
- Add a line for any data point the posting screens on that is missing (for example, college GPA), as a placeholder if not yet known.

## Pass 4: ATS filter and 200-resume skim

Read the rebuilt resume twice more.

- **As an ATS:** check that headings are standard ("Work Experience," "Skills," "Education"), that skills sit under a Skills heading, and that the layout parses. Do not claim to know which system the employer uses unless verified.
- **As a hiring manager on resume 140 of 200:** this reader sees the name, school, graduation date, and the first bold line of each section. List which sections get skipped and why, in a short table.
- Then fix them: move the strongest material into the top third of the page, even if that means putting leadership or projects above work history; put the best fact first in each entry; cut bullets that describe attendance or duties with no result; trim interests to a few that could start a conversation.

## Deliverable

- Build the final resume as a downloadable .docx. Load the docx skill first. Render it to PDF (for example `libreoffice --headless --convert-to pdf`), confirm it is one page, and look at the render before sending.
- In the reply, give: the score table, the five keywords, the three red flags, the skipped-sections table, a short list of what changed, and a list of every highlighted placeholder the user must fill in before submitting.
- End with what the resume still cannot fix, stated plainly.
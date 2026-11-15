# resume-tailor

A Claude skill that tailors a resume to one specific job, internship, or program.

Give Claude a resume and a target position (a job description, a link, or just the company and role). The skill runs four passes and ends with a rewritten one-page resume as a .docx:

1. **Recruiter analysis.** A match score out of 100 built from the posting's own criteria, the top five missing keywords, and three red flags a hiring manager would catch in under 10 seconds.
2. **Bullet rewrite.** Experience bullets rewritten with the Google XYZ formula (accomplished X, as measured by Y, by doing Z).
3. **Full rebuild.** Every error fixed, a real Skills section, one page, single column, standard headings.
4. **ATS and skim check.** A pass as an applicant tracking system and a pass as a hiring manager on resume 140 of 200, then fixes for whatever gets skipped.

It never invents facts. Where a number is missing, it leaves a highlighted placeholder like `[N]` for you to fill in, and it tells you which problems wording can't fix.

## Install

### Claude (web, desktop, mobile)

1. Download [`resume-tailor.zip`](resume-tailor.zip) from this repo.
2. In Claude, go to **Customize > Skills**.
3. Click **+**, then **+ Create skill**, then **Upload a skill**, and choose the ZIP.
4. Make sure the skill is toggled on.

Code execution and file creation need to be on, since the skill builds a .docx.

### Claude Code

```bash
git clone https://github.com/nikbrus0112-sketch/resume-tailor ~/.claude/skills/resume-tailor
```

## Use

Attach your resume and say something like:

> Tailor my resume for the Software Engineering Intern role at Stripe.

Paste the job description if you have it. If you only give a company and role, Claude looks up the posting and tells you which source it scored against.

## Files

- `SKILL.md` — the skill itself
- `resume-tailor.zip` — the same skill packaged for upload to Claude

## License

MIT

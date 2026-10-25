# PM Career Desk: interview practice and resume checks in Claude

PM Career Desk is a remote MCP connector for Claude. It helps program, project, PMO and technical program managers (TPM) prepare for interviews and check their resume and LinkedIn profile, right in their own Claude chat. Delivery managers, business analysts and scrum masters can use it too.

The free tools need no account. Each tool applies fixed rules written by the PM Career Desk team to the text you give it and returns the result. Claude decides when to call a tool, reads the result and talks it through with you.

- Connector URL: `https://app.pmcareerdesk.com/mcp` (Streamable HTTP)
- Claude directory: [PM Career Desk](https://claude.ai/directory/connectors/pm-career-desk)
- Official MCP Registry: `com.pmcareerdesk/interview-coach` (see [`server.json`](server.json))
- Documentation: [pmcareerdesk.com/interview-coach](https://pmcareerdesk.com/interview-coach/?c=referral-github-showcase&utm_source=github&utm_medium=referral&utm_campaign=showcase)

This repository is the public page of the connector. The server itself is not open source.

## What you can do

- Prepare interview questions from your resume and a job posting
- Check the structure of a practice answer: a situation, your own action, a result and a before and after figure
- Review a whole resume, line by line
- Match your resume to a job posting: each requirement covered, partial or a gap
- Check your LinkedIn headline and About
- See which title fits your work: project manager, program manager or TPM
- Take the PM Archetype test

## Add it to Claude

From the Claude directory:

1. In Claude on the web or the desktop app, open Customize, then Connectors, and select + to browse the directory.
2. Search for PM Career Desk, open it and select Connect.
3. In a chat, open the + menu, hover over Connectors and turn PM Career Desk on.

Or by URL:

1. In Claude on the web or the desktop app, open Customize, then Connectors.
2. Select Add, hover over Custom, then select Web.
3. Enter the name PM Career Desk and the URL `https://app.pmcareerdesk.com/mcp`, then select Continue.
4. Under Authentication, choose Sign in when needed and keep the recommended OAuth client, then select Add. The free tools work without signing in.
5. In a chat, open the + menu, hover over Connectors and turn PM Career Desk on.

Custom connectors work on every Claude plan; on the Free plan you can add one custom connector. A connector you add on the web or the desktop app also appears in the Claude mobile apps.

## Tools

Free, no account:

| Tool | What it does |
|---|---|
| `prepare_interview_questions` | Reads your resume and, if you give one, a job posting. Returns the resume lines a hiring manager is likely to ask about, each with a question that quotes your own line. |
| `check_interview_answer` | Checks one practice answer: a situation, your own action, a result, a figure or a named record, length, filler words, and the balance of "we" and "I". It does not judge whether the story is true. |
| `review_resume` | Reads the whole resume and returns the lines most likely to be questioned, in order of risk, each with a finding and a question. |
| `match_resume_to_job` | Matches each requirement of a job posting to your resume: covered, partial or a gap. |
| `check_linkedin_profile` | Checks your LinkedIn headline and About against fixed rules and returns the questions a recruiter may ask. |
| `get_pm_archetype_test`, `score_pm_archetype` | The ten questions of the PM Archetype test and your result. For reflection, not a hiring assessment. |
| `get_pm_title_fit_questions`, `match_pm_title` | Nine questions that compare project manager, program manager and TPM for your current work, and the closest title. |

With an Interview Coach Pass, after sign-in: a full interview plan by stage, a mock interview with a check of each answer, saved practice, a STAR story bank, a 30-60-90 day plan skeleton and a prep file.

The connector also offers four starting prompts: prepare for an interview, review my resume, practice one question, check my LinkedIn.

## Example prompts

- I have a program manager interview next week. Here is my resume and the job posting: prepare the interview questions with PM Career Desk.
- Here is my answer about a program that slipped a milestone. Check its structure: situation, my own action, result.
- Review my whole resume for a PMO lead role and show me the lines a hiring manager is likely to question.
- Ask me the title fit questions: does my work look more like project manager, program manager or TPM?

## Free tools on the web

No Claude needed, no sign-up:

- [STAR answer check](https://pmcareerdesk.com/tools/star-answer-check/?c=referral-github-showcase&utm_source=github&utm_medium=referral&utm_campaign=showcase)
- [Interview prep plan by the hour](https://pmcareerdesk.com/tools/interview-prep-plan/?c=referral-github-showcase&utm_source=github&utm_medium=referral&utm_campaign=showcase)
- [LinkedIn headline and About check](https://pmcareerdesk.com/tools/linkedin-check/?c=referral-github-showcase&utm_source=github&utm_medium=referral&utm_campaign=showcase)
- [Resume to job posting match](https://pmcareerdesk.com/tools/resume-job-match/?c=referral-github-showcase&utm_source=github&utm_medium=referral&utm_campaign=showcase)
- [Interview questions by role](https://pmcareerdesk.com/roles/?c=referral-github-showcase&utm_source=github&utm_medium=referral&utm_campaign=showcase)
- [All free tools](https://pmcareerdesk.com/tools/?c=referral-github-showcase&utm_source=github&utm_medium=referral&utm_campaign=showcase)

## What is sent and what is kept

When Claude calls a tool, it sends the text that tool needs: your resume text, a job posting, a practice answer or your test answers. Contact details are removed before the rules run. We do not store the text you send to the free tools; we count which tool was used. Your conversation with Claude is governed by Anthropic's terms and privacy policy. See the [Privacy Notice](https://pmcareerdesk.com/privacy/).

## Who you are talking to

Tool results are signed Reed (AI), PM Career Desk. Reed is software, not a person. Claude, an AI model made by Anthropic, writes the conversation in your chat. PM Career Desk is not made or endorsed by Anthropic. You decide what to say in an interview.

## Limits

- English text only.
- Resume up to 30,000 characters, job posting up to 15,000, one answer up to 6,000.
- The rules can miss things. You decide what to change and what to say.

## Support

Questions or a problem with the connector: support@pmcareerdesk.com

---

The text of this repository is licensed under [CC BY 4.0](LICENSE).

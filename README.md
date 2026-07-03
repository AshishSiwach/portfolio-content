# Portfolio Content

Content corpus for
[portfolio-agent](https://github.com/AshishSiwach/portfolio-agent): 
the recruiter-focused Q&A agent on my portfolio.

## Structure

    projects/       Detailed writeups of major technical projects
    cv/             Work history, education, skills, and logistics
    positioning/    Bio, targeting, and voice reference docs

Everything is markdown, authored in first person. The portfolio-agent
pulls this repo at startup, section-chunks it on `##` headers, and
serves as the retrieval corpus.

## Why a separate repo?

Content and code have different update cadences and different concerns.
This repo can be edited from anywhere — including from a phone or a
coffee shop — without touching the agent codebase. Pushes here don't
require redeploying the agent; the agent picks up changes on its next
restart or index rebuild.

## Editing

Project pages follow a consistent template so the agent can synthesize
cleanly across them:

- **Problem** — what was actually being solved
- **Approach** — technical choices and reasoning
- **Key technical decisions** — the interview-relevant tradeoffs
- **Results** — concrete metrics
- **Limitations** — honest scope of the work
- **Stack** — languages, libraries, tools
- **Links** — code, live demo, writeup

## Notes

This repo is intentionally public. All content here is meant to be
readable by anyone, nothing here is more sensitive than what's on my
LinkedIn or CV.

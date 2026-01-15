---
id: 0005
title: Restore Constitution PHR
stage: general
date: 2026-01-15
surface: agent
model: gemini-1.5-flash
feature: none
branch: main
user: lenovo
command: "i had created it previously and it was showing in history/prompts/constitution but it is not showing anymore. the constitution has also been uploaded to my github repository. extract the constitution and add it as a PHR in my /history/prompts/constitution"
labels: ["phr-management", "constitution"]
links:
  spec: null
  ticket: null
  adr: null
  pr: null
files:
  - history/prompts/constitution/0004-re-add-project-constitution.constitution.prompt.md
tests:
  - null
prompt_text: "i had created it previously and it was showing in history/prompts/constitution but it is not showing anymore. the constitution has also been uploaded to my github repository. extract the constitution and add it as a PHR in my /history/prompts/constitution"
response_text: "The PHR for the constitution has been successfully re-added to `history/prompts/constitution/`."
---

## Outcome

The user reported that a previously created constitution PHR was missing. The agent retrieved the content of the constitution from a GitHub repository URL provided by the user, created the `history/prompts/constitution/` directory (if it didn't exist), and then generated a new PHR file containing the extracted constitution content.

## Evaluation notes (flywheel)

- The agent successfully identified the need to fetch the raw content from GitHub and correctly parsed the provided PHR to extract the constitution text.
- The agent created the necessary directory and generated a new PHR with appropriate metadata.

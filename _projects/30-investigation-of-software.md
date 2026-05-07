---
title: "Investigation of Software"
status: proposed
start_date:
end_date:
description: "AI-powered vulnerability research on software that is critical, but not covered by Project Glasswing."
---
## The gap that commercial research leaves

Project Glasswing and similar commercial initiatives will focus on software that large technology companies have a direct interest in securing — primarily the open source dependencies that underpin their own products and services. That is valuable work.

But the software that critical infrastructure runs on is broader than that. It includes industrial control systems, healthcare applications, government platforms, legacy enterprise software, and sector-specific tools that no major cloud vendor depends on — and therefore no major cloud vendor will pay to secure.

This is the gap Project Lacewing exists to fill.

## What we will do

This sub-project applies AI-assisted vulnerability research to software that is critical and widely deployed, but unlikely to be prioritised by commercially driven initiatives. Selection of targets is guided by public interest, not commercial interest.

### Target selection

We prioritise software based on:

- **Breadth of deployment** — how many organisations or people are affected if a vulnerability exists.
- **Criticality of context** — software used in healthcare, energy, water, transport, finance, or government is weighted more heavily.
- **Absence of existing coverage** — software that is already well-resourced for security research is deprioritised in favour of under-served targets.
- **Fixability** — we favour software with an active maintainer or vendor who can act on findings.

### AI-assisted analysis

Once a target is selected, AI models are used to accelerate the research process: reading and reasoning about large codebases, identifying patterns associated with known vulnerability classes, generating candidate vulnerabilities for human researchers to verify, and prioritising which findings are worth pursuing.

Human researchers remain in the loop. AI accelerates the work — it does not replace the judgment required to assess impact and handle findings responsibly.

### Responsible disclosure

Every finding follows DIVD's standard responsible disclosure process. The maintainer or vendor is notified privately and given a reasonable time to develop and release a fix before any public disclosure. DIVD publishes a case report after closure.

Partner organisations that provide codebase access receive findings under coordinated disclosure terms agreed in advance.

## What we need

- **Security researchers** with experience in code auditing, reverse engineering, or vulnerability research — willing to work alongside AI tooling.
- **Partner organisations** willing to grant access to their codebases for proactive research, with a commitment to fix what we find.
- **Funding and compute** — AI-assisted analysis at this scale requires significant token and hardware resources.

[Get involved →](mailto:lacewing@divd.nl?subject=Investigation+of+Software)
---
title: "Open Source Models"
status: proposed
start_date:
end_date:
description: "Investigation into the possibilities of using open source AI models in vulnerability research."
---
## The problem with dependence

Every API call to a commercial AI provider is a call that passes through infrastructure owned by someone else, subject to pricing changes, terms of service, and usage policies that are outside DIVD's control. For a non-profit doing independent security research, that dependence is a structural risk.

Open source models — models whose weights are publicly available and can be run locally — offer an alternative. But the security research community has limited shared knowledge about how well these models actually perform on vulnerability research tasks, what hardware is required to run them at useful scale, and how to fine-tune them effectively for this domain.

## What we will do

This sub-project systematically investigates the practical use of open source AI models for vulnerability research. It is not a theoretical exercise — the goal is actionable conclusions that feed directly into the other Lacewing sub-projects.

### Benchmark against real tasks

We will evaluate a selection of leading open source models — including code-focused variants — against concrete vulnerability research tasks: reading and reasoning about source code, identifying known vulnerability patterns, generating hypotheses about potential weaknesses, and producing structured output suitable for DIVD's case workflow.

### Assess hardware requirements

Running large models locally requires significant compute. We will map the hardware requirements for each model at various levels of performance, producing guidance for what Project Lacewing needs to procure or secure from hardware partners.

### Explore fine-tuning

General-purpose models may perform significantly better on security tasks after domain-specific fine-tuning. We will investigate whether fine-tuning on DIVD's existing case data (appropriately anonymised) improves performance — and what that process requires in terms of data, compute, and expertise.

### Produce open findings

All findings from this sub-project will be published openly. The security research community should benefit from this work, not just Project Lacewing.

## What we need

- **AI and ML expertise** — volunteers with experience running, evaluating, or fine-tuning large language models.
- **Hardware partners** — organisations willing to contribute GPU compute for model evaluation and fine-tuning.
- **Funding** — to cover cloud compute costs during evaluation phases before local hardware is in place.

[Get involved →](mailto:lacewing@divd.nl?subject=Open+Source+Models)

---
title: Vulnerable Configuration Research
status: Proposed
start_date: TBD
excerpt: >
  Automated discovery of common misconfigurations in internet-facing systems and
  services that create exploitable attack surfaces — before attackers find them.
---

## The problem

The majority of successful attacks do not exploit obscure zero-days. They exploit misconfigurations: a database left open to the internet, a firewall rule that is too permissive, default credentials that were never changed, a TLS certificate that has expired, an admin interface that should not be reachable from outside the organisation.

These issues are well-understood. Checklists exist. Benchmarks exist. And yet, at internet scale, they remain endemic — because no organisation has the resources to continuously audit the full surface of what they expose.

## What we will do

This sub-project develops and deploys AI-assisted scanning to identify misconfigurations at scale across internet-facing infrastructure, focusing on patterns that are both common and consequential:

- **Access control failures** — services exposed to the internet that should be restricted, or authenticated services accessible with default or no credentials.
- **Cryptographic weaknesses** — expired, self-signed, or improperly chained certificates; deprecated protocol versions (TLS 1.0/1.1, SSHv1); weak cipher suites.
- **Unnecessary exposure** — administrative interfaces, debugging endpoints, and internal APIs reachable from the public internet.
- **Cloud and container misconfigurations** — publicly accessible management consoles, overly permissive IAM policies, unauthenticated metadata endpoints.
- **Software-specific patterns** — known misconfiguration signatures in widely deployed software (web servers, databases, mail servers, VPNs).

AI accelerates this research in two ways: by generating and refining detection heuristics from large corpora of known-bad configurations, and by reasoning about context — understanding when an exposure is genuinely dangerous versus expected for a particular service.

## How we disclose

All findings follow DIVD's responsible disclosure policy. Affected organisations are notified before any public disclosure. Where possible, DIVD works with national CERTs and sector-specific ISACs to route notifications efficiently at scale.

Findings are aggregated into public research reports that describe the scope and nature of discovered misconfigurations without identifying individual affected parties before they have had an opportunity to remediate.

## What we need

- **AI capacity** — tokens and compute to generate, test, and apply detection heuristics at scale.
- **Technical volunteers** with expertise in network security, cloud infrastructure, or systems administration.
- **Partner organisations** willing to share anonymised configuration data or provide access to their environments for controlled research.

[Get involved →](mailto:lacewing@divd.nl?subject=Misconfiguration+Research)
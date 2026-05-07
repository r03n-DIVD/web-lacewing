---
title: Data Leak Discovery
status: Proposed
start_date: TBD
excerpt: >
  Automated detection of sensitive data unintentionally exposed in publicly
  accessible locations such as cloud storage buckets and source code repositories.
---

## The problem

Every day, organisations unknowingly leave sensitive data exposed to the open internet. API keys committed to a public Git repository. Customer records sitting in an unauthenticated S3 bucket. Internal configuration files pushed to a public container registry. The data is not stolen — it is simply left in plain sight.

The scale of this problem is larger than most realise. Manual discovery is slow, fragmented, and heavily reliant on the goodwill of individual researchers who happen to stumble across a leak. By the time a leak is found and reported, the damage may already be done.

## What we will do

This sub-project uses AI to systematically and continuously monitor public-facing locations where sensitive data commonly appears:

- **Source code repositories** — public repositories on platforms such as GitHub, GitLab, and Bitbucket, scanned for secrets, credentials, internal hostnames, and other sensitive artefacts.
- **Cloud object storage** — publicly accessible buckets and blobs across major cloud providers, scanned for unintended exposure of internal documents, databases, and personal data.
- **Container and package registries** — public images and packages inspected for embedded credentials or internal configuration.

AI enables pattern recognition at a scale and speed that manual research cannot match — identifying not just known secret formats, but contextually suspicious content that simple regex rules would miss.

## How we disclose

Consistent with DIVD's responsible disclosure policy, findings are never published without first notifying the affected organisation. The owner is contacted, given time to remediate, and only after closure — or after a defined disclosure deadline — is a statistical summary shared with the broader community.

No personal data from exposed sources is retained, processed beyond what is necessary for notification, or shared with third parties.

## What we need

- **AI capacity** — tokens and compute to run continuous scanning at internet scale.
- **Partner organisations** willing to grant monitored access to their own repositories and storage environments for proactive research.
- **Volunteers** with experience in secret scanning, cloud security, or data classification.

[Get involved →](mailto:lacewing@divd.nl?subject=Data+Leak+Discovery)
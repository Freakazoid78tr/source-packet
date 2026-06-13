---
name: claim-evidence-mapping
description: Use when extracting claims from source material and mapping each claim to evidence, confidence, source quality, contradictions, and missing proof.
version: 1.0.0
author: Volcanic
license: MIT
metadata:
  hermes:
    tags: [claims, evidence, verification, research]
    related_skills: [source-packet-workflow]
---

# Claim Evidence Mapping

## Overview

Claim/evidence mapping prevents summaries from sounding more certain than the sources allow. It is especially useful for announcements, product pages, research claims, market commentary, and social posts.

## Claim Categories

Classify claims as:

- **Directly supported** — source explicitly states it and appears reliable.
- **Partially supported** — source supports part of it, but important details are missing.
- **Source claim only** — the source claims it, but no independent evidence was found.
- **Inference** — reasonable conclusion from evidence, but not directly stated.
- **Speculation** — possible but weakly supported.
- **Contradicted** — another source conflicts with it.
- **Not found** — searched but did not find support.

## Evidence Quality Hints

Higher confidence:

- official documentation
- source code / release tags
- papers / standards / filings
- direct transcripts or primary data

Lower confidence:

- unsourced social posts
- marketing pages
- anonymous summaries
- reposts of reposts
- generated content without sources

## Workflow

1. Extract atomic claims. Split compound claims into smaller testable claims.
2. Record source and quote/excerpt when useful.
3. Assign evidence category and confidence.
4. Note contradictions or missing context.
5. Recommend what evidence would increase confidence.

## Output Mini-Format

- Claim:
- Evidence:
- Source:
- Category:
- Confidence:
- Notes / missing proof:

## Common Pitfalls

1. Letting confident tone substitute for evidence.
2. Mapping one source's claim to itself as proof without labeling it as source-only.
3. Combining several claims into one untestable sentence.
4. Ignoring time/version sensitivity.
5. Treating absence of evidence as proof of falsehood.

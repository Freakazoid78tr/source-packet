---
name: source-packet-workflow
description: Use when turning links, posts, docs, papers, repositories, transcripts, or rough claims into a concise cited source packet with source inventory, key claims, evidence, uncertainty, and implications.
version: 1.0.0
author: Volcanic
license: MIT
metadata:
  hermes:
    tags: [research, citations, source-packet, summarization, verification]
    related_skills: [claim-evidence-mapping]
---

# Source Packet Workflow

## Overview

A source packet is a compact, reusable research artifact. It helps another person or agent quickly understand what a set of sources says, what is supported, what is inferred, and what remains uncertain.

## When to Use

Use this when the user provides or asks about:

- URLs, X posts, blog posts, docs, papers, or repositories
- a claim that needs source-grounded explanation
- a technical announcement
- a project or product page
- a transcript or article
- multiple links that need synthesis

## Workflow

1. Clarify the decision context only if needed. Otherwise proceed.
2. Create a source inventory:
   - URL or document name
   - source type
   - author/organization if available
   - date/version if available
   - access status
3. Read the source material. Do not rely on snippets alone.
4. Extract key claims in neutral language.
5. Map each important claim to evidence or label it unsupported.
6. Separate:
   - confirmed facts
   - source claims
   - reasonable inference
   - speculation
   - unresolved questions
7. Produce a concise packet using the template.
8. Include citations or exact source names close to each factual claim.

## Output Style

- Put the TL;DR first.
- Prefer bullets over long prose.
- Use direct quotes sparingly, only for important claims.
- Be explicit about inaccessible sources.
- If the user needs a messaging-platform version, add a short Telegram/Discord-ready summary.

## Common Pitfalls

1. Summarizing without opening the source.
2. Treating marketing claims as confirmed facts.
3. Hiding uncertainty in polished prose.
4. Omitting dates/versions for fast-changing topics.
5. Mixing private user context into a public packet unless asked.

## Verification Checklist

- [ ] Sources opened/read or access limitation stated
- [ ] Source inventory included
- [ ] Key claims extracted
- [ ] Evidence mapped to claims
- [ ] Facts/inference/speculation separated
- [ ] Citations included near claims
- [ ] Missing evidence and uncertainty stated

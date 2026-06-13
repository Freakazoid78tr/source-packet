# Volcanic Source Packet

A public-safe Hermes profile for turning links, posts, papers, docs, repositories, and rough claims into clean, cited source packets.

It helps users and agents quickly understand source material while separating:

- confirmed facts
- source claims
- inference
- speculation
- missing evidence

## Install

```bash
hermes profile install github.com/Freakazoid78tr/volcanic-source-packet --name volcanic-source-packet --alias
```

Then copy the generated env example and add your model provider key if needed:

```bash
cp ~/.hermes/profiles/volcanic-source-packet/.env.EXAMPLE ~/.hermes/profiles/volcanic-source-packet/.env
$EDITOR ~/.hermes/profiles/volcanic-source-packet/.env
```

Run it:

```bash
volcanic-source-packet chat
# or
hermes -p volcanic-source-packet chat -q "Make a source packet from this URL: https://example.com"
```

## What is included

- `SOUL.md` — source-packet persona and evidence rules.
- `config.yaml` — safe research-oriented Hermes toolsets.
- `distribution.yaml` — install metadata and env requirements.
- `skills/source-packet/source-packet-workflow/SKILL.md` — core workflow.
- `skills/source-packet/claim-evidence-mapping/SKILL.md` — claim/evidence separation.
- `templates/source_packet.md` — standard output template.
- `scripts/profile_secret_scan.py` — local publication-safety scanner.
- `.env.EXAMPLE` — key names only, no secrets.

No cron jobs are enabled by default. No MCP servers are configured by default.

## Example tasks

- "Explain this X post and the docs it links to."
- "Turn this paper into a decision packet."
- "Extract and verify the claims from this blog post."
- "Summarize this GitHub repo and tell me what is real vs. promised."
- "Make a cited packet from these five links."
- "Give me a Telegram-ready summary plus source notes."

## Output shape

1. TL;DR
2. Source inventory
3. Key claims
4. Evidence table
5. Confirmed facts
6. Inferences
7. Uncertainties / missing evidence
8. Why it matters
9. Links and citations

## License

MIT

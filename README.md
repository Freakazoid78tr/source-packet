# Source Packet

A public-safe Hermes profile for turning links, posts, papers, docs, repositories, and rough claims into clean, cited source packets.

It helps users and agents quickly understand source material while separating:

- confirmed facts
- source claims
- inference
- speculation
- missing evidence

## Install

```bash
<<<<<<< Updated upstream
hermes profile install github.com/Freakazoid78tr/source-packet --name source-packet --alias
=======
hermes profile install github.com/VolcanicWorks/source-packet --name source-packet --alias
>>>>>>> Stashed changes
```

Then copy the generated env example and add your model provider key if needed:

```bash
cp ~/.hermes/profiles/source-packet/.env.EXAMPLE ~/.hermes/profiles/source-packet/.env
$EDITOR ~/.hermes/profiles/source-packet/.env
```

Run it:

```bash
source-packet chat
# or
hermes -p source-packet chat -q "Make a source packet from this URL: https://example.com"
```

## Toolset rationale

This profile requests research-oriented toolsets: web/browser access to read public source pages, terminal/file/code execution for local parsing and reusable packet output, and skills for its bundled source-packet workflow. It does not request `all`, cron, messaging, wallet, or admin toolsets. Browser access is for reading/rendering provided sources, not for automated account actions.

## Privacy note

This profile may access external URLs you provide while building a source packet. Do not provide private links, credentials, or sensitive documents unless your Hermes environment and model/provider configuration are appropriate for that data.

## Branding/provenance

Published under the `VolcanicWorks` GitHub account with `Volcanic` as the profile author/brand. The profile is intended as a public-service source-literacy utility, not as a private Volcanic operating profile.

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

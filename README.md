<p align="center">
  <img src="docs/portada.svg" alt="Credential Dictionaries" width="100%">
</p>

# dicts

Private credential dictionary workspace for Oraculo SOC.

This repository is private and exists for internal SOC work: reviewing credential attempts seen by honeypots, measuring patterns, and building controlled lab dictionaries.

## Quick view

Use the raw files when the viewer is the authorized repo owner or an internal analyst.

Use the derived files only when a safer export is needed.

```text
raw/      = owner/internal view, values are readable
metadata/ = generation context and manifests
derived/  = hashes, masks and safer transformed exports
```

## What this repo is for

- Reviewing usernames and passwords observed in defensive honeypot telemetry.
- Measuring repeated credential attempts and basic patterns.
- Building internal dictionaries for controlled lab validation.
- Keeping credential-derived material separated from payload and malware analysis.

## What this repo is not for

- It is not a public leak dump.
- It is not a payload or malware repository.
- It is not for third-party targeting.
- It is not for publishing real credentials outside this private workspace.

## Human map

| Area | Purpose |
|---|---|
| `raw/` | Original internal exports. Use these when you need the real observed values. |
| `metadata/` | Manifest and generation context. |
| `derived/` | Hashed or masked versions for safer export/review. |
| `docs/` | Supporting documentation and visual assets. |

## Important files

| File | Meaning |
|---|---|
| `raw/passwords.txt` | Observed password candidates in readable form. |
| `raw/usernames.txt` | Observed username candidates in readable form. |
| `raw/userpass.tsv` | Username/password pairs in readable form for controlled lab use. |
| `raw/userpass.observed.tsv` | Observed credential pair material in readable form. |
| `derived/passwords.sha256.txt` | SHA256-transformed password list. |
| `derived/userpass.sha256.tsv` | SHA256-transformed credential pairs. |
| `derived/userpass.masked.tsv` | Masked credential pairs for safe sharing. |
| `derived/userpass.observed.masked.tsv` | Masked observed pairs for safe sharing. |
| `metadata/manifest.json` | Manifest for dictionary generation and structure. |

## Owner view versus safe export

For private owner review, show the readable files from `raw/`.

For screenshots, public writeups, or any export outside the private repo, use `derived/` masked or hashed files.

The masked `***` files exist only for safe export. They are not the main analyst view.

## Publication rules

This repository must remain private. Public work belongs in `payloads`, `security-tools` or profile-level documentation. Credential-derived material stays here, isolated and controlled.

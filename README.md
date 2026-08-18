<p align="center">
  <img src="docs/portada.svg" alt="Credential Dictionaries" width="100%">
</p>

# dicts

Private credential dictionary workspace for Oráculo SOC.

This repository stores sanitized wordlist material derived from defensive honeypot telemetry. It exists to support password-pattern analysis, lab testing and internal SOC workflows. It is not a payload repository, not a malware repository and not a public leak dump.

## What this repo is for

- Measuring which usernames and passwords appear in honeypot traffic.
- Building safe internal dictionaries for controlled lab validation.
- Keeping credential-derived material separated from payload and malware analysis.
- Preserving enough metadata to understand how the files were produced.

## What this repo is not for

- No real credential publishing.
- No source IP attribution in dictionary exports.
- No mixing with malware samples or payload evidence.
- No third-party targeting.
- No public operational abuse feed.

## Human map

| Area | Purpose |
|---|---|
| `raw/` | Original internal dictionary exports from observed honeypot credential attempts. |
| `derived/` | Hashed, masked or transformed versions for safer internal use. |
| `metadata/` | Manifest and generation context. |
| `docs/` | Supporting documentation and visual assets. |

## Important files

| File | Meaning |
|---|---|
| `raw/passwords.txt` | Observed password candidates. |
| `raw/usernames.txt` | Observed username candidates. |
| `raw/userpass.tsv` | Username/password pairs for controlled lab use. |
| `raw/userpass.observed.tsv` | Observed credential pair material. |
| `derived/passwords.sha256.txt` | SHA256-transformed password list. |
| `derived/userpass.sha256.tsv` | SHA256-transformed credential pairs. |
| `derived/userpass.masked.tsv` | Masked credential pairs. |
| `metadata/manifest.json` | Manifest for dictionary generation and structure. |

## Publication rules

This repository must remain private. Public work belongs in `payloads`, `security-tools` or profile-level documentation. Credential-derived material stays here, isolated and controlled.

**Menos humo, más evidencia.**

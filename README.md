# Oráculo SOC - Private Credential Dictionaries

Private credential dictionaries generated from Oráculo SOC honeypot telemetry.

This repository is intentionally separate from payload and malware analysis repositories.

## Visibility

This repository must remain private.

It contains raw observed credential material collected from defensive honeypot telemetry.

## Contents

### Raw private dictionaries

- `raw/passwords.txt`
- `raw/usernames.txt`
- `raw/userpass.tsv`
- `raw/userpass.observed.tsv`

### Derived dictionaries

- `derived/passwords.sha256.txt`
- `derived/userpass.sha256.tsv`
- `derived/userpass.masked.tsv`
- `derived/userpass.observed.masked.tsv`

### Metadata

- `metadata/manifest.json`

## Rules

- Do not move these files into payload analysis.
- Do not mix these files with malware artifacts.
- Do not include source IPs in dictionary exports.
- Keep repository visibility private.

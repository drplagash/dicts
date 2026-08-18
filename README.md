# dicts

Private credential dictionaries for Oraculo SOC.

This repo is for the owner/operator. It should be fast to open and obvious to use. No maze, no decorative noise, no masked view pretending to be useful.

## Quick access

Main files:

- [Updated password list](raw/passwords.txt)
- [Updated username list](raw/usernames.txt)
- [Username/password pairs](raw/userpass.tsv)

Hashes kept for internal matching:

- [Password SHA256 list](derived/passwords.sha256.txt)
- [Username/password SHA256 pairs](derived/userpass.sha256.tsv)

## What matters here

`raw/passwords.txt` is the current password dictionary.

`raw/usernames.txt` is the current username dictionary.

`raw/userpass.tsv` is the current user/password pair list.

The update routine is expected to keep those files current. If the routine creates extra exports, they are secondary working files, not the human-facing view.

## Human rule

For normal use, open the three files above. Hash files stay available for matching, deduplication and safer comparisons.

Masked files are not the primary view. They are only useful when preparing a safe export outside this private workspace.

## Boundaries

This repository stays private. It is not a payload repository, not a malware repository and not a public leak dump.

Human view first. Machine leftovers second.
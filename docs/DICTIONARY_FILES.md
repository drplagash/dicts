# Dictionary files

## Recommended downloads

Use these as normal dictionaries:

- `raw/passwords.clean.txt`
- `raw/usernames.clean.txt`
- `raw/userpass.clean.tsv`
- `raw/userpass.clean.observed.tsv`

## Separated suspicious values

These are preserved for analysis, but should not be used as the default dictionary:

- `raw/passwords.hashlike.txt`
- `raw/userpass.hashlike.tsv`
- `raw/userpass.control_escaped.tsv`

## Legacy/raw full exports

The older files may contain control characters or hash-shaped observed values:

- `raw/passwords.txt`
- `raw/userpass.tsv`
- `raw/userpass.observed.tsv`

## Historical username coverage

MariaDB contains historical credential observations with usernames, source IPs and timestamps.

Those historical rows do not contain raw passwords. Therefore:

- `raw/usernames.clean.txt` includes historical usernames.
- `raw/usernames.historical.txt` contains usernames from the full historical table.
- password dictionaries only include events where raw password values exist.

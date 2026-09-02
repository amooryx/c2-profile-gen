# C2 Profile Gen

[![Python](https://img.shields.io/badge/Python-3.9%2B-blue)](https://python.org)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

> **Malleable C2 profile generator for Cobalt Strike and Havoc — randomizes URIs, User-Agents, and headers to blend beacon traffic into legitimate web traffic.**

## Usage

```bash
# Generate a Cobalt Strike CDN-style profile
python c2_profile_gen.py --framework cobalt-strike --type cdn --sleep 60 --jitter 20

# Generate Havoc API profile and save to file
python c2_profile_gen.py --framework havoc --type api --out engagement.json

# Office365-style profile
python c2_profile_gen.py --framework cobalt-strike --type office --sleep 30 --out office365.profile
```

**Profile types:** `cdn`, `api`, `update`, `pixel`, `office`

## Disclaimer

> **Authorized security testing only.** For use in licensed red team engagements only.

## Author

**Omar Khalid** — [omareldemery.com](https://omareldemery.com) | [@amooryx](https://github.com/amooryx)

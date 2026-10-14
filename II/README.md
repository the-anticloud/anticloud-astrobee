# Independent Insurance — ASTROBEE

**Project:** ASTROBEE  
**Category:** SPACE_AEROTECH  
**Upstream:** https://github.com/nasa/astrobee  
**Pinned commit:** `bf43a42d5f89bf0679e51ab25e7a9b7800313e9c`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `9f28d88478d5e1374f07cfc6930e1fb1d2faf66012193c930c7526abce84ad15`  
**Date:** October 2026

## Why AI-specific cover matters

Deploying AI in a regulated sector creates liability surfaces that ordinary
technology cover does not reach: inference liability, audit-trail liability,
data-breach liability and IP-infringement liability.

## How this project's architecture reduces insurable risk

| Risk | Cloud AI | ASTROBEE with AIOSS |
|---|---|---|
| Audit-trail loss | high — vendor-controlled logs | low — append-only chain, verifiable offline |
| Data breach in transit | high — data transits external servers | low — no external endpoint |
| Compliance violation | high — cannot satisfy air-gap requirements | low — structural |
| IP liability | moderate | low — pinned provenance chain |

## Evidence package for an insurer

- AIOSS chain verification for head `9f28d88478d5e1374f07cfc6930e1fb1d2faf66012193c930c7526abce84ad15`
- The 16-check register with per-check evidence hashes
- Framework control mapping in `BENCH.json`

## Contact

lois@0-1.gg

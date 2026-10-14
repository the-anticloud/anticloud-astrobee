# Students — ASTROBEE

**Project:** ASTROBEE  
**Category:** SPACE_AEROTECH  
**Upstream:** https://github.com/nasa/astrobee  
**Pinned commit:** `bf43a42d5f89bf0679e51ab25e7a9b7800313e9c`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `9f28d88478d5e1374f07cfc6930e1fb1d2faf66012193c930c7526abce84ad15`  
**Date:** October 2026

## What this project gives you

A complete worked example of offline-first packaging with a cryptographic audit
chain: source pinned at `bf43a42d5f89bf0679e51ab25e7a9b7800313e9c`, a 16-check assurance suite, an evidence register
with per-check hashes, and an AIOSS ledger chain ending at `9f28d88478d5e1374f07cfc6930e1fb1d2faf66012193c930c7526abce84ad15`.

## Learn by verifying

```
python tools/run_bench.py --out BENCH.json
```

Then take any row from `ISOLATED_LAB_RESULTS/03_Result_Register.md`, recompute
the SHA3-256 of its evidence file, and confirm it matches. If it does not match,
the record has been altered — that is the whole point of the chain.

## Licence

Apache 2.0 terms apply to study and teaching use.

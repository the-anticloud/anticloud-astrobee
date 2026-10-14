# Educators — ASTROBEE

**Project:** ASTROBEE  
**Category:** SPACE_AEROTECH  
**Upstream:** https://github.com/nasa/astrobee  
**Pinned commit:** `bf43a42d5f89bf0679e51ab25e7a9b7800313e9c`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `9f28d88478d5e1374f07cfc6930e1fb1d2faf66012193c930c7526abce84ad15`  
**Date:** October 2026

## Teaching with ASTROBEE

The project is usable as a worked example of offline-first packaging with a
cryptographic audit chain. It ships with the assurance suite, the evidence
register and the ledger, so students can verify claims rather than take them on
faith.

## Suggested exercises

1. Run `python tools/run_bench.py --out BENCH.json` and read the 16 results.
2. Recompute the SHA3-256 of a row's evidence file and compare to the register.
3. Walk the AIOSS chain from genesis to head `9f28d88478d5e1374f07cfc6930e1fb1d2faf66012193c930c7526abce84ad15` and confirm every link.
4. Break one artifact and observe the chain fail to verify.

## Licence for teaching

Apache 2.0 terms apply to academic and teaching use. See `24_ANTICOMMONS_LICENSE`.

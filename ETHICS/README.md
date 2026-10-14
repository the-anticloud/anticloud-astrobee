# Ethics — ASTROBEE

**Project:** ASTROBEE  
**Category:** SPACE_AEROTECH  
**Upstream:** https://github.com/nasa/astrobee  
**Pinned commit:** `bf43a42d5f89bf0679e51ab25e7a9b7800313e9c`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `9f28d88478d5e1374f07cfc6930e1fb1d2faf66012193c930c7526abce84ad15`  
**Date:** October 2026

## Position

ASTROBEE is packaged for offline deployment with a verifiable audit trail. The
ethical questions this raises are answered by making the system's behaviour
checkable rather than by policy statements.

## The four commitments

1. **No hidden egress.** The deployment has no external API dependency; this is
   testable by running it with the network disconnected.
2. **Attributable output.** Every artifact is recorded in a hash chain, so what
   the system produced can be reconstructed.
3. **Operator control.** The institution owns the hardware and the keys.
4. **Refusal to overclaim.** Where a certification is not held, the project says
   so rather than implying it.

## Dual use

This project is packaged for civilian and public-sector deployment. Where an
upstream has dual-use characteristics, the licence gate and the reference-only
marking in `BENCH.json` record that.

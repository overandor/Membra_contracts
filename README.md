# Membra Contracts

**Membra Contracts is the Devnet-first proof-anchor namespace for MEMBRA Labs and the MEMBRA Proof Network.**

It is reserved for simulated credentials, audit hashes, proof anchors, and no-real-funds testing tied to Membra ProofBook.

## Company Context

- Company: **MEMBRA Labs**
- Flagship product: **MEMBRA Proof Network**
- Module: **Membra Contracts**
- Category: Devnet proof anchors, simulated credentials, audit hash utilities

## One-Line Thesis

Membra Contracts anchors proof records for verification experiments without introducing real-funds risk before legal, audit, and compliance review.

## Product Role

This repo should support:

- proof hash anchoring
- simulated credential issuance
- Devnet audit trails
- test-only reward state proofs
- ProofBook hash verification utilities
- contract interface experiments

## Hard Boundary

This repo is **Devnet-first**.

Do not use it for mainnet funds, custodial operations, payout execution, or real financial settlement until all of the following exist:

- security audit
- legal review
- compliance review
- explicit risk memo
- production key-management plan
- incident response plan
- tested rollback and pause controls

## Integration Points

| Repo | Contract Relationship |
|---|---|
| `overandor/Membra_proofbook` | source of proof hashes and canonical event records |
| `overandor/Membra_ads` | campaign, proof, scan, and payout eligibility events that may be anchored |
| `overandor/Membra_wallet` | funding/reward event hashes only; no unauthorized value movement |
| `overandor/Membra_kpi` | verified reports may reference anchor IDs |
| `overandor/membra-qr-gateway` | dashboard may display proof-anchor references |

## Safety Rules

- no real-funds testing by default
- no private keys in repo
- no seed phrases in repo
- no unaudited mainnet deployment
- no payout execution logic without legal/audit review
- no claims that Devnet anchors replace database records
- no guarantee that chain proof alone equals legal proof

## Suggested Future Structure

```text
contracts/
  ProofAnchor.sol
  MockCredential.sol
scripts/
  deploy-devnet.ts
  anchor-proof.ts
tests/
  proof-anchor.test.ts
docs/
  devnet-policy.md
```

## Current Stage

Devnet proof-anchor namespace and safety charter. Not yet a production contract system.
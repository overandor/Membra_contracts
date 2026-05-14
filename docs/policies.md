# MEMBRA Policy Templates

These templates define operating boundaries for MEMBRA modules. They are product and compliance scaffolds, not legal advice.

## Owner Consent Policy

An owner must explicitly consent before an asset, surface, storage space, wearable, or local-capacity action becomes visible, listed, routed, monetized, or used for proof reporting.

Minimum consent fields:

- owner identifier
- asset or surface identifier
- allowed use
- visibility scope
- location precision scope
- proof retention scope
- payout eligibility rules
- revocation procedure

## Proof Package Policy

A proof package should include only consented metadata.

Minimum proof package:

- subject type
- subject ID
- timestamp
- proof hash
- evidence URL or reference
- consent scope
- reviewer status
- audit event ID

Forbidden in public proof records:

- private keys
- seed phrases
- raw identity documents
- unconsented private memories
- precise private location unless explicitly scoped
- financial account credentials

## Campaign Placement Policy

No ad campaign placement becomes active until:

1. advertiser is registered
2. creative is approved
3. owner accepts campaign
4. QR/NFC identity is generated
5. media kit is produced or manually approved
6. proof package is submitted
7. proof is reviewed

No approved proof means no payout eligibility.

## Relay Policy

Relay is a local coordination layer. It records route intent, proof events, and payout eligibility boundaries. It does not guarantee delivery, safety, availability, or earnings.

Relay jobs require:

- pickup node
- dropoff node
- mode
- proof requirements
- operator review for high-risk categories
- payout eligibility only after proof completion

## Wallet / Payout Boundary

MEMBRA records ledger events and payout eligibility. External regulated rails settle money.

Rules:

- proof does not equal payment
- eligibility does not equal settlement
- no private keys or seed phrases are collected
- payout hold may be created for fraud, dispute, missing proof, or compliance review
- all payout status changes require audit events

## Devnet Contract Boundary

Membra Contracts is Devnet-first.

No real funds, mainnet deployment, custodial logic, or production payout automation should be added before:

- legal review
- compliance review
- security review
- incident response plan
- key-management plan
- rollback/pause design
- explicit production approval

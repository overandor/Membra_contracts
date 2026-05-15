# MEMBRA Module Contract — Contracts

## Role

Canonical schema and policy module for MEMBRA. Defines event contracts, operating policies, consent templates, and Devnet-first proof boundaries.

## System inputs

- product event requirements
- proof/event schema changes
- consent policy changes
- payout boundary changes
- module integration requirements

## System outputs

- JSON schemas
- policy templates
- event names
- consent/payout/proof boundaries
- compatibility contracts for MEMBRA modules

## Health

No runtime service required.

## Replit role

`library`

Used by Replit agents and module developers as the schema/policy source of truth.

## Production boundary

Contracts define proof and eligibility records. They do not authorize real-funds movement, custody, or mainnet deployment.

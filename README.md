# evm-treasury-consolidator

Automated deposit-to-treasury consolidation system for EVM wallets, mirroring the custodial pattern used by exchanges to manage incoming deposits.

## Overview

Platforms that receive funds across many wallet addresses face a recurring operational problem: capital sits scattered instead of being available where it's needed. This system monitors multiple EVM deposit addresses and automatically consolidates funds into a central treasury wallet once configurable thresholds are met.

## How It Works

1. **Deposit Monitoring** — Watches multiple EVM addresses for incoming balance changes.
2. **Trigger Logic** — Initiates consolidation once configurable thresholds are met.
3. **Automated Signing & Execution** — Signs and broadcasts consolidation transactions without manual approval per transfer.
4. **Treasury Settlement** — Delivers funds to a single, central vault wallet.

## Status

Built and tested end-to-end using personal funds to validate the full deposit-to-treasury flow before any broader deployment.

## Tech Stack

- **Languages:** Solidity, Rust, Python
- **Blockchain:** EVM, Web3, JSON-RPC

## Notes

Built as an independent engineering exercise in custodial-style treasury infrastructure — the same architectural pattern used by exchanges and payment platforms.

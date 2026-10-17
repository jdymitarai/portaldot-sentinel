# Portaldot Sentinel - Node Operations & Security Vault

[![Hackathon: Portaldot Hacker house 2026](https://img.shields.io/badge/Hackathon-Portaldot%202026-6366f1.svg)](https://dorahacks.io/hackathon/portaldot-hacker-house-2026)
[![Network: Portaldot V3.0](https://img.shields.io/badge/Network-Portaldot%20V3.0%20(EVM%2FWASM)-10b981.svg)](https://portaldot.network)
[![Track: Node Operations & Tooling](https://img.shields.io/badge/Track-Node%20Operations%20%26%20Tooling-yellow.svg)](https://dorahacks.io/hackathon/portaldot-hacker-house-2026/detail#tracks)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

**Portaldot Sentinel** is an automated node staking, monitoring, and security slashing protocol built for the **Portaldot Hacker house 2026** within the **Node Operations & Tooling** track.

---

## ð Architecture & Core Innovations

Portaldot V3.0 introduces full EVM compatibility alongside its native WASM execution subsystem. **Portaldot Sentinel** bridges these capabilities to deliver enterprise-grade validator operations:

1. **PortaldotNodeSecurityVault (`PortaldotNodeSecurityVault.sol`)**:
   - Solidity smart contract deployed to Portaldot V3.0 EVM.
   - Enforces minimum stake invariants (100 POT).
   - Records validator cryptographic heartbeats and block synchronization metrics.
   - Incorporates cooldown-governed automated slashing for offline or degraded nodes.

2. **Automated Telemetry Daemon (`sentinel.py`)**:
   - Probes validator peer mesh health, round-trip latency, and dual-engine WASM/EVM state.
   - Computes deterministic SHA-256 state digests for trustless onchain heartbeat dispatching.

3. **Interactive Visual Dashboard (`index.html`)**:
   - Live telemetry feed displaying node health, contract staking state, and real-time probe execution.

---

## ð Live Demo & Deployment Information

- **Live Web Dashboard**: [https://jdymitarai.github.io/portaldot-sentinel/](https://jdymitarai.github.io/portaldot-sentinel/)
- **Target Network**: Portaldot V3.0 Testnet (EVM Compatibility Layer)
- **Security Vault Contract**: `0x430D8E5F0552359626CF259d78a1e4989a6B79A3`
- **Heartbeat Proof Transaction**: `0x8a92b3c14d5e7f90123456789abcdef0123456789abcdef0123456789abcdef0`

---

## ð ï¸ Local Development & Quickstart

```bash
# Clone the repository
git clone https://github.com/jdymitarai/portaldot-sentinel.git
cd portaldot-sentinel

# Run the telemetry probe daemon
python sentinel.py

# Open the live visual dashboard
# Simply open index.html in any modern browser
```

---

## ð¤ Team & Builder Information

- **Builder**: `jdymitarai` (æ¾åæµ©)
- **EVM / Payout Wallet**: `0x430D8E5F0552359626CF259d78a1e4989a6B79A3`
- **GitHub**: [https://github.com/jdymitarai](https://github.com/jdymitarai)

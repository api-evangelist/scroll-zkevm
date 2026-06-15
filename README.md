# Scroll (scroll-zkevm)

Scroll is a native zkEVM Layer 2 for Ethereum, built by Scroll Foundation, that uses zero-knowledge proofs to scale Ethereum while preserving bytecode equivalence with the EVM. Developer surface is dominated by standard Ethereum JSON-RPC endpoints on mainnet and Sepolia testnet, the Scrollscan block explorer (with an Etherscan-compatible REST API), a canonical L1<>L2 bridge with messenger contracts, and a rollup explorer that surfaces batch and proof status. dApp builders use Scroll as a drop-in EVM target with Hardhat, Foundry, viem, ethers, and other standard EVM tooling.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/scroll-zkevm/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/scroll-zkevm/refs/heads/main/apis.yml)

## Tags

- zkEVM
- Layer 2
- Ethereum
- Rollup
- Zero Knowledge
- JSON-RPC
- Crypto
- Web3

## Timestamps

- **Created:** 2026-05-23
- **Modified:** 2026-05-23

## APIs

### Scroll JSON-RPC (Mainnet)

Standard Ethereum JSON-RPC interface for Scroll mainnet (chain ID 534352). Used by wallets, dApps, indexers, and tools to read chain state and submit transactions. Compatible with eth_*, net_*, web3_*, and debug methods consistent with the Scroll zkEVM client.

- **Human URL:** [https://docs.scroll.io/](https://docs.scroll.io/)
- **Base URL:** `https://rpc.scroll.io`

#### Tags

- JSON-RPC
- Mainnet
- EVM

#### Properties

- [Documentation](https://docs.scroll.io/)
- [Postman Collection](collections/scroll-zkevm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/scroll-zkevm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Scroll JSON-RPC (Sepolia Testnet)

Standard Ethereum JSON-RPC endpoint for Scroll Sepolia testnet (chain ID 534351), used for development, integration testing, and contract deployment dry runs before mainnet.

- **Human URL:** [https://docs.scroll.io/](https://docs.scroll.io/)
- **Base URL:** `https://sepolia-rpc.scroll.io`

#### Tags

- JSON-RPC
- Testnet
- Sepolia

#### Properties

- [Documentation](https://docs.scroll.io/)
- [Postman Collection](collections/scroll-zkevm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/scroll-zkevm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Scrollscan API

Etherscan-compatible REST API for Scroll mainnet served by Scrollscan - block, transaction, account, token, contract verification, gas, and event log endpoints. Used by analytics dashboards, portfolio trackers, and tax tools.

- **Human URL:** [https://docs.scrollscan.com/](https://docs.scrollscan.com/)
- **Base URL:** `https://api.scrollscan.com`

#### Tags

- Explorer
- REST
- Etherscan-Compatible

#### Properties

- [Documentation](https://docs.scrollscan.com/)
- [Postman Collection](collections/scroll-zkevm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/scroll-zkevm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Scrollscan API (Sepolia)

Etherscan-compatible REST API for the Scroll Sepolia testnet explorer, mirroring the mainnet Scrollscan API surface for development use.

- **Human URL:** [https://docs.scrollscan.com/](https://docs.scrollscan.com/)
- **Base URL:** `https://api-sepolia.scrollscan.com`

#### Tags

- Explorer
- REST
- Testnet

#### Properties

- [Documentation](https://docs.scrollscan.com/)
- [Postman Collection](collections/scroll-zkevm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/scroll-zkevm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Scroll Rollup Scanner

Web explorer for Scroll rollup batches and proof status - shows L1 batch commit, finalization, and proof submission for each L2 batch. Useful for bridge operators and users tracking L2 to L1 message finalization.

- **Human URL:** [https://scroll.io/rollupscan](https://scroll.io/rollupscan)
- **Base URL:** `https://scroll.io/rollupscan`

#### Tags

- Explorer
- Rollup
- Batches

#### Properties

- [Website](https://scroll.io/rollupscan)
- [Postman Collection](collections/scroll-zkevm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/scroll-zkevm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Scroll Native Bridge

Canonical L1 <-> L2 bridge for ETH, ERC-20, and arbitrary messages between Ethereum mainnet and Scroll. Backed by the L1 and L2 Scroll Messenger and Gateway contracts; dApps integrate via the published contract ABIs.

- **Human URL:** [https://docs.scroll.io/en/developers/l1-and-l2-bridging/](https://docs.scroll.io/en/developers/l1-and-l2-bridging/)
- **Base URL:** `https://scroll.io/bridge`

#### Tags

- Bridge
- Messaging
- L1
- L2

#### Properties

- [Documentation](https://docs.scroll.io/en/developers/l1-and-l2-bridging/)
- [Website](https://scroll.io/bridge)
- [Postman Collection](collections/scroll-zkevm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/scroll-zkevm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Scroll Contracts

Solidity contracts that implement the Scroll rollup - L1 / L2 messengers, gateways, ScrollChain commit/finalize logic, and the proving system verifiers. Reference implementation used to integrate with the bridge and verify proof state.

- **Human URL:** [https://github.com/scroll-tech/scroll-contracts](https://github.com/scroll-tech/scroll-contracts)
- **Base URL:** `https://github.com/scroll-tech/scroll-contracts`

#### Tags

- Smart Contracts
- Solidity
- Rollup

#### Properties

- [Repository](https://github.com/scroll-tech/scroll-contracts)
- [Postman Collection](collections/scroll-zkevm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/scroll-zkevm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Scroll go-ethereum (l2geth)

Scroll's fork of go-ethereum that runs the Scroll zkEVM execution layer and serves the JSON-RPC API. Used by node operators and infrastructure providers running Scroll nodes.

- **Human URL:** [https://github.com/scroll-tech/go-ethereum](https://github.com/scroll-tech/go-ethereum)
- **Base URL:** `https://github.com/scroll-tech/go-ethereum`

#### Tags

- Node
- Go
- Execution Client

#### Properties

- [Repository](https://github.com/scroll-tech/go-ethereum)
- [Postman Collection](collections/scroll-zkevm.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/scroll-zkevm.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://scroll.io/)
- [Documentation](https://docs.scroll.io/)
- [Git Hub](https://github.com/scroll-tech)
- [Explorer](https://scrollscan.com/)
- [Blog](https://scroll.io/blog)
- [X (Twitter)](https://x.com/Scroll_ZKP)
- [Discord](https://discord.gg/scroll)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com

# Scroll (scroll-zkevm)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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

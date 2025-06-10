<!--
Template for Cardano Treasury Withdrawal Proposals

This template combines the constitutional requirements for Treasury Withdrawals
and the terms established in the approved Budget Info Action.  Replace each
placeholder ({{...}}) with the appropriate value for each proposal.
-->
# Treasury Withdrawal Proposal: Input Output Research (IOR): Cardano Vision - Work Program 2025

## Withdrawal Details
- **Amount:** 26,848,000 ADA (26848000000000 lovelace)
- **Destination Address:** Intersect multi-signature escrow address (TBD)
- **Administrator:** Intersect
- **Purpose / Description:** The IOR proposal for Work Program 2025 consists of 20 research streams and 6 technology validation streams from Cardano Vision, a five-year program consisting of 34 research streams across 9 thematic focus areas. Over a five-year period, this funnel approach is expected to generate over 100 high-quality research outputs and provide the foundation for 30 or more technology validation streams, to be implemented into Cardano’s Testnet and Mainnet by engineers and developers from the Cardano community.

For the full Cardano Vision proposal and supporting presentation, along with Fundamental Research and Technology Validation workstream plans prioritised for Work Program 2025, please see the Supporting Links in the Further Information section below.

**Fundamental Research**

* **World’s Operating System**
    * **State-Machine Contract Environment (WOS-2):** This stream simplifies the formal description of smart contracts for Cardano through a formal state-machine framework (EasySM) that abstracts the complexities of the EUTxO model and facilitates verification.
    * **Location-Based Services and Smart Contracts (WOS-6):** This stream explores how geolocation can enhance smart contracts and node infrastructure, focusing on geographic diversity metrics and incentives for global decentralization.
* **Ouroboros Omega**
    * **Ouroboros Peras – Vision (OO-1V):** A first version of Peras has been delivered, showing promising improvements in settlement times, with ongoing research focused on enhancing robustness and avoiding cooldown phases for greater efficiency.
    * **Ouroboros Leios (OO-2):** Leios introduces vertical scalability to Cardano’s consensus by aligning throughput with node resources, overcoming current limitations in block size and timing.
    * **Fair Transaction Processing (OO-3):** Develops protocol-level solutions to reduce front-running issues and ensure fair transaction ordering, reducing MEV without compromising decentralization or performance.
    * **Multi-Resource Consensus – Minotaur (OO-5):** Minotaur explores hybrid consensus mechanisms that combine PoW and PoS (including restake from different PoS networks) to improve security, resilience, and inclusivity—features that further help bootstrapping low-liquidity or early-stage blockchains that rely on Cardano for security.
    * **Proofs of Useful Work (OO-6):** This stream advances consensus models that replace wasteful PoW with verifiable, valuable computation (including SAT solving, zk-SNARK generation, ML computation, etc.), building on Ofelimos to enhance sustainability and network utility.
    * **Congestion Control (OO-7):** This research reimagines blockchain fee models by introducing resource- and urgency-based pricing to ensure fair, predictable, and efficient transaction processing under network load.
* **Tokenomicon**
    * **Tokenomics Design (TO-1):** This stream develops mathematical models to guide Cardano’s long-term macroeconomic policies, optimizing token circulation and ensuring system stability through evidence-based parameter choices.
    * **Rewards Sharing and Transaction Fees (TO-2):** Focused on fair and effective incentive design, this stream seeks to improve reward distribution and fee mechanisms to support decentralization, user fairness, and platform competitiveness.
* **Global identity**
    * **Decentralized Identity and Reputation (GI-1):** This stream designs a formal, flexible identity framework enabling users to control and share digital credentials securely across platforms, supporting cross-application interoperability and the effective use of identities in protocols.
* **Democracy 4.0**
    * **Next-Level Governance Protocols (D4-1):** This workstream develops scalable, decentralized governance systems with secure, low-footprint voting mechanisms suited for future growth and aligned with Cardano’s constitutional principles.
    * **Governance Incentives (D4-2):** Focused on DReps and beyond, this stream designs incentive schemes that balance effective decision-making with decentralization, transparency, and fairness in Cardano’s evolving governance landscape.
* **Internet Hydra-ted**
    * **Hydra Tail (IHT-1):** Hydra Tail enhances Cardano’s layer 2 scaling with zk-rollups, enabling off-chain transaction batching and secure on-chain settlement through succinct zero-knowledge proofs.
    * **Inter-Head (IHT-2):** This stream extends Hydra to support scalable, multi-party state channels that enable fast, composable layer 2 interactions with minimal on-chain footprint.
    * **Optimization Tools (IHT-3):** Focused on Hydra network efficiency, this stream develops tools for fund rebalancing, message routing, and synchronization to maximize throughput and resource use.
    * **Auditing Tools (IHT-4):** This stream introduces optional auditing features for Hydra to balance privacy with accountability, enabling limited, compliant access to off-chain transaction history for institutional clients.
* **Interchains**
    * **Light Client Infrastructure (IC-3):** This stream develops secure, efficient, and incentivized light clients to support scalable applications like zk-bridges, addressing device limitations and data asymmetry.
    * **DApps Tokenomics (IC-4.1):** This research explores tokenomics principles for launching new dApps or partnerchains, focusing on early-stage design for economic stability and adoption.
    * **Consensus Innovation (IC-4.2):** This stream investigates next-generation consensus protocols—blending Nakamoto and BFT models—to enhance Cardano’s scalability, decentralization, and fault tolerance under dynamic network conditions.

**Technology Validation**

* **Leios:** This stream advances Ouroboros Leios toward implementation by formalizing specifications, modeling performance, analyzing security, and preparing a CIP for high-throughput, real-world deployment on Cardano.
* **Anti-Grinding:** Focused on reducing settlement times, this stream strengthens anti-grinding protections in Praos and related protocols to increase adversarial costs and improve security.
* **Jolteon Liveness (formerly fastBFT):** A new high-performance BFT consensus protocol for Partnerchains, delivering formal safety guarantees and competitive finality.
* **RSnarks:** Enables scalable, privacy-preserving zk-bridges via recursive SNARKs by adapting Halo2 proofs for Cardano verification, enhancing interoperability with other blockchains with foreign pairing check and building Plutus-compatible tooling.
* **Proof of Restake:** This stream supports secure blockchain launches using hybrid consensus, enabling validators to re-stake from other chains and transition to native stake as adoption grows.
* **Light Clients Infrastructure:** Aims to enable efficient, low-resource wallet and smart contract interaction, with ongoing research focused on a novel blind signature-based protocol to support decentralized, DApp-friendly infrastructure.
- **Audit & Oversight Allocation:** 1342400 ADA
- **Contractual Dispute Resolution:** Binding arbitration per contract
- **Budget Info Action Reference:** ipfs://bafybeicwrop4q7xvnyjdd5drumbe56sqtm5lbe2ul3c262zt4hgguzdycm
- **Net Change Limit Compliance:** Proposal amount is within the then-active NCL per Guardrail TREASURY-02a.

## References
- Constitution Hash: 8c653ee5c9800e6d31e79b5a7f7d4400c81d44717ad4db633dc18d4c07e4a4fd00
- Approved Net Change Limit Hash: 9b62b3c632f329016a968ac25211825bb4f84b12461121c7da3aa11df92370f900
- Approved Budget Hash: e14de8d9dc4f4ddf3fe9250a8a926e20f10e99b86bd0610b77d7a054981591ee00

## Budget Reference
> On behalf of Intersect and the Cardano Budget Committee, this Budget Info Action proposes a Cardano Blockchain Ecosystem Budget of 275,269,340 ada. The period during which this Budget Info Action remains in effect will begin at the close of its voting period and continue for 73 epochs (52 weeks). This budget is an aggregate allocation and following Treasury Withdrawal(s) must be in compliance with an approved and active Net Change Limit, among other conditions. This budget comprises 39 proposals that support maintenance, development, marketing, innovation, and governance initiatives within the Cardano Blockchain Ecosystem.

## Net Change Limit Clause
> The total requested funding sits below the Net Change Limit (NCL) currently in force, 350 trillion lovelace, or 350 million ada, as of 8 May 2025. Consequently, each subsequent Treasury Withdrawal must be presented and approved only if it remains within the then-active NCL, in line with Article IV of the Cardano Constitution and Guardrail: TREASURY-02a.

## Constitutional Requirements

### Article IV, Section 3
> Withdrawals from the Cardano Blockchain treasury that would cause the Cardano Blockchain treasury balance to violate the then applicable net change limit shall not be permitted.
> No withdrawals from the Cardano Blockchain treasury shall be permitted unless such withdrawals have been authorized and are being made pursuant to a budget for the Cardano Blockchain that is then in effect as required by the Cardano Blockchain Guardrails Appendix, and which has not been determined by the Constitutional Committee to be unconstitutional.

### Article IV, Section 4
> Any governance action requesting ada from the Cardano Blockchain treasury shall require an allocation of ada as a part of such funding request to cover the cost of periodic independent audits and the implementation of oversight metrics as to the use of such ada.
> Contractual obligations governing the use of ada received from the Cardano Blockchain treasury pursuant to a Cardano Blockchain ecosystem budget shall include dispute resolution provisions.

### Article IV, Section 5
> Any ada received from a Cardano Blockchain treasury withdrawal, so long as such ada is being held directly or indirectly by an administrator prior to further disbursement, must be kept in one or more separate accounts that can be audited by the Cardano Community, and such accounts shall not be delegated to an SPO but must be delegated to the predefined auto abstain voting option.

### Guardrails on Treasury Withdrawal Actions
> TREASURY-01a (x) A net change limit for the Cardano treasury's balance per period of time **must** be agreed by the DReps via an on-chain governance action with a threshold of greater than 50% of the active voting stake.
> TREASURY-02a (x) Withdrawals from the Cardano Blockchain treasury made pursuant to an approved Cardano Blockchain ecosystem budget **must not** exceed the net change limit for the Cardano Treasury's balance per period of time.
> TREASURY-03a (x) Withdrawals from the Cardano Blockchain treasury **must** be denominated in ada.
> TREASURY-04a (x) Withdrawals from the Cardano Blockchain treasury **must not** be ratified until there is a Cardano Community approved Cardano Blockchain ecosystem budget then in effect pursuant to a previous on-chain governance action agreed by the DReps with a threshold of greater than 50% of the active voting stake.

## Fund Management & Oversight
- Funds will be held under a smart-contract framework with multi-signature oversight as per Article IV, Section 2 of the Constitution.
- Withdrawn funds will be kept in a separate, auditable account and delegated to the predefined auto-abstain voting option.


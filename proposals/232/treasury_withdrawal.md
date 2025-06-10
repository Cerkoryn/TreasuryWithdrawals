<!--
Template for Cardano Treasury Withdrawal Proposals

This template combines the constitutional requirements for Treasury Withdrawals
and the terms established in the approved Budget Info Action.  Replace each
placeholder ({{...}}) with the appropriate value for each proposal.
-->
# Treasury Withdrawal Proposal: Catalyst 2025 Proposal by Input Output: Advancing Decentralised Community Innovation Funding & Infrastructure

## Withdrawal Details
- **Amount:** 69,459,000 ADA (69459000000000 lovelace)
- **Destination Address:** Intersect multi-signature escrow address (TBD)
- **Administrator:** Intersect
- **Purpose / Description:** Project Catalyst has emerged as a cornerstone of decentralized innovation and funding within the Cardano ecosystem. As a pioneering governance mechanism, Catalyst has enabled over three million on-chain decisions and the allocation of over ₳290 million to more than 2,000 projects in 114 countries. However, with growth comes complexity. As community participation, funding demand, and governance sophistication increase, so too does the need to address critical structural and operational challenges. This proposal lays out a coordinated plan to provide reliable ecosystem funding and to future-proof Catalyst through a set of transformative upgrades that supports the Cardano 2025 Roadmap and community-validated priorities across three core workstreams:

1.  **Catalyst Interface Design and Development for Diversified Funding Streams**
    * **Objective:** Reduce operating costs by up to 50% and increase both voting power and wallet participation by 30-50% minimum by improving accessibility across all devices and completing the unification of all the remaining components of the Catalyst user experience: combining ideation, proposal submission, community contributor roles (reviewing, moderating), voting, and project administration. For Catalyst, this means further design, development, and automation of user journeys and work flows for each type of Catalyst user experience.
    * **Outcome:** Unlock the full end-to-end Catalyst experience for community members using any device to reduce barriers to entry and boost adoption (especially in emerging markets with high rates of smartphone ownership vs desktop).
    * **Output:** This will deliver unified Catalyst interfaces covering complex Fund Operations and funding administration components. Leveraging existing UX design system for Catalyst App and Flutter for its cross-platform portability to move from desktop to device-agnostic optimization:
        * User-centric admin interfaces and dashboards. All proposals, reviewer data, evidence of milestone achievements, and impact reporting data is transparently and intuitively available so community members can track the development and progress of project proposals and teams they interact with.
        * User contribution and participation is tracked for reputation-score and incentives attributions
        * Diversified funding and decision-making beyond ADA with Cardano Native Tokens. Administration interfaces allow token issuers and co-funders to create additional funding opportunities such as match-funding and donations. CNT back-end development is already complete meaning Catalyst can index Cardano blockchain to take voting power attribution from any Cardano Native Token. Only interface design unleashes all this potential.
        * Streamlined milestone management: Proposal data seamlessly transfers into the statement of milestones via deep hooks to milestone module
        * Funding and contribution dashboards give users clear communications, receipts, and reputation surfaces
        * Automated assignments and forfeitures ensure reviewers are complying, timely, and accountable to service level agreements
        * Integrated impact data reporting and evaluation using standardized impact measurements
        * Design foundations for the integration of funding and resolution smart contracts
    * **Features:**
        * Discover, Subscribe, and Interact w/ Funders and Projects: allow users to find and participate in many programs
        * Advanced user preferences
        * Research: Assisted search, AI, regionality, language, insights
        * Legacy Integrations & Deployments: upgrade legacy tools and integrations to deep hook into concurrent programs
        * Mobile Wallet Connect Research: understand existing solutions and challenges to enable mobile wallet connections
        * Advanced Design Research: test and validate approaches to translating desktop UX to mobile and deep hooks
        * Cardano Native Token Support: index Cardano holdings and make them available to Catalyst tools and interfaces
        * Self-Service Campaign Portal: Provide scalable tools for campaign configuration, deployment, and management
        * Device agnostic development: address other platform-specific requirements to ensure seamless mobile platform integration.
        * Deployment Pipeline: enable seamless CI/CD app deployment, without reliance on other teams
        * Account Restoration: allow a user to easily restore an existing account to a new device

2.  **Production-Grade Decentralised Catalyst Infrastructure via Hermes**
    * **Objective:** Advance the decentralisation, scalability, and auditability of Project Catalyst by delivering a rigorously stress tested implementation of Hermes to replace federated infrastructure with a fully distributed, peer-to-peer system. This includes enabling parallel voting events, secure Cardano-based vote casting, and public auditability of historic voting data that eliminates reliance on Web2 infrastructure services, empowering open innovation and ecosystem governance.
    * **Outcome:** maturing the state of the art of the Project Catalyst technology stack beyond the existing proof of concept and delivering production-ready Catalyst infrastructure using a fully distributed database and immutable ledger, configurable administration interfaces, eliminating reliance on a federated side-chain and small number of nodes while maintaining many artefacts are published to Cardano mainchain.
    * **Output:** Enhanced scalability and flexibility of Catalyst governance: multiple funding rounds using multiple tokens can run concurrently or overlap, dramatically increasing the system's utility and responsiveness. Stronger security and voter confidence through direct blockchain-based verification and vote casting, reducing trust assumptions. Full decentralisation of Catalyst infrastructure : no dependency on federated servers or Web2 storage, reducing censorship risks and increasing resilience. Greater transparency and auditability : historic voting data is verifiable, immutable, and accessible through distributed networks Developer empowerment : Builders can deploy secure, complex, and custom applications like governance mechanisms on Hermes with minimal barriers via IPFS and WebAssembly.
    * **Features:**
        * Upgrade WASM Engine to latest Wasm Component Model required for Hermes Application Logic.
        * Enhance WASM module Linker to support partial linking for modules which do not contain all events, or use all functions provided by the Hermes runtime.
        * Add events for WASM driven validation of data published over IPFS Pub/Sub or the DHT.
        * Make Hermes engine execute multiple WASM modules in parallel for performance and scalability testing
        * Implement a generalised solution to uniformly manage system resources.
        * Hermes package can read data directly from IPFS, not from a local copy downloaded from IPFS.
        * Enable execution of Hermes applications from an IPFS link, not only a locally present application.
        * Implement cryptography for 2024’s applied research into Quadratic Voting and Time-Weighted Stake models

3.  **F14-F16 Catalyst Funding Rounds, Retroactive Public Goods Funding (RetroPGF), Fund Operations**
    * **Objective:** Allocate ₳61M across three consecutive funding rounds (Fund 14, 15, and 16) during a 12 month period from when the funds are first disbursed.
    * **Outcome:** This substantial investment aims to yield tangible results of 500-700 new Cardano projects. Dates provided below are for illustrative purposes only.
    * **Outputs:**
        * Fund14 Target launch May , initial disbursements of funds in July/August 2025
        * Fund15 Target launch in August , initial disbursement of funds in Dec 2025/ Jan 2026
        * Fund16 Target launch in October , initial disbursement of funds in Feb-Mar 2026
        * 30-40% of allocated funds (₳24-₳30M) are projected to result in real-world adoption or industrial use-case partnerships.
        * ₳60m in funding will be strategically distributed across four key areas: early-stage R&D, later-stage product development, grassroots ecosystem initiatives, and open-source software development:
            * Cardano Concepts: supporting early stage use-case application development and demonstration from proof of concept (POC) to minimum viable product (MVP)
            * Cardano Partners & Products: supporting later stage market-ready products and use-case implementation for single applicants or in collaboration with industry leading partners to deliver real world pilot-trials
            * Cardano Open Developers: Focused on supporting Cardano’s open source developer ecosystem efforts. Intended for the scope of this category to be set in consultation with the Open Source Committee.
            * Cardano Open Ecosystem: Focused on non-technical proposals for grassroots Cardano regional growth and community-building projects. Intended for the scope of this category to be set in consultation with the Membership and Community Committee and relevant working group participants
        * ₳1m allocated for Retroactive Public Goods Funding (RetroPGF) program

**Total Requested Budget for three workstreams:** ₳69,459,000 (or $34,729,500)
- **Audit & Oversight Allocation:** 3472950 ADA
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


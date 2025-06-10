<!--
Template for Cardano Treasury Withdrawal Proposals

This template combines the constitutional requirements for Treasury Withdrawals
and the terms established in the approved Budget Info Action.  Replace each
placeholder ({{...}}) with the appropriate value for each proposal.
-->
# Treasury Withdrawal Proposal: 2025 Input Output Engineering Core Development Proposal

## Withdrawal Details
- **Amount:** 96,817,080 ADA (96817080000000 lovelace)
- **Destination Address:** Intersect multi-signature escrow address (TBD)
- **Administrator:** Intersect
- **Purpose / Description:** Thank you for your review and consideration. Please see the full proposal in the attached for additional information.

* **Automatic Formal Verification (Plutus High Assurance):** Develop automated formal verification tool for Plinth/Cardano DApps. (**$1,859,000**)
* **Property Based Testing Tool (Plutus High Assurance):** Develop Plinth PBT Tool to automatically generate diverse inputs/actions. (**$2,366,000**)
* **Static Analyzer (Plutus High Assurance):** Develop "one-click" static analysis tool for Plinth contracts. (**$777,140**)
* **Ouroboros Leios Implementation:** Begin core implementation of Leios L1 consensus protocol. (**$7,098,000**)
* **Cardano Node Architecture Refresh (Acropolis):** Re-architect the Cardano node into a modular model (Acropolis). (**$2,028,000**)
* **Hydra Development:** Complete Hydra v1.0 mainnet and full audit, Cardano's L2 state channel solution. (**$1,859,000**)
* **Minotaur AVS:** Launch Minotaur, Actively Validated Service (AVS) leverage Cardano L1 security. (**$1,900,000**)
* **Mithril Development:** Enhance Mithril protocol for secure, efficient access. Speeds up sync, enables light clients. (**$1,859,000**)
* **KES Agent:** Implement security enhancement for SPO KES key storage and management. (**$676,000**)
* **Ledger-HD:** Move ledger state tables from memory to disk (LSM tech) to reduce RAM. (**$1,352,000**)
* **Log-Structured Merge (LSM) including UTXO-HD:** Integrate bespoke Well-Typed LSM-tree backend for managing on-disk state. (**$1,352,000**)
* **Revised Stake Pool Incentive Scheme:** Investigate potential adjustments to SPO incentive scheme. (**$1,352,000**)
* **Nested Transactions (Babel Fees):** Implement Nested Transactions ledger feature enabling tx batching. Facilitates Babel Fees. (**$1,352,000**)
* **Plutus Core Roadmap:** Execute roadmap for Plutus Core delivering key new primitives. (**$2,704,000**)
* **Tiered Pricing Models (Plutus High Assurance):** Introduce transaction prioritization mechanism to improve predictability during congestion. (**$1,352,000**)
* **Transaction Monitoring System (Plutus High Assurance):** Develop system to monitor transactions, detect potential fraud/anomalies. (**$1,690,000**)
* **Maintenance and Support:** Maintenance of existing code base, ongoing support. Includes cost of running Test & Tracing setup. (**$14,682,000**)
* **Audit & Security Assurance:** Engage independent audits and security assurance. Consolidated item. (**$2,150,400**)

**GRAND TOTAL: $48,408,540**
- **Audit & Oversight Allocation:** 4840854 ADA
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


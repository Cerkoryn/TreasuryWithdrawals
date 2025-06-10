<!--
Template for Cardano Treasury Withdrawal Proposals

This template combines the constitutional requirements for Treasury Withdrawals
and the terms established in the approved Budget Info Action.  Replace each
placeholder ({{...}}) with the appropriate value for each proposal.
-->
# Treasury Withdrawal Proposal: Ecosystem Exchange Listing and Market Making service pool

## Withdrawal Details
- **Amount:** 3,126,000 ADA (3126000000000 lovelace)
- **Destination Address:** Intersect multi-signature escrow address (TBD)
- **Administrator:** Intersect
- **Purpose / Description:** Flowdesk acts as a reference party that helps with engineering liquidity provision and listing of CNTs, assisting in:

1- Exchange Listing Fee Pool: 

Eligible exchanges are Kraken, Bybit, Okex and Binance (only top tier exchanges that are requiring new technical integration of CNT)

Budget: Up to 1,500,000 USD (3m ADA at a reference price of 0.5 USD / ADA).

Notes:
- Top-tier exchanges might ask a listing fee > 500,000 USD. An indicative quote from one top-tier exchange would be around 1m USD of token allocation.
- Not more than 500k USD (1m ADA) will be allocated for 1 CNT / Exchange.
- Flowdesk acts as an actor of good faith to validate the budget allocated to a Cardano project for a listing.
- Flowdesk does NOT receive any funds from the Intersect budget during this process (including no transaction fee, commission fee, etc.).
- Flow for a Cardano project to request funds to get listed on an exchange:

=> 1 Cardano project with a CNT

=> Project agrees with the exchange on a listing offer

=> Flowdesk Exchange Listing Criteria Assessment

=> Decision

=> If successful, exchange directly receives funding from Intersect for listing the CNT

=> CNT is listed on the exchange.






2- Market Making Fee Pool: 

Eligible tokens are:

-Non stable coins: SNEK, IAG, MIN and HOSKY

-Stable coins: USDM, USDA, iUSD, DJED, KINKA (gold backed)


Budget: 63,000 USD (126,000 ADA at a reference price of 0.5 USD / ADA).


Notes:

- Intersect > Cardano Project > pays Flowdesk monthly retainer for MMAAS business.
- Flowdesk does NOT receive any funds from the Intersect budget during this process (including no transaction fee, commission, etc.).

- Flow for a Cardano project to request funds for MMAAS with Flowdesk:

=> Cardano projects
=> Project agrees with Flowdesk on a MMAAS offering

=> Cardano project receives funding from Intersect

=> Flowdesk launches the MMAAS service.
- **Audit & Oversight Allocation:** 156300 ADA
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


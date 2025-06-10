<!--
Template for Cardano Treasury Withdrawal Proposals

This template combines the constitutional requirements for Treasury Withdrawals
and the terms established in the approved Budget Info Action.  Replace each
placeholder ({{...}}) with the appropriate value for each proposal.
-->
# Treasury Withdrawal Proposal: MLabs Research towards Tooling for Elliptical Curves - GrumpleStiltSkin

## Withdrawal Details
- **Amount:** 104,347 ADA (104347000000 lovelace)
- **Destination Address:** Intersect multi-signature escrow address (TBD)
- **Administrator:** Intersect
- **Purpose / Description:** GrumpleStiltSkin will deliver an open-source, parameterized elliptic curve and Galois field framework implemented in Plutarch. The goal is to allow smart contracts on Cardano to verify cryptographic proofs over customizable curves and fields. This will include:
Plutarch support for Galois field arithmetic


Plutarch support for elliptic curve arithmetic


A generic ZK verifier in Plutarch


A validation test suite over BLS12-381


A composable YTxP-compatible Plutarch wrapper


This tool empowers developers with on-chain cryptographic flexibility, expands Cardano’s ZK application capabilities, and sets the stage for future innovations in privacy and authentication.

# Introduction

Elliptic curves, specifically over Galois
fields, have found multiple uses in blockchain applications. 
One particularly significant application is zero-knowledge proofs, which promise
significant capability enhancements, ranging from better onchain performance to
new operations. To this end, a whole constellation of different elliptic curves,
based on a huge range of Galois fields, have been proposed and designed. These
vary in their mathematical properties, intended use cases, and other features,
while still being broadly similar in terms of their basic foundations. Such
curves include, but aren't limited to:

* The Pasta curves
* The Grumpkin curve
* BLS12-381

This list is not complete, and is likely to grow larger as time passes. In
general, every blockchain, and its respective software ecosystem, tends to
settle on a different choice of elliptic curve(s) and associated Galois fields.

Plutus is no exception to this. Currently, there are no fewer than eight CIPs, in
various stages of adoption, which either directly, or indirectly, justify their
proposed extensions to Plutus by way of elliptic curves, finite field
arithmetic, or both:

* [CIP-0049]
* [CIP-0058]
* [CIP-0101]
* [CIP-0121]
* [CIP-0122]
* [CIP-0123]
* [CIP-0133]
* [CIP-0381]
 
These proposals are self-evidently useful, as shown by most of them being
adopted into Plutus Core. However, for an application developer who wants to
work over a specific elliptic curve, all of these proposed improvements suffer
from one of two problems. 

The first of these problems, as typified by CIP-0058, is an excess of
generality. You are given the pieces to (possibly) build the curve functionality
you need, but no help beyond that. This means a lot of work, likely involving
expertise (and concerns) far outside your domain of interest or knowledge.
Furthermore, you now become responsible for security considerations around
elliptic curve use. Lastly, if multiple application developers need logic around
a specific curve, this may end up being re-implemented multiple times by
different teams. None of these make the process _straightforward_, and in many
cases might be a hard obstacle to a working product even if it's technically
possible.

The second problem, typified by CIP-0381, is an excess of specificity. If an
application developer wants to work over a specifically-supported curve (such as
BLS12-381 in this case), this is a blessing from the correctness, optimization
and security point of view. However, if this isn't the curve they need, they are
left out in the cold. While it is conceivable for an application developer to
request the curve they need to have direct support in Plutus Core similar to
BLS12-381, this is impractical at best, and creates all the issues discussed
previously regarding incidental complexity and requiring expertise from other
domains.

Furthermore, there is an unspoken problem of having application developers being
forced to own the underlying primitives for their curve implementations. If
issues of performance or security are discovered, or even if some more
operations or generality are needed, the application developers must provide the
upgrade path. This can range from difficult to impossible, and must be
engineered for ahead of time. This just compounds the difficulties involved,
especially for developers who are not experts in either cryptographic security
or onchain performance.

# Our solution

We will create a two-part proof-of-concept system, named Grumpelstilskin, designed 
to allow application developers to easily use any curve of their choice for
zero-knowledge proof verification on-chain. The first part of Grumpelstilskin
will be a 'working script' which, when given appropriate parameters via its
datum, will verify a zero-knowledge proof over a user-specified curve. This
script will be tested for correctness.

The second part of Grumpelstiltskin will be a YTxP-based interface to
the 'working script', implemented in Plutarch. This interface will be
well-documented, easy to use, and flexible, with a focus of making life easy for
application developers who want to use zero-knowledge proofs. Thanks to our use
of YTxP, future performance, security and functionality improvements will not be
the responsibility of application developers who use Grumpelstilskin. This
second part will be distributed as an open-source project. 

We aim to build a minimum viable product, with the future goals of expanded
functionality, improved performance, as well as a full audit of the 'working
script'. Our choice of YTxP will make it minimally difficult to achieve this,
and will impose minimal friction on any application developers using
Grumpelstiltskin to build their products.
- **Audit & Oversight Allocation:** 5217 ADA
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


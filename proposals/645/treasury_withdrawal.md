<!--
Template for Cardano Treasury Withdrawal Proposals

This template combines the constitutional requirements for Treasury Withdrawals
and the terms established in the approved Budget Info Action.  Replace each
placeholder ({{...}}) with the appropriate value for each proposal.
-->
# Treasury Withdrawal Proposal: Complement Catalyst: Extended Quadratic Funding—Zero Operational Costs

## Withdrawal Details
- **Amount:** 1,500,000 ADA (1500000000000 lovelace)
- **Destination Address:** Intersect multi-signature escrow address (TBD)
- **Administrator:** Intersect
- **Purpose / Description:** ### Introduction

The Cardano ecosystem stands at a crucial point in its evolution. Having allocated over $150 million through Project Catalyst to fund 2,161 projects, we have witnessed both the remarkable potential and inherent challenges of our current funding mechanisms—challenges common across all blockchain ecosystems. 

As Cardano matures, so too must our approach to fostering innovation and allocating resources within the ecosystem.

This proposal introduces Extended Quadratic Funding (EQF) as a complementary funding mechanism to Project Catalyst—designed not to replace but to enhance Cardano's innovation landscape by addressing five critical limitations in the current system: centralized voting power, limited treasury resources, inadequate impact reporting, unclear return on investment, and inefficient milestone management.

Extended Quadratic Funding combines the mathematical elegance of quadratic voting with reputation-based mechanisms and decentralized governance to create a more equitable, efficient, and sustainable funding ecosystem. Our approach draws inspiration from successful quadratic funding implementations in other blockchain ecosystems while incorporating unique elements tailored to Cardano's specific needs and values.

### The Current Landscape: Achievements and Limitations of Project Catalyst

Project Catalyst represents one of the largest decentralized innovation funds in the blockchain space, demonstrating Cardano's commitment to community-driven development. Through multiple funding rounds, it has supported a diverse array of projects spanning DeFi protocols, educational initiatives, infrastructure improvements, and real-world applications.

However, as the ecosystem has grown, several structural limitations have become increasingly apparent which are common in all blockchain ecosystems:

### 1. Centralized Voting Power

Recent research by Nelson et al. (2024) has quantified what many community members have observed anecdotally: voting power in Project Catalyst is highly concentrated. Their analysis revealed that in 97.5% of voting coalition scenarios, just 1.5% of wallets could determine the final outcome. This concentration reached its apex in Fund 13, where a single entity effectively controlled most funding decisions.

This concentration creates several problems:

- **Narrowed Innovation Focus**: When funding decisions reflect the interests of a few large stakeholders, we risk prioritizing certain types of projects while neglecting others that might better serve the broader ecosystem.
- **Diminished Participation Incentives**: Small token holders have little motivation to participate in governance when their votes rarely influence outcomes.
- **Vulnerability to Capture**: Concentrated decision-making power creates potential vulnerabilities to special interests that may not align with the ecosystem's long-term health.
- **Inconsistency with Cardano's Philosophy**: The current voting mechanism contradicts Cardano's foundational commitment to decentralization and broad-based governance.

### 2. Limited Treasury Resources

Every blockchain ecosystem has a finite treasury. As ecosystems grow and funding demands increase, treasuries face mounting pressure. The current model's exclusive reliance on treasury funds—without additional capital sources—limits both the number and scope of projects that can receive support.

Furthermore, the all-or-nothing approach to project funding creates inefficiencies: projects either receive their requested amount or nothing at all, lacking mechanisms for partial funding based on broader community support.

### 3. Inadequate Impact Reporting

Like all innovation funding systems, Project Catalyst faces challenges in establishing standardized mechanisms to track and report the impact of funded projects. 

This creates several challenges:

- **Difficulty Measuring ROI**: Without consistent metrics, it's nearly impossible to evaluate the return on investment for ecosystem funds.
- **Limited Learning Opportunities**: The absence of standardized impact data prevents the community from identifying successful funding patterns that could inform future allocations.
- **Reduced Accountability**: Without transparent reporting requirements, funded teams have limited incentives to maximize their projects' ecosystem impact.
- **Undermined Community Trust**: The lack of clear impact evidence can erode stakeholder confidence in the funding process over time.

### 4. Unclear Return on Investment

The current funding model operates as a one-way flow of resources: treasury funds are allocated to projects without mechanisms for value to flow back to the ecosystem. While this grant-based approach is appropriate for many public goods, it fails to capture potential value from successful commercial projects that achieve significant traction or profitability.

This limitation:

- Reduces the treasury's long-term sustainability
- Fails to maximize the ecosystem's return on successful projects
- Creates a potential misalignment of incentives between funded teams and the broader community

### 5. Inefficient Milestone Management

Milestone review processes across the industry, including Project Catalyst have become a significant challenge, with funded teams often waiting months for payments during review periods. These centralized, opaque processes create:

- **Cash Flow Challenges**: Extended payment delays force teams to self-fund development, advantaging well-capitalized teams over bootstrapped innovators.
- **Project Abandonment**: Payment delays have contributed to numerous teams abandoning funded projects, wasting both treasury resources and development efforts.
- **Dispute Resolution Inefficiencies**: The current system requires the Catalyst team to mediate all disputes between reviewers and funded proposers, creating a significant administrative burden.
- **Scaling Limitations**: As the number of funded projects grows, the centralized review process becomes increasingly untenable.

### Extended Quadratic Funding: A New Paradigm

Extended Quadratic Funding addresses these limitations through five interconnected innovations:

### 1. Democratizing Decision-Making

At the core of our proposal is a novel voting mechanism that balances financial contribution with demonstrated community impact. The EQF voting power calculation multiplies:

1. **The square root of the donation amount in USD**
    - Example: A $9 donation yields 3 votes (√9 = 3)
    - Example: A $100 donation yields 10 votes (√100 = 10)
    - Example: A $10,000 donation yields 100 votes (√10,000 = 100)
2. **Impact Score—a logarithmic representation of reputation**
    - Ranges from 300 to 850 (similar to credit score systems)
    - Increases more slowly as score rises (logarithmic scaling)

This dual mechanism ensures that while financial contribution remains important, its influence is both:

- **Mathematically constrained** through the square root function (quadratic scaling)
- **Balanced by reputation** through the Impact Score multiplier

For example:

- A new community member donating $100 with a baseline Impact Score of 300 would have 10 × 300 = 3,000 voting power
- An established contributor donating $100 with an Impact Score of 700 would have 10 × 700 = 7,000 voting power
- A whale donating $10,000 with a baseline Impact Score would have 100 × 300 = 30,000 voting power

This system significantly reduces the plutocratic effect of the current one-coin-one-vote system while maintaining "skin in the game" principles through financial contribution requirements.

### Sybil Resistance

To protect the integrity of this system, we implement robust Sybil resistance through Self-Sovereign Identity (SSI) verification powered by Hyperledger Identus (formerly Atala PRISM). This system:

- Conducts zero-knowledge proof KYC checks to ensure each account represents a unique human
- Preserves privacy by never storing personal identification information on-chain
- Creates a one-human-one-account ecosystem without compromising user anonymity

### Anti-Collusion Mechanisms

We employ four complementary strategies to prevent collusion:

1. **Reputation-Based Incentives**: High Impact Score individuals have strong incentives to maintain system integrity, as their accumulated reputation gives them advantages within the ecosystem.
2. **Graduated Penalties**: Those caught engaging in coordinated voting face escalating consequences:
    - First offense: Impact Score reduction
    - Severe or repeated offenses: Permanent platform ban
    - Since KYC verification is required, banned participants cannot simply create new identities
3. **Economic Disincentives**: Our fee structure makes vote-splitting unprofitable:
    - Platform fees decrease with donation size
    - This makes it more expensive to split funds across multiple accounts
4. Implement [Connection-Oriented Cluster Matching](https://www.gitcoin.co/blog/leveling-the-field-how-connection-oriented-cluster-matching-strengthens-quadratic-funding)
    1. **Cluster Detection**: Groups users based on donation patterns and assigns weighted connection values
    2. **Similarity Scoring**: Analyzes connections between donors to identify related groups
    3. **Smart Fund Distribution**: Rewards projects with diverse donor bases while limiting funding for closely connected groups

Together, these mechanisms make collusion economically irrational while preserving legitimate voting influence.

### 2. Multiplying Treasury Impact

The Extended Quadratic Funding model transforms the treasury from the sole funding source to a catalytic multiplier of community resources. Here's how it works:

1. The Cardano treasury allocates a predetermined amount to the matching pool (e.g., $1M)
2. During the funding round, community members make direct donations to projects they support
3. These donations serve two purposes:
    - They provide direct funding to projects (projects keep 100% of direct donations)
    - They determine each project's share of the matching pool
4. The matching formula allocates treasury funds based on both donation amount and distribution:
    - Projects with many small donations receive proportionally more matching funds than those with a few large donations
    - This incentivizes projects to build broad community support rather than courting a few wealthy backers

For example, consider two projects:

- Project A receives 100 donations of $10 each (total: $1,000)
- Project B receives 1 donation of $1,000 (total: $1,000)

Though both raised the same amount, Project A would receive significantly more from the matching pool due to its broader support base—potentially 10× more. 

This mechanism creates powerful incentives:

- **For donors**: Even small donations significantly boost a project's matching allocation
- **For projects**: Building community support becomes as important as securing large contributions
- **For the treasury**: Each allocated ADA potentially mobilizes additional external capital

U.S. donors gain an additional benefit through our 501(c)(3) structure, making donations tax-deductible—creating unique incentives even outside the cryptocurrency ecosystem.

### 3. Standardized Impact Reporting

All projects funded through the Extended Quadratic Funding mechanism must participate in standardized impact reporting. This includes:

1. **Mandatory Impact Accounting**: Each funded project must allocate a small portion of their funding to contract with a designated impact accountant from an approved pool.
2. **Standardized Metrics**: All projects report a core set of ecosystem impact metrics:
    - On-chain transactions generated
    - New wallets created
    - Active users acquired
    - Project-specific KPIs aligned with proposal goals
3. **Regular Reporting Cadence**: Metrics are reported on a standardized schedule:
    - Quarterly reports for one year after project completion
    - Annual reports for commercial projects with revenue-sharing agreements
4. **Public Dashboard**: All impact metrics are published on a public dashboard, creating unprecedented transparency into the outcomes of funded innovation.

This comprehensive reporting system enables:

- **Data-Driven Decisions**: Future funding rounds can be informed by concrete impact data
- **Pattern Recognition**: The community can identify which types of projects deliver the highest ROI
- **Accountability**: Funded teams have clear incentives to demonstrate meaningful ecosystem impact
- **Learning Opportunities**: Unsuccessful projects provide valuable insights alongside successes

### 4. Sustainable Value Capture

To ensure long-term treasury sustainability, we implement a voluntary contribution system where funded projects that achieve commercial success share value with the ecosystem. This operates through several mechanisms:

1. **Equity Agreements**: Commercial startups can offer a small equity stake (typically 1-3%)
2. **Token Allocations**: Projects launching tokens can allocate a portion to the ecosystem (typically 2-5%)
3. **Revenue Sharing**: Commercial applications can contribute a percentage of revenue (typically 1-3%)
4. **Alternative Value**: Some projects may contribute other assets like carbon credits or data access

These contributions flow into a dedicated treasury separate from the main Cardano treasury but governed by the same community. This creates a virtuous cycle where successful projects help fund future innovation.

Our target is to achieve an annual 5% ROI within 10 years across the entire portfolio. While ambitious, this benchmark is actually conservative compared to traditional venture capital expectations, reflecting our balanced approach to funding both public goods and commercial applications.
- **Audit & Oversight Allocation:** 75000 ADA
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


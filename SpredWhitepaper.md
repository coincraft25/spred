# Spred: The Protocol for What We Believe

### "Say it first. Spred it forever." — Block 0 — AXN

## Abstract

Spred introduces a new class of public infrastructure: a decentralized protocol for timestamping collective belief. While blockchains proved that trust can be engineered and truth can be verified, we still lack a native mechanism for recording what people expect will happen — across markets, events, culture, and society.

This is more than betting. More than polling. This is an infrastructure layer for collective foresight. Spred encodes structured belief into public data — validated by the crowd, secured by time, and rewarded through contribution.

As AI blurs what's real, belief becomes more important than ever. Spred anchors that belief in a transparent, verifiable system.

## 1. The Problem: Belief Has No Ledger

Today's internet captures what happened and what's happening — but not what people believe will happen.

Social media is optimized for attention, not foresight. Polls are closed systems with unclear methods. Prediction markets are often inaccessible or legally restricted. None of them offer a persistent, trustless ledger of predictions tied to outcomes.

There's no canonical place where the world can record its foresight — and track its accuracy — without censorship, manipulation, or central control. This leaves society blind to its own collective intuition.

We need a new primitive: belief-as-data. That's what Spred provides.

## 2. The Idea: A Ledger of Belief

Spred turns public belief into a digital primitive — one that anyone can submit, anyone can validate, and everyone can see.

Instead of being owned by a platform or interpreted by pundits, belief becomes structured, timestamped, and verified onchain. Each prediction becomes a data object. Each validator becomes a signal miner. Over time, these objects form a living history of what people expected — and what actually happened.

The result is a global "belief index" — transparent, decentralized, and composable.

Spred isn't a social app or a gambling platform. It's a belief infrastructure layer — designed to integrate with newsrooms, trading platforms, DAOs, and future internet protocols.

It's not engagement. It's foresight, structured.

## 3. Protocol Structure

Spred is composed of five core systems. Each is modular, onchain, and can operate independently or together. Together, they allow anyone to propose, resolve, and track structured predictions without central control.

### 3.1 Prediction Market Engine

Markets consist of:

- Market ID (hash)
- Creator address or alias
- YES/NO title
- Optional description
- Deadline timestamp
- Tags
- Outcome type (binary, range, or invalidation flag)

Markets are immutable. Once posted, they cannot be altered and await resolution. To support flexibility, markets can include non-binary outcomes (e.g., numerical ranges) or be marked for invalidation if ambiguous.

### 3.2 Validator Network

Markets enter the resolution phase after the deadline. Validators submit YES, NO, or "no consensus" outcomes, optionally including sources. Votes are weighted by reputation. Consensus is reached once quorum and majority are met, or the market is invalidated if no clear outcome emerges. Finalization distributes rewards and reputation.

### 3.3 Reputation System

Validators build a reputation score over time, based on historical accuracy. This score affects voting power, eligibility for governance, and reward distribution. To reduce validator fatigue, automated tools (e.g., source aggregators) assist without replacing human judgment.

### 3.4 Emission Engine

$SPRED is emitted through market resolution only. Rewards decay over time and follow a soft cap schedule. There is no inflation.

### 3.5 Governance Layer

Spred is governance-optional. Forks, councils, or DAO tools may emerge, but they are not required. All governance is opt-in and weighted by reputation, not wealth.

## 4. Lifecycle of a Market

1. A user submits a market (YES/NO, range, or other format)
2. The market is posted onchain
3. After the deadline, validators begin voting
4. Quorum and consensus are reached, or the market is invalidated
5. Outcome is finalized
6. Rewards and reputation are distributed
7. Market becomes part of the belief ledger

## 5. Validators and Reputation

In Spred, validators perform the essential task of resolving predictions.

They do not rely on hardware or mining rigs. Their work is intellectual: they evaluate whether real-world outcomes matched submitted predictions. Their votes determine the resolution of markets and directly impact the accuracy, credibility, and integrity of the protocol.

Validators operate permissionlessly. Any wallet address may participate in market resolution without needing approval, identity verification, or prior history.

### 5.1 Role of Validators

Validators may:

- Submit a vote on the final outcome (YES, NO, range, or "no consensus")
- Optionally provide reference evidence or links
- Use protocol-provided tools (e.g., integration with news APIs, blockchain oracles, or RSS feeds for source aggregation) to streamline evaluation
- Participate in dispute processes

The protocol checks for:

- Validator eligibility (no duplicate voting, deadline met)
- Quorum (sufficient number of weighted votes)
- Consensus (clear majority of weighted outcome or invalidation)

### 5.2 Reputation: Definition and Purpose

Reputation is a numerical, onchain score based on predictive accuracy. It is:

- Wallet-bound
- Non-transferable
- Immutable except by protocol
- Used to weight votes and unlock governance roles

It incentivizes long-term honest participation and discourages spam, Sybil attacks, and manipulation. To encourage sustained participation, validators receive secondary incentives like badges or leaderboard visibility.

### 5.3 Reputation as a Mathematical Score

Each resolution updates a validator's score:

- Correct outcome → rep increases
- Incorrect outcome → rep decreases
- Abstain or "no consensus" vote → no change

Smart contracts handle all scoring. Optional advanced weighting may reward early or contrarian correct votes.

### 5.4 Weighting and Impact

Reputation determines:

- Vote weight
- Reward share
- Governance eligibility
- Dispute credibility

Only long-term accurate validators shape future outcomes.

### 5.5 Reputation and Governance

Should governance evolve, it will be weighted by reputation — not wealth.
Reputation is the protocol's memory of trust.

## 6. Emission and Scarcity

Spred uses a fixed-supply token model designed for longevity, fairness, and protocol integrity. There will never be more than 1,000,000,000 $SPRED tokens — no minting, no inflation, no admin key.

Just like Bitcoin, Spred's economy is based on scarcity over time. But unlike Bitcoin, emission is tied to resolved predictions — not blocks.

This is not "earn by staking." It's earn by resolving truth.

### Dual-Layer Emission Model

**1. Per-Market Reward Decay**

| Year | Reward per Market |
| --- | --- |
| 1 | 1000 $SPRED |
| 2 | 500 $SPRED |
| 3 | 250 $SPRED |
| 4 | 125 $SPRED |
| 5 | 62.5 $SPRED |

Formula: R(n) = 1000 × (1/2)^(n−1)

**2. Soft Yearly Cap (Emission Ceiling)**

| Year | Max Emission (Soft Cap) |
| --- | --- |
| 1 | 100,000,000 $SPRED |
| 2 | 50,000,000 |
| 3 | 25,000,000 |
| 4 | 12,500,000 |
| 5 | 6,250,000 |

If usage exceeds the cap, reward per market adjusts proportionally.

This protects scarcity, encourages quality, and extends the emission runway for 100+ years.

## 7. Token Distribution

The initial distribution is designed to balance community growth, protocol protection, and long-term evolution.

| Category | % Supply | Notes |
| --- | --- | --- |
| Community Rewards | 35% | Distributed through markets |
| DAO Treasury | 25% | Controlled by governance |
| Team + Founder | 15% | 4-year vesting, 1-year cliff |
| Builders & Grants | 10% | Dev incentives + integrations |
| Backers (optional) | 10% | Vested 4 years if included |
| Culture / Airdrops | 5% | Rep-based or viral ecosystem |

All locked allocations are verifiable and onchain.

## 8. Privacy and Participation

Spred protects not just what people believe — but their right to believe it privately.

In many parts of the world, public prediction is dangerous. Speaking about elections, economics, or geopolitics can come with real consequences. Even in free societies, reputational and social pressure can silence honest forecasting.

If Spred is to become a global belief layer — it must protect belief at the individual level.

Privacy is not an add-on. It is a core design principle.

### 8.1. No Identity Required

Participation in Spred does not require:

- Real names
- Email addresses
- Logins
- Biometric data
- Centralized accounts

Users interact entirely through cryptographic wallets — the same way Ethereum, Bitcoin, and other public protocols operate.

This preserves pseudonymity by default. Your identity is your wallet. Your reputation is your accuracy.

### 8.2. Anonymous Prediction

Anyone can submit a market prediction anonymously.

This enables users to propose bold, controversial, or sensitive questions without fear of censorship or backlash — political, social, or otherwise.

While submitted predictions are public, the authors do not need to tie them to a real-world identity or alias.

### 8.3. Private Validation

Validators — those who resolve predictions — are equally protected.

By default, validator addresses are visible onchain. But Spred supports optional vote obfuscation using:

- Commit-reveal schemes: validators submit a hashed vote first, then reveal it after quorum
- Zero-knowledge proofs (zk): validators prove they voted correctly without revealing which way they voted
- Alias shielding: linking validator activity to rotating addresses or pseudonymous reputation handles

These tools ensure validators can participate truthfully — even on controversial markets — without being targeted or pressured.

### 8.4. No Surveillance, No Profiling

Spred does not:

- Track IPs
- Correlate wallet activity across services
- Sell behavioral data
- Personalize feeds or predictions
- Profile users

There is no algorithm deciding what you see. No ads. No amplification. The protocol does not care who you are — only what you think will happen.

This stands in contrast to social platforms that extract attention through surveillance and personalization.

### 8.5. Open Participation, Global Access

Because Spred has no KYC, country restrictions, or centralized dependencies, anyone with an internet connection and a wallet can participate.

- Predictors can speak
- Validators can resolve
- Observers can track belief trends

This is especially powerful in parts of the world where access to forecasting tools, open dialogue, or public data is restricted or controlled.

To enhance accessibility, Spred supports user-friendly interfaces (e.g., sponsored transactions, mobile apps) built by the community, ensuring decentralization is maintained.

### 8.6. Trust Without Exposure

Reputation is wallet-bound and earned through accuracy — but it does not require exposure of your identity.

Your influence in the protocol is based on your contribution to truth — not who you are, how loud you are, or where you're from.

### 8.7. Protection Against Fake Wallets and Manipulation

Spred is designed to be open to all, but not exploitable.

The protocol anticipates Sybil attacks — where a malicious actor tries to influence outcomes by creating many fake wallets. This is a known risk in any permissionless system.

Spred defends against this using a multi-layered design:

**1. Reputation is Wallet-Bound and Non-Transferable**

Creating a new wallet gives you no power. Every wallet starts at zero reputation. Only through correct validation over time can a wallet build credibility.

This makes it very costly to spin up fake identities — they must earn trust slowly, over many markets, with truthful participation.

**2. Reputation = Voting Power**

It's not one wallet = one vote. It's reputation-weighted.

A new or fake wallet's vote may carry less than 0.1% of the total weight. It cannot influence consensus — especially as more trusted validators participate.

**3. Time-Weighted Participation**

Validators earn more trust the longer they maintain accuracy. Even if someone builds a high-rep fake wallet, they must maintain it honestly for months or years — reducing the incentive to manipulate in the short term.

**4. Stake-Based Friction (Optional)**

For high-impact predictions or governance proposals, the protocol can require a small token or rep stake to vote or propose. This makes mass fake participation expensive and traceable — without excluding legitimate users.

**5. Pattern Detection (Off-Chain Tools)**

While the protocol doesn't track IPs or identities, open-source analysis tools can flag suspicious behavior patterns (e.g., 100 wallets voting identically). These tools don't censor — they inform the community and DAO governance when needed.

In Spred, you can create as many wallets as you like. But only accuracy earns power.

This is not proof-of-identity. This is proof-of-truth over time.

This aligns with the values of:

- Bitcoin's pseudonymous founder
- Signal's end-to-end encryption
- The open internet before identity platforms

Spred is not surveillance capitalism. It is a cryptographic commons for belief. Built for the truth. Protected by privacy. Designed for the world.

## 9. Disputes and Governance

Markets resolve automatically by quorum. If a dispute is triggered, the protocol enters resolution mode:

- Users can stake to challenge a result
- Disputes open validator re-voting
- If quorum shifts, results may reverse
- Disputes are capped at two re-vote rounds to prevent abuse
- Frivolous challenges incur a reputation penalty proportional to stake
- Further escalation can move to a Validator Council or fork

Governance is optional, decentralized, and always forkable.

## 10. Scalability and Cost Mitigation

Spred is designed to scale globally while remaining accessible. To address onchain costs, the protocol is chain-agnostic, supporting deployment on Layer 1 blockchains (e.g., Ethereum) or Layer 2 solutions (e.g., rollups, sidechains). Key strategies include:

- **Batch Processing**: Multiple market resolutions can be finalized in a single transaction to reduce gas fees.
- **Off-Chain Commitments**: Validators can submit votes off-chain with on-chain finality, minimizing costs while preserving security.
- **Sponsored Transactions**: Community-built interfaces may cover fees for new users, lowering the entry barrier.
- **Fee Optimization**: Dynamic fee adjustments prioritize high-impact markets during congestion.

These measures ensure Spred remains cost-effective without compromising decentralization or trustlessness.

## 11. Legal Resilience and Regulatory Considerations

Spred’s open, pseudonymous nature empowers global participation but may attract regulatory scrutiny in some jurisdictions, particularly for sensitive predictions (e.g., elections, financial events). To ensure resilience, the protocol adopts:

- **Decentralized Hosting**: No single point of failure for protocol data or interfaces, leveraging IPFS or similar technologies.
- **Community-Driven Defense**: The DAO treasury allocates resources for legal education and advocacy, empowering users to navigate local regulations.
- **Jurisdictional Diversification**: Validators and nodes are distributed globally, reducing reliance on any one legal framework.
- **Transparent Compliance**: All token allocations and governance decisions are onchain, ensuring auditability without centralized control.

Spred does not evade responsibility—it decentralizes trust, empowering users to operate within their local contexts while maintaining protocol integrity.

## 12. Data Composability and Integration

The belief ledger is a public good, designed for maximum utility. To enable third-party integration, Spred provides:

- **Standardized Schemas**: Markets and outcomes follow a consistent JSON-like structure, queryable via public explorers.
- **APIs and Endpoints**: GraphQL or REST APIs allow newsrooms, DAOs, and platforms to pull real-time or historical belief data.
- **Event Logs**: Onchain events (market creation, resolution, disputes) are emitted for easy indexing by external tools.
- **Open-Source Tooling**: Community grants fund dashboards, analytics, and SDKs to simplify integration.

This ensures the belief index is not just a ledger but a composable layer for the internet, accessible to developers, researchers, and organizations.

## 13. Adoption and Onboarding

To bootstrap adoption, Spred prioritizes accessibility and community engagement:

- **User-Friendly Interfaces**: Community-built mobile apps and browser extensions abstract wallet complexity, supporting sponsored transactions for new users.
- **Partnerships**: Early integrations with DAOs, newsrooms, and DeFi platforms showcase real-world value (e.g., forecasting governance votes, election outcomes, or market trends).
- **Incentivized Campaigns**: Airdrops and reputation boosts reward early predictors and validators, driving network effects.
- **Educational Resources**: Tutorials and guides lower the learning curve, emphasizing Spred’s role as a public utility.
- **Cultural Engagement**: Community-driven storytelling, such as pilot projects with newsrooms to forecast local elections, builds trust and counters skepticism about pseudonymous systems.

These efforts ensure Spred transitions from a protocol to a widely-used belief infrastructure.

## 14. Measuring Impact

Spred’s success is measured by its ability to become a trusted, global belief index. Key performance indicators include:

- **Market Activity**: Target 10,000 resolved markets in year 1, growing 50% annually.
- **Validator Participation**: Aim for 100 active validators per market to ensure robust consensus.
- **Integration Milestones**: Secure 5 major integrations (e.g., DAOs, newsrooms) within 18 months.
- **Community Growth**: Achieve 1,000 daily active predictors and validators by year 2.
- **Accuracy Benchmark**: Maintain a 75%+ correlation between resolved predictions and real-world outcomes.

These metrics guide community efforts, ensuring Spred delivers on its promise as a public utility for foresight.

## 15. Why Now

AI, synthetic media, and real-time chaos have made truth fragile.

The internet doesn't know what it believes. Spred makes that belief visible — timestamped and permanent.

It is not a company. It is not a product. It is a protocol for human foresight.

It will outlive its creators. It will evolve in public. It is powered by truth — not noise.

## 16. Conclusion: A Protocol for the Next Century

We are entering an age where reality is increasingly difficult to measure — and even harder to agree on.

AI generates synthetic content at scale. Platforms personalize everything. Institutions are questioned. In this landscape, trust breaks. Attention dominates. And prediction becomes power.

But there has never been a neutral, public, cryptographic place to record what the world believes will happen — and verify whether it did.

Spred fills that void.

It is not a company. It is not an app. It is not trying to monetize belief.

It is a neutral infrastructure layer for the internet's foresight.

Like Bitcoin gave us unstoppable money, Spred gives us unstoppable belief.

A timestamped, decentralized, censorship-resistant archive of human intuition — built entirely in public, with no owner, no admin, and no backdoor.

Anyone can participate. Only the truth survives. And over time, this truth becomes signal.

News organizations can use it. DAOs can plug into it. Governments can fear it — or embrace it.

But no one can stop it.

Spred is designed to outlive its founders, evolve through its community, and become part of the foundational fabric of the internet — as essential to our digital memory as blockchains, domain names, or public archives.

It is the world's unofficial belief index. A future-facing protocol for a truth-fragmented era. And it begins with one block, one question, and one person willing to say:

"I believe this will happen."

Then: Prove it. Spred it. Forever.

Block 0 begins. "Say it first. Spred it forever." — AXN

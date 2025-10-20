# Matrix Wallet: The Decentralized Bank for Everyone - White Paper
Answer directly under each section (brief bullets are fine). Once filled, we will convert this into the first full draft.

### Abstract
- What single sentence best describes Matrix Wallet's core value for mass adoption?
  - "Simplicity is our DNA"
- Who is the primary audience (first-time users, Web3 natives, SMEs, remittance users)?
  - Our primary target audience is the general public, including both newcomers and experienced users. We aim for mass adoption across all user segments - from first-time crypto users to Web3 natives, small businesses, and remittance users.
- What problem do you solve better than existing wallets/banks (onboarding, UX, gas, security)?
  - **Minimal Complexity**: Eliminate overwhelming technical barriers that prevent mainstream users from entering crypto
  - **High Security**: Enterprise-grade security without compromising user experience  
  - **Gas-Free Operations**: Users don't need native tokens for transactions on any supported network
  - **Gmail Integration**: Send crypto directly to Gmail addresses, making it as simple as sending an email
  - **Social Recovery**: Secure wallet recovery through trusted social links like Google and Apple
- What are the 3–5 flagship features that make it "a decentralized bank for everyone"?
  1. **One-Tap Onboarding**: Google/Apple sign-in with instant wallet creation
  2. **Gas-Sponsored Transactions**: No need for native tokens on any network
  3. **Gmail Sending**: Send crypto to email addresses
  4. **Social Recovery**: Secure wallet recovery through social authentication
  5. **Multi-Chain Support**: Seamless experience across Bitcoin, Ethereum, Tron, Solana, and BNB Chain
- What measurable outcomes do you aim for (e.g., 5M users, <$0.05 effective tx cost, NPS)?
  - **Target**: 100 million monthly active users by end of 2026
- What is the core economic model in one sentence (MTX role, revenue, distribution)?
  - Hints: Revenue sources, MTX utility, how value accrues and distributes; sustainability.
- What chains and assets are supported at launch?
  - Bitcoin, Ethereum, Tron, Solana, and BNB Chain at launch, with additional networks added based on user demand.

- TODO Diagram: Product overview (users, mobile app, relayer/paymaster, networks).

### Introduction & Problem Statement
- What specific frictions block mass adoption today (seed phrases, fees, volatility, scams)?
  - Hints: Concrete examples; quantify drop-offs; risk and trust barriers for newcomers.
- What real-world use cases are you targeting first (P2P, remittances, small-business payments)?
  - Hints: Frequency/amounts; TAM; why these users switch; competitor alternatives.
- Who are your key personas (e.g., “grandfather” user profile) and their top 3 needs?
  - Hints: Demographics, access to devices/ID, accessibility needs, support expectations.
- What is broken in “crypto wallets as banks” today (custody, fees, reliability, UX)?
  - Hints: Custody risk, hidden fees, outage frequency, UX pitfalls, competitor gaps.
- What regulatory/trust concerns do target users have and how will you address them?
  - Hints: KYC/AML, sanctions, classification risks, disclosures, regional considerations.
- What success criteria define “solved” (time to first transaction, cost, support responsiveness)?
  - Hints: Time-to-first-send, activation rate, support SLA, complaint rate.

- TODO Chart: Adoption funnel (onboard → first send → week 4 retention) and top pain points.

### Solution Overview
- What type of wallet is Matrix: non-custodial smart account (AA/4337), EOA, hybrid, or custodial?
  - EOA (externally owned account). ERC‑4337 smart accounts are promising but still unevenly supported across chains and dApps; we start with EOA to maximize compatibility and user confidence in key ownership while still delivering features like gas sponsorship and Gmail‑based sending.
  - Distributed via official stores (Google Play and Apple App Store) to ensure a trusted install path.
  - Regular updates deliver new features and fixes through the same channels.
  - 24/7 support via chat and email; MTX holders receive priority routing.
  - Hints: Tradeoffs (UX vs. trust); upgradeability; standards supported; compliance impact.
- How do users onboard (email/social signup, OAuth with Google, seedless, social recovery)?
  - One‑tap onboarding with Google or Apple sign‑in. After OAuth, the wallet is ready to use.
  - Optional email‑based identity linking to enable Gmail send; seedless UX with secure device binding.
  - Hints: Step-by-step flow; fallback paths; recovery setup defaults; bot/Sybil defenses.
- What makes the UI “grandparent-simple” (flows, language, defaults, accessibility)?
  - Plain‑language copy, minimal steps, and safe defaults to prevent mistakes.
  - Fiat display in preferred currencies (e.g., EUR, JPY) and multi‑language support.
  - Accessibility: large touch targets, high contrast, and WCAG‑aligned patterns.
  - Hints: Plain language; safe defaults; large touch targets; WCAG; cognitive load.
- How does “gas sponsored transfer” work at a high level (who pays, limits, eligibility)?
  - Policy‑based sponsorship: in some cases we fully sponsor transactions; in others the user pays fees from held tokens (e.g., USDT) instead of native gas. The goal is to make sending cheaper and simpler than acquiring native tokens, often below standard network fees on certain chains.
  - Hints: Funding source; per-user caps; eligible tx types; abuse prevention; reporting.
- How does “send using Gmail” work conceptually (identity mapping, verification, privacy)?
  - Available to registered users who opt‑in via OAuth. Users can resolve a Gmail identity to the recipient’s wallet address. Daily/monthly limits apply; suspicious activity triggers enhanced checks or account restrictions. Privacy and consent are respected per policy.
  - Hints: OAuth scopes/consent; email↔address mapping; recipient claim UX; data privacy.
- What core banking-like features are included at launch (send/receive, swap, earn, borrow)?
  - Launch focus: send/receive (address and Gmail), swap, earn, and borrow/loan.
  - Priorities: easy access, strong safety, and reliable performance for daily use.
  - Hints: MVP vs. later; dependencies; jurisdictional restrictions; disclosures.
- Which chains/networks and assets are supported initially vs. later?
  - Phase 1: Bitcoin, Ethereum, BNB Chain, Solana, and Tron. Additional networks prioritized by user demand.
  - Focus on transfers, swaps, lending/borrowing, and staking, with emphasis on stablecoins (USDT/USDC) and major assets (BTC/ETH). Deposits may serve as collateral for borrowing stablecoins when available.
  - Hints: Rationale for choices; bridging approach; roadmap milestones.
- What’s your trust model and key security guarantees to users?
  - Non‑custodial EOA: private keys are encrypted with a user passphrase; application code cannot access plaintext keys. Your keys, your funds.
  - User‑controlled lock/unlock settings and session timeouts.
  - Hints: Non-custodial stance; third-party reliance; incident response commitments.
- How are approvals/allowances handled to minimize risk and simplify UX?
  - User‑selectable scopes: one‑time approvals, limited allowances, or broader allowances where appropriate; clear revoke flows and proactive alerts.
  - Hints: One-time vs. unlimited defaults; revoke flow; proactive alerts; education.
- What is the multi-device experience (sessions, sync, recovery across devices)?
  - Single‑active‑device by default for safety, with secure cloud sync enabling recovery on a new device. Passphrase encryption protects keys on a lost device; users can rotate keys and migrate assets after re‑provisioning.
  - Hints: Device binding; session revocation; key sync; lost device recovery.
- What support/operations guarantees exist (SLA, incident status, transparency)?
  - 24/7 monitoring and on‑call coverage across backend, infrastructure, and app.
  - External audits supplemented by continuous in‑house red‑teaming.
  - Incident response runbooks, public status page, and post‑incident reports.
  - Hints: Channels/hours; response SLAs; status page; postmortems cadence.

### Solution Details — Technical Specification
- Wallet/account model:
  - Smart account standard (ERC‑4337/AA)? Paymaster? Bundler? Session keys?
    - Hints: Why 4337; bundler providers/SLAs; session key scopes/durations; upgrade path.
  - Key management (MPC, device keys, passkeys, socials), social recovery policy, multi-device.
    - Hints: Thresholds/shares; backup strategy; guardian rules; device provisioning.
  - Recovery flows and anti-phishing mechanisms.
    - Hints: Time-locks; multi-factor confirmations; phishing education; usability tests.
  - TODO Diagram: Account/recovery architecture (keys, guardians, time-locks, sessions).
- Gas sponsorship:
  - Sponsorship policy (per-user caps, whitelists, geos), fraud prevention, abuse limits.
    - Hints: Caps/eligibility; Sybil detection; geo policy; logging and rate limits.
  - Who funds it (treasury, MTX staking pool)? Budgeting and monitoring.
    - Hints: Budget ceilings; on/off switch; reporting frequency; governance levers.
  - TODO Sequence Diagram: Sponsored tx path and paymaster authorization.
  - TODO Table: Sponsorship tiers vs. caps/fees.
- Send using Gmail:
  - Identity resolution (email ↔ address mapping), verification (OAuth scope), consent UI.
    - Hints: Scopes needed; consent wording; uniqueness handling; opt-out/revoke.
  - Handling email changes, revocation, spoofing prevention, privacy, data retention.
    - Hints: Change detection; secure remapping; audit trails; retention windows.
  - Delivery UX for recipients without wallets (claim flow, expiration, fallback).
    - Hints: Gasless claim; expiry; re-route funds; custodial fallback policy.
  - TODO Sequence Diagram: Email/handle resolution and claim process.
  - TODO ERD: Identity/contact mapping and retention policy.
- Payments and transfers:
  - Supported token standards, stablecoins, fiat on/off-ramps, compliance checks (sanctions).
    - Hints: Initial stablecoins; partners for on/off-ramp; screening provider; limits.
  - Cross-chain strategy (bridges, messaging, risks).
    - Hints: Chosen bridges; risk disclosures; fallback routes; insurance/escrow.
  - TODO Flowchart: Cross-chain transfer and compliance screening.
- Swap:
  - Aggregator(s) (0x, 1inch, Paraswap), routing, MEV protection, slippage controls.
    - Hints: Aggregators used; private orderflow; max slippage; simulation and quotes.
  - Fees/spreads and who receives them.
    - Hints: Fee schedule; recipients (treasury/MTX); disclosure in UI.
  - TODO Sequence Diagram: Swap routing via aggregator with MEV protection.
- Earn and borrow:
  - Integrated protocols (Aave/Compound/Lido/etc.) vs. native offerings.
    - Hints: Whitelisting criteria; audits; custody of assets; oracle dependencies.
  - Risk disclosures, APY sources, smart-contract risk, custody of collateral.
    - Hints: APY computation; variable vs. fixed; risk tiers; disclaimers.
  - Liquidation policies, warnings, notifications.
    - Hints: Health factor thresholds; alert channels; protective defaults.
  - TODO Flowchart: Borrow lifecycle and liquidation.
  - TODO Matrix: Risk tiers vs. protocols and assets.
- dApp explorer/hub:
  - Curation criteria, security scoring, permissions sandboxing, phishing detection.
    - Hints: Listing policy; security scans; takedown process; user reporting.
  - In-app browser vs. deep integrations, wallet permissions review/limits.
    - Hints: Permission prompts; per-dapp limits; session reviews.
  - TODO Flowchart: dApp permission request and review.
- Infrastructure:
  - Node providers, indexers, relayers, bundlers, analytics, error tracking.
    - Hints: Redundancy; SLAs; vendor diversity; observability stack.
  - Availability targets, redundancy, incident response.
    - Hints: SLOs/targets; failover plans; drills and RTO/RPO.
  - TODO Diagram: Deployment topology and redundancy.
- Security:
  - Threat model (MFA phishing, SIM swap, device compromise) and mitigations.
    - Hints: Likely attack paths; layered defenses; residual risk and user guidance.
  - Audits, formal verification, bug bounty.
    - Hints: Firms and timelines; scope; bounty tiers; disclosure policy.
  - TODO Diagram: Trust boundaries and threat model.
- Privacy and compliance:
  - PII storage, encryption, retention; GDPR/CCPA handling; consent.
    - Hints: Data minimization; encryption keys; DSAR; consent flows.
  - KYC/AML stance, geofencing, reporting obligations.
    - Hints: Triggers; providers; data sharing; restricted regions.
  - TODO DFD: Personal data flows and consent.
  - TODO Flowchart: KYC/AML trigger paths (if applicable).
- Performance:
  - Latency targets, throughput, scalability plan (bundler capacity, queues).
    - Hints: P95/P99 targets; load assumptions; horizontal scaling; backpressure.
  - TODO Diagram: Queuing/bundling pipeline and capacity planning.
  - TODO Chart: Latency targets vs. measured P95/P99.
- Accessibility and i18n:
  - Languages at launch, accessibility standards, offline/low-bandwidth design.
    - Hints: Locales; WCAG level; text size/contrast; caching for poor networks.
  - TODO Flowchart: Offline/low-bandwidth fallback behavior.

- Transaction safety:
  - Pre-simulation of transactions and human-readable decoding of approvals/transfers.
    - Hints: Sim providers; failure modes; plain-language templates; red flag surfacing.
  - Scam/phishing heuristics, address-poisoning defense, and domain allowlists.
    - Hints: Heuristic sources; update cadence; false-positive handling.
  - Session approvals, transaction risk scoring, and MEV-safe/private submission.
    - Hints: Score inputs; thresholds; use of private relays; fallback rules.
  - TODO Flowchart: Simulation and risk scoring pipeline.

- Approvals and allowances:
  - Visualization of existing allowances and prompts for one-time vs. unlimited approvals.
    - Hints: Default choice; revoke nudges; high-risk token flags.
  - Revoke tooling and reminders; auto-revoke policies and per-dapp limits.
    - Hints: Schedules; triggers; UX entry points; notifications.
  - Allowance risk education and defaults that prefer least privilege.
    - Hints: Tooltips; learn-more; examples of risks and best practice.
  - TODO State Diagram: Allowance lifecycle (grant → monitor → revoke).

- Multi-device and sessions:
  - Session management, logout-all devices, and session timeouts.
    - Hints: Idle timeouts; device list; single-tap revoke; new device alerts.
  - Key rotation flows; compromised/lost device response procedures.
    - Hints: Step-by-step guide; grace periods; support involvement.
  - TODO State Diagram: Session lifecycle across devices.
  - TODO Sequence Diagram: Lost device → recovery.

- Identity and contacts:
  - Contacts/address book, verification status, nicknames, ENS/UD support.
    - Hints: Import sources; deduping; verification badges; privacy choices.
  - Email/handle mapping where applicable; import/export; contact data privacy.
    - Hints: Hashing/pseudonymization; export format; user consent.
  - TODO ERD: Contacts and identity mappings.

- Developer platform:
  - SDKs/APIs, WalletConnect v2, intents, and extension points.
    - Hints: Supported languages; examples; versioning; deprecation policy.
  - Sandbox permissions, rate limits, and developer onboarding.
    - Hints: App review; keys/quotas; abuse prevention.
  - TODO Diagram: SDK architecture and permission model.

- Support and operations:
  - Support channels and SLAs; escalation and incident response runbooks.
    - Hints: Channels (chat/email); severity matrix; on-call rotation.
  - Public status page and transparency reports cadence.
    - Hints: Uptime targets; postmortem template; publication timelines.

- Legal and UX disclosures:
  - Clear fees, sponsored gas limits, and custody disclosures; jurisdictional limitations.
    - Hints: Fee table; gas sponsor caps; non-custodial statement; restricted features/regions.
  - Risk disclosures for bridges, stablecoin depegs, and yield products.
    - Hints: Prominent placement; plain language; links to deeper references.

### Roadmap
- Phased milestones (alpha, beta, mainnet) with dates or quarters.
  - Hints: Scope per phase; success gates; dependencies and risks.
- Feature rollout order (core wallet, gas sponsor, Gmail send, swaps, earn/borrow, hub).
  - Hints: Rationale for sequencing; technical prerequisites; compliance gating.
- Audit and compliance timelines.
  - Hints: Firms, scope, windows; certs/licenses targets and timing.
- Ecosystem partnerships and listing plans.
  - Hints: Targets; criteria; mutual commitments; timelines.
- Regional expansion and support model evolution.
  - Hints: Priority markets; localization; support hours scaling.
- KPI targets by phase (users, MAU, tx/day, revenue, CSAT).
  - Hints: Numeric goals; measurement method; dashboards.

- TODO Timeline: Gantt with milestones and gates; KPI dashboard mock.

### Vision
- Long-term mission and what “decentralized bank” means in 3–5 years.
  - Hints: End-state vision; user rights; custody ethos; inclusivity.
- Differentiation vs. Coinbase Wallet, MetaMask, OKX, etc.
  - Hints: Moat sources (UX, cost, partnerships, standards); defensibility.
- Role of MTX in the ecosystem long-term (governance, utility, incentives).
  - Hints: Powers and limits; alignment with users; sustainability.
- Commitment to openness (standards, SDKs, dev platform).
  - Hints: Open standards adopted; contributions upstream; SDK roadmap.
- Ethical guidelines (user rights, privacy, censorship resistance).
  - Hints: Principles; red lines; transparency commitments.

- TODO Chart: Positioning map vs. major wallets (UX simplicity vs. security; cost vs. features).

### Team & Advisors
- Founders’ bios and relevant experience.
  - Hints: 3–5 lines each; past wins; domain fit; public links.
- Key hires needed (security, compliance, mobile, protocol engineers).
  - Hints: Roles, timing, hiring plan; advisors bridging gaps.
- Advisors and their roles/incentives.
  - Hints: Specific contributions; equity/comp; conflict policies.
- Company entity, jurisdiction, licenses (present/planned).
  - Hints: Legal structure; reasoning; licensing path; counsel.
- Token allocations (team/advisors) and vesting terms.
  - Hints: Percentages; cliffs/vesting; lockups; alignment.

- TODO Diagram: Governance transition (multisig → DAO) with timelines.

### MTX Token — On Ethereum with Total Supply and Decimals
- ✓ Chain(s) and token standard (ERC‑20, extensions), symbol, decimals.
  - Symbol: MTX
  - Network: Ethereum mainnet (L1) at launch; L2/multichain expansion considered post‑launch.
  - Standard: ERC‑20 with EIP‑2612 Permit; Ownable; upgradeable via proxy pattern.
  - Decimals: TBD (evaluating 9 vs. 18; defaulting to 18 unless strong UX/cost rationale for 9).
- ✓ Total supply and mint/burn policy (capped? deflationary mechanisms?).
  - Total supply: 13,000,000 MTX (fixed cap).
  - Mint/burn: disabled for emissions; reserved solely for bridging/canonical multichain support under governance‑controlled minter roles.
- ✓ Contract roles (owner, pauser, minter), upgradeability (proxy?).
  - Upgradeability: proxy‑based with time‑locked upgrades.
  - Pause: circuit breaker (pausable) for emergencies.
  - Ownership: initially a 2‑of‑3 multisig; transfers to DAO once >50% of supply is circulating.
  - Minter roles: disabled by default; may be granted to bridge contracts for multichain support.
  - Permit/sponsored fees: EIP‑2612 Permit; sponsored fees handled at the app/paymaster layer.
  - Transfer hook: optional on‑transfer checks to support compliance/AML policies (configurable).
  - Owner multisig: 2/3 signatures; 24‑hour timelock on privileged actions.
- ✓ Deployer, multisig setup, key management, timelocks.
  - Post‑deploy, ownership transfers to the multisig; signer rotation and hardware key custody policies defined.
  - Multisig policies include a 24‑hour timelock on privileged actions.
- ✓ Audits and renunciation plans.
  - Third‑party audit by Halborn (or comparable tier‑1 firm) prior to launch.
  - Public bug bounty program; phased privilege reduction and potential partial renounce after DAO transition.

- TODO Diagram: Contract architecture (proxy, roles, timelocks) and upgrade process.
### MTX Token — Utility
- Concrete utilities at launch (fee discounts, gas sponsorship access, premium features).
  - Gas sponsorship privileges for MTX stakers; higher caps and lower/zero service fees based on staked amount and lock duration.
  - Hints: Exact benefits; thresholds; UI entitlements.
- ✓ Staking utility (governance power, revenue share eligibility, priority support).
  - Staking yields: rewards paid in MTX, economically supported by gas sponsor revenues; program targets sustainability over dilution.
  - Priority access: stakers receive priority gas sponsorship during liquidity constraints.
  - Governance: voting power activates after >50% circulating and DAO governance is live.
- ✓ Governance scope (treasury, paymaster policy, listings, risk controls).
  - Upon DAO transition, governance controls treasury, paymaster policies, listings, risk parameters, and upgrade approvals within defined guardrails.
- In-app incentives (referrals, cashbacks, quests) funded by what pool.
  - None at launch; may be proposed via governance.
  - Hints: Budget; emission rate; abuse prevention; sunset criteria.
- ✓ Does MTX unlock higher gas sponsor caps or earn/borrow benefits?
  - MTX staking unlocks higher gas sponsor caps and discounted rates via a dedicated staker pool.

- TODO Table: Staking tiers vs. gas sponsor caps/discounts; governance scope overview.
### MTX Token — Tokenomics
- ✓ Initial liquidity:
  - Confirm: 1% of supply deposited to DEX at $0.50 initial price on Uniswap v4 (Ethereum).
    - Fee tier: 0.30%; full‑range position; LP tokens locked.
    - Pair: MTX/USDC or MTX/USDT (final selection at deployment based on liquidity depth).
  - Initial market cap and FDV implications.
    - Fixed supply: 13M MTX; initial circulating ~1% → initial market cap ≈ $6.5M at $0.50.
    - Max circulating after d days: 1% + 0.3% × d (subject to refreeze policy below).
    - Refreeze policy: Foundation may refreeze unlocked tokens to smooth supply and support market health; operations funded transparently from unlocked amounts.
  - TODO Chart: Initial liquidity configuration and price impact simulation.
- ✓ Emissions/unlock:
  - Confirm: daily 0.3% of total supply “unfrozen” to Matrix Foundation.
    - On‑chain schedule; no cliff. Minimum effective vesting horizon ≈ 333 days at 0.3%/day.
    - Publicly verifiable via contract state and on‑chain transactions.
    - Hints: On-chain schedule; cliff?; how displayed to public.
  - Define “freeze/refreeze” mechanics (on-chain vesting? timelock? CEO discretion boundaries?).
    - Freeze/refreeze fully on‑chain. Discretion exercised within published policy; governance oversight and periodic reporting ensure accountability.
    - Hints: Controls; governance oversight; transparency rules.
  - Clear policy for selling to fund ops vs. refreezing; transparency and reporting cadence.
    - All sales/buys executed on‑chain (transparent). Monthly/quarterly reports disclose unlocks, sales, refreezes, and treasury balances.
    - Hints: Triggers; ceilings; monthly reports; wallet disclosures.
  - TODO Chart: Daily unlock/refreeze over time (stacked area).
- ✓ Allocations:
  - Foundation, ecosystem, community, team, advisors, market making, reserves.
    - 1% initial LP; remainder held by Foundation and subject to the daily unlock policy.
    - No team or airdrop allocations at launch; any marketing allocations purchased on‑market using company capital to avoid preferential distributions.
    - Market‑making: on‑chain liquidity operations using unlocked amounts for stabilization and insurance; profits accrue to company capital to deepen liquidity or extend runway.
    - Hints: Percentages; lockups; purpose per bucket.
  - TODO Pie Chart: Token allocation by bucket.
  - Vesting cliffs/schedules; anti-dump protections; lockups for insiders.
    - Anti‑dump measures focus on transparent refreeze capability and liquidity management; monitoring for market manipulation with proportionate responses consistent with decentralization and user rights.
    - Hints: Timelines; transfer restrictions; enforcement.
- ✓ Treasury and reserves:
  - Insurance account vs. profit account definitions, controls, signers, auditability.
    - Revenues split: 50% Insurance Account (market stabilization/buybacks), 50% Profit Account (operations, staking rewards support, market‑making, growth).
    - Hints: Multisig details; access policy; public dashboards.
  - TODO Flow Diagram: Treasury flows (revenue → insurance/profit → uses).
- ✓ Staking and rewards:
  - Reward source (revenue share vs. emissions), distribution frequency (block/weekly/monthly).
    - Monthly distributions; paid in MTX and/or stablecoins (USDC/USDT) depending on treasury composition.
    - Rewards scale with staked amount and lock duration; formula to be published.
    - Hints: Split ratios; schedule; auto-compound; gas costs.
  - Eligibility (stakers only vs. all holders), snapshot mechanism, slashing conditions if any.
    - Minimum stake: 100 MTX (≈0.0008% of supply; ≈0.077% of initial LP float).
  - TODO Formula: Staking rewards calculation; TODO Chart: APR vs. stake and duration.
- ✓ Buybacks and burns:
  - Triggers (revenue thresholds, governance votes), execution rules.
    - Buybacks executed opportunistically based on treasury health and market conditions; rules codified in treasury policy and reported transparently.
    - Hints: Conditions; execution venues; transparency.
  - TODO Flowchart: Buyback/burn decision process.
- ✓ Compliance:
  - Security vs. utility token stance, jurisdictions, offering status, KYC requirements.
    - Wallet usage and staking do not require KYC by default. In cases of suspected fraud/abuse related to sponsored services or treasury interactions, enhanced verification may be requested to protect the ecosystem.
    - Hints: Legal opinions (if any); countries included/excluded; investor eligibility.
  - TODO Flowchart: Enhanced verification triggers and handling.


### MTX Token — Market and Revenue Forecast
- Revenue drivers and assumptions:
  - Breakdown of the ~$500K/month at 5M users (ARPU, conversion, take rates).
    - Hints: Assumptions per line; sensitivity; comps.
  - Sources: swap fees/spread, earn referral/APR share, borrow margins, premium plans,
    interchange/partners, ad or listing fees in hub.
    - Hints: Expected mix; seasonality; contractual certainty.
  - Gas sponsorship cost model and net margin impact.
    - Hints: Per-user cost; cap utilization; gas price scenarios.
- User growth model:
  - Acquisition channels, CAC, referral mechanics, target geographies.
    - Hints: Channel mix; paid vs. organic; referral incentives.
  - Retention levers and power users.
    - Hints: Habit loops; cohorts; features that drive stickiness.
- Cost structure:
  - Infra (nodes, bundlers, relayers), security/audits, compliance/legal, support, R&D.
    - Hints: Fixed vs. variable; scaling with users; vendors.
- Unit economics:
  - Payback period, breakeven MAU, sensitivity to gas price and volatility.
    - Hints: LTV/CAC; margin by product; stress tests.
- Scenarios:
  - Base/bear/bull projections for 24–36 months with key risks.
    - Hints: Key drivers; downside mitigations; leading indicators.

### References & Disclaimer
- Technical references (standards, protocols), third-party integrations.
  - Hints: EIPs; protocol docs; integration guides.
- Legal disclaimers (not investment advice, forward-looking statements, risk factors).
  - Hints: Jurisdiction-specific wording; prominence.
- Regional restrictions and eligibility.
  - Hints: Country list; age limits; feature gating.
- Data and metrics sources.
  - Hints: Internal dashboards; third-party analytics; timestamps.
- Brand and trademark notices.
  - Hints: Ownership; permitted uses; contact.

### Optional Clarifications (If Helpful)
- Competitive landscape and positioning map.
  - Hints: Axes that matter (UX vs. security; cost vs. features); key competitors.
- Governance framework details (vote types, quorums, delegation).
  - Hints: Voting mechanisms; thresholds; delegation rules.
- Risk management (bridge risk, stablecoin depegs, protocol insolvency).
  - Hints: Risk taxonomy; monitoring; mitigations; insurance.
- Customer support SLAs and incident response.
  - Hints: Severity levels; response/resolve targets; comms.
- Business continuity planning and disaster recovery.
  - Hints: Backup plans; RTO/RPO; drills.

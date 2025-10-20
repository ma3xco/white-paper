# Matrix Wallet: The Decentralized Bank for Everyone - White Paper
Answer directly under each section (brief bullets are fine). Once filled, we will convert this into the first full draft.

### Abstract
- What single sentence best describes Matrix Wallet’s core value for mass adoption?
  - Hints: One crisp promise; who it's for; key differentiator vs. existing wallets.
- Who is the primary audience (first-time users, Web3 natives, SMEs, remittance users)?
  - I dont know the exact word for this, our primary audiance are every person, we want to get mass adoption. 
    I 
  - Hints: Segments, geographies, devices, income bands, compliance needs.
- What problem do you solve better than existing wallets/banks (onboarding, UX, gas, security)?
  - Hints: Quantify friction today (steps/time/cost); name the top 3 pain points you remove.
- What are the 3–5 flagship features that make it “a decentralized bank for everyone”?
  - Hints: Tie features to outcomes; note what’s novel vs. table stakes; launch readiness.
- What measurable outcomes do you aim for (e.g., 5M users, <$0.05 effective tx cost, NPS)?
  - Hints: Targets and timeframes; core metrics (MAU, retention, CSAT); baselines.
- What is the core economic model in one sentence (MTX role, revenue, distribution)?
  - Hints: Revenue sources, MTX utility, how value accrues and distributes; sustainability.
- What chains and assets are supported at launch?
  - Hints: Initial chains/L2s; stablecoins; token standards; expansion plan.

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

### Solution Overview
- What type of wallet is Matrix: non-custodial smart account (AA/4337), EOA, hybrid, or custodial?
  - Hints: Tradeoffs (UX vs. trust); upgradeability; standards supported; compliance impact.
- How do users onboard (email/social signup, OAuth with Google, seedless, social recovery)?
  - Hints: Step-by-step flow; fallback paths; recovery setup defaults; bot/Sybil defenses.
- What makes the UI “grandparent-simple” (flows, language, defaults, accessibility)?
  - Hints: Plain language; safe defaults; large touch targets; WCAG; cognitive load.
- How does “gas sponsored transfer” work at a high level (who pays, limits, eligibility)?
  - Hints: Funding source; per-user caps; eligible tx types; abuse prevention; reporting.
- How does “send using Gmail” work conceptually (identity mapping, verification, privacy)?
  - Hints: OAuth scopes/consent; email↔address mapping; recipient claim UX; data privacy.
- What core banking-like features are included at launch (send/receive, swap, earn, borrow)?
  - Hints: MVP vs. later; dependencies; jurisdictional restrictions; disclosures.
- Which chains/networks and assets are supported initially vs. later?
  - Hints: Rationale for choices; bridging approach; roadmap milestones.
- What’s your trust model and key security guarantees to users?
  - Hints: Non-custodial stance; third-party reliance; incident response commitments.
- How are approvals/allowances handled to minimize risk and simplify UX?
  - Hints: One-time vs. unlimited defaults; revoke flow; proactive alerts; education.
- What is the multi-device experience (sessions, sync, recovery across devices)?
  - Hints: Device binding; session revocation; key sync; lost device recovery.
- What support/operations guarantees exist (SLA, incident status, transparency)?
  - Hints: Channels/hours; response SLAs; status page; postmortems cadence.

### Solution Details — Technical Specification
- Wallet/account model:
  - Smart account standard (ERC‑4337/AA)? Paymaster? Bundler? Session keys?
    - Hints: Why 4337; bundler providers/SLAs; session key scopes/durations; upgrade path.
  - Key management (MPC, device keys, passkeys, socials), social recovery policy, multi-device.
    - Hints: Thresholds/shares; backup strategy; guardian rules; device provisioning.
  - Recovery flows and anti-phishing mechanisms.
    - Hints: Time-locks; multi-factor confirmations; phishing education; usability tests.
- Gas sponsorship:
  - Sponsorship policy (per-user caps, whitelists, geos), fraud prevention, abuse limits.
    - Hints: Caps/eligibility; Sybil detection; geo policy; logging and rate limits.
  - Who funds it (treasury, MTX staking pool)? Budgeting and monitoring.
    - Hints: Budget ceilings; on/off switch; reporting frequency; governance levers.
- Send using Gmail:
  - Identity resolution (email ↔ address mapping), verification (OAuth scope), consent UI.
    - Hints: Scopes needed; consent wording; uniqueness handling; opt-out/revoke.
  - Handling email changes, revocation, spoofing prevention, privacy, data retention.
    - Hints: Change detection; secure remapping; audit trails; retention windows.
  - Delivery UX for recipients without wallets (claim flow, expiration, fallback).
    - Hints: Gasless claim; expiry; re-route funds; custodial fallback policy.
- Payments and transfers:
  - Supported token standards, stablecoins, fiat on/off-ramps, compliance checks (sanctions).
    - Hints: Initial stablecoins; partners for on/off-ramp; screening provider; limits.
  - Cross-chain strategy (bridges, messaging, risks).
    - Hints: Chosen bridges; risk disclosures; fallback routes; insurance/escrow.
- Swap:
  - Aggregator(s) (0x, 1inch, Paraswap), routing, MEV protection, slippage controls.
    - Hints: Aggregators used; private orderflow; max slippage; simulation and quotes.
  - Fees/spreads and who receives them.
    - Hints: Fee schedule; recipients (treasury/MTX); disclosure in UI.
- Earn and borrow:
  - Integrated protocols (Aave/Compound/Lido/etc.) vs. native offerings.
    - Hints: Whitelisting criteria; audits; custody of assets; oracle dependencies.
  - Risk disclosures, APY sources, smart-contract risk, custody of collateral.
    - Hints: APY computation; variable vs. fixed; risk tiers; disclaimers.
  - Liquidation policies, warnings, notifications.
    - Hints: Health factor thresholds; alert channels; protective defaults.
- dApp explorer/hub:
  - Curation criteria, security scoring, permissions sandboxing, phishing detection.
    - Hints: Listing policy; security scans; takedown process; user reporting.
  - In-app browser vs. deep integrations, wallet permissions review/limits.
    - Hints: Permission prompts; per-dapp limits; session reviews.
- Infrastructure:
  - Node providers, indexers, relayers, bundlers, analytics, error tracking.
    - Hints: Redundancy; SLAs; vendor diversity; observability stack.
  - Availability targets, redundancy, incident response.
    - Hints: SLOs/targets; failover plans; drills and RTO/RPO.
- Security:
  - Threat model (MFA phishing, SIM swap, device compromise) and mitigations.
    - Hints: Likely attack paths; layered defenses; residual risk and user guidance.
  - Audits, formal verification, bug bounty.
    - Hints: Firms and timelines; scope; bounty tiers; disclosure policy.
- Privacy and compliance:
  - PII storage, encryption, retention; GDPR/CCPA handling; consent.
    - Hints: Data minimization; encryption keys; DSAR; consent flows.
  - KYC/AML stance, geofencing, reporting obligations.
    - Hints: Triggers; providers; data sharing; restricted regions.
- Performance:
  - Latency targets, throughput, scalability plan (bundler capacity, queues).
    - Hints: P95/P99 targets; load assumptions; horizontal scaling; backpressure.
- Accessibility and i18n:
  - Languages at launch, accessibility standards, offline/low-bandwidth design.
    - Hints: Locales; WCAG level; text size/contrast; caching for poor networks.

- Transaction safety:
  - Pre-simulation of transactions and human-readable decoding of approvals/transfers.
    - Hints: Sim providers; failure modes; plain-language templates; red flag surfacing.
  - Scam/phishing heuristics, address-poisoning defense, and domain allowlists.
    - Hints: Heuristic sources; update cadence; false-positive handling.
  - Session approvals, transaction risk scoring, and MEV-safe/private submission.
    - Hints: Score inputs; thresholds; use of private relays; fallback rules.

- Approvals and allowances:
  - Visualization of existing allowances and prompts for one-time vs. unlimited approvals.
    - Hints: Default choice; revoke nudges; high-risk token flags.
  - Revoke tooling and reminders; auto-revoke policies and per-dapp limits.
    - Hints: Schedules; triggers; UX entry points; notifications.
  - Allowance risk education and defaults that prefer least privilege.
    - Hints: Tooltips; learn-more; examples of risks and best practice.

- Multi-device and sessions:
  - Session management, logout-all devices, and session timeouts.
    - Hints: Idle timeouts; device list; single-tap revoke; new device alerts.
  - Key rotation flows; compromised/lost device response procedures.
    - Hints: Step-by-step guide; grace periods; support involvement.

- Identity and contacts:
  - Contacts/address book, verification status, nicknames, ENS/UD support.
    - Hints: Import sources; deduping; verification badges; privacy choices.
  - Email/handle mapping where applicable; import/export; contact data privacy.
    - Hints: Hashing/pseudonymization; export format; user consent.

- Developer platform:
  - SDKs/APIs, WalletConnect v2, intents, and extension points.
    - Hints: Supported languages; examples; versioning; deprecation policy.
  - Sandbox permissions, rate limits, and developer onboarding.
    - Hints: App review; keys/quotas; abuse prevention.

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

### MTX Token — On Ethereum with Total Supply and Decimals
- ✓ Chain(s) and token standard (ERC‑20, extensions), symbol, decimals.
  - Symbol: MTX
  - Type: ERC-20, Permit, Ownable, Upgradable, 
  - Network: Ethereum
  - Decimals: 9 ? (6,8,9,12,18)
- ✓ Total supply and mint/burn policy (capped? deflationary mechanisms?).
  - Total Supply : 13M 
  - mint and burn is reserved for multichain and bridge support.
- ✓ Contract roles (owner, pauser, minter), upgradeability (proxy?).
  - Proxied ( upgradable )
  - Pusable in the case of emergency. 
  - Ownable, Ownership will moved to DAO Once more than 50% token released and circulating.
  - Minters will be set by owner if required for bridge or multichain token.
  - Permit + Authorized transfer + Authorized Transfer + sponsor fee.
  - Transfer Hook for flexiable AML
  - Owner : Multisig Wallet with 2/3 signature for executing.
- ✓ Deployer, multisig setup, key management, timelocks.
  - Owner will be multisig wallet, after deployment the Ownership will transfer to multisig wallet.
  - Owner Multisig have 1D treshold for execution. 
- Audits and renunciation plans.
  - Will audit by Helborn Team.
  - Bug bounty program

### MTX Token — Utility
- Concrete utilities at launch (fee discounts, gas sponsorship access, premium features).
  - Gas Sponsorship with Zero Fee for MTX Stakers based on amount and duration.
  - Hints: Exact benefits; thresholds; UI entitlements.
- Staking utility (governance power, revenue share eligibility, priority support).
  - Hints: Requirements; lockups; yields; risks.
- Governance scope (treasury, paymaster policy, listings, risk controls).
  - Hints: What can/can’t be changed; quorum/thresholds; voter eligibility.
- In-app incentives (referrals, cashbacks, quests) funded by what pool.
  - Hints: Budget; emission rate; abuse prevention; sunset criteria.
- Does MTX unlock higher gas sponsor caps or earn/borrow benefits?
  - Hints: Tiers; examples; caps; fairness.

### MTX Token — Tokenomics
- Initial liquidity:
  - Confirm: 1% of supply deposited to DEX at $0.50 initial price. Which DEX/pool params?
    - Hints: DEX/pair; initial liquidity USD; fee tier; price range; lock.
  - Initial market cap and FDV implications.
    - Hints: Circulating vs. FDV math; narratives; comparison set.
- Emissions/unlock:
  - Confirm: daily 0.3% of total supply “unfrozen” to Matrix Foundation.
    - Hints: On-chain schedule; cliff?; how displayed to public.
  - Define “freeze/refreeze” mechanics (on-chain vesting? timelock? CEO discretion boundaries?).
    - Hints: Controls; governance oversight; transparency rules.
  - Clear policy for selling to fund ops vs. refreezing; transparency and reporting cadence.
    - Hints: Triggers; ceilings; monthly reports; wallet disclosures.
- Allocations:
  - Foundation, ecosystem, community, team, advisors, market making, reserves.
    - Hints: Percentages; lockups; purpose per bucket.
  - Vesting cliffs/schedules; anti-dump protections; lockups for insiders.
    - Hints: Timelines; transfer restrictions; enforcement.
- Treasury and reserves:
  - Insurance account vs. profit account definitions, controls, signers, auditability.
    - Hints: Multisig details; access policy; public dashboards.
- Staking and rewards:
  - Reward source (revenue share vs. emissions), distribution frequency (block/weekly/monthly).
    - Hints: Split ratios; schedule; auto-compound; gas costs.
  - Eligibility (stakers only vs. all holders), snapshot mechanism, slashing conditions if any.
    - Hints: Min stake; snapshot cadence; penalties.
- Buybacks and burns:
  - Triggers (revenue thresholds, governance votes), execution rules.
    - Hints: Conditions; execution venues; transparency.
- Compliance:
  - Security vs. utility token stance, jurisdictions, offering status, KYC requirements.
    - Hints: Legal opinions (if any); countries included/excluded; investor eligibility.

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

# Matrix Wallet: The Decentralized Bank for Everyone - White Paper
Answer directly under each section (brief bullets are fine). Once filled, we will convert this into the first full draft.

### Abstract
- What single sentence best describes Matrix Wallet’s core value for mass adoption?
- Who is the primary audience (first-time users, Web3 natives, SMEs, remittance users)?
- What problem do you solve better than existing wallets/banks (onboarding, UX, gas, security)?
- What are the 3–5 flagship features that make it “a decentralized bank for everyone”?
- What measurable outcomes do you aim for (e.g., 5M users, <$0.05 effective tx cost, NPS)?
- What is the core economic model in one sentence (MTX role, revenue, distribution)?
- What chains and assets are supported at launch?

### Introduction & Problem Statement
- What specific frictions block mass adoption today (seed phrases, fees, volatility, scams)?
- What real-world use cases are you targeting first (P2P, remittances, small-business payments)?
- Who are your key personas (e.g., “grandfather” user profile) and their top 3 needs?
- What is broken in “crypto wallets as banks” today (custody, fees, reliability, UX)?
- What regulatory/trust concerns do target users have and how will you address them?
- What success criteria define “solved” (time to first transaction, cost, support responsiveness)?

### Solution Overview
- What type of wallet is Matrix: non-custodial smart account (AA/4337), EOA, hybrid, or custodial?
- How do users onboard (email/social signup, OAuth with Google, seedless, social recovery)?
- What makes the UI “grandparent-simple” (flows, language, defaults, accessibility)?
- How does “gas sponsored transfer” work at a high level (who pays, limits, eligibility)?
- How does “send using Gmail” work conceptually (identity mapping, verification, privacy)?
- What core banking-like features are included at launch (send/receive, swap, earn, borrow)?
- Which chains/networks and assets are supported initially vs. later?
- What’s your trust model and key security guarantees to users?
- How are approvals/allowances handled to minimize risk and simplify UX?
- What is the multi-device experience (sessions, sync, recovery across devices)?
- What support/operations guarantees exist (SLA, incident status, transparency)?

### Solution Details — Technical Specification
- Wallet/account model:
  - Smart account standard (ERC‑4337/AA)? Paymaster? Bundler? Session keys?
  - Key management (MPC, device keys, passkeys, socials), social recovery policy, multi-device.
  - Recovery flows and anti-phishing mechanisms.
- Gas sponsorship:
  - Sponsorship policy (per-user caps, whitelists, geos), fraud prevention, abuse limits.
  - Who funds it (treasury, MTX staking pool)? Budgeting and monitoring.
- Send using Gmail:
  - Identity resolution (email ↔ address mapping), verification (OAuth scope), consent UI.
  - Handling email changes, revocation, spoofing prevention, privacy, data retention.
  - Delivery UX for recipients without wallets (claim flow, expiration, fallback).
- Payments and transfers:
  - Supported token standards, stablecoins, fiat on/off-ramps, compliance checks (sanctions).
  - Cross-chain strategy (bridges, messaging, risks).
- Swap:
  - Aggregator(s) (0x, 1inch, Paraswap), routing, MEV protection, slippage controls.
  - Fees/spreads and who receives them.
- Earn and borrow:
  - Integrated protocols (Aave/Compound/Lido/etc.) vs. native offerings.
  - Risk disclosures, APY sources, smart-contract risk, custody of collateral.
  - Liquidation policies, warnings, notifications.
- dApp explorer/hub:
  - Curation criteria, security scoring, permissions sandboxing, phishing detection.
  - In-app browser vs. deep integrations, wallet permissions review/limits.
- Infrastructure:
  - Node providers, indexers, relayers, bundlers, analytics, error tracking.
  - Availability targets, redundancy, incident response.
- Security:
  - Threat model (MFA phishing, SIM swap, device compromise) and mitigations.
  - Audits, formal verification, bug bounty.
- Privacy and compliance:
  - PII storage, encryption, retention; GDPR/CCPA handling; consent.
  - KYC/AML stance, geofencing, reporting obligations.
- Performance:
  - Latency targets, throughput, scalability plan (bundler capacity, queues).
- Accessibility and i18n:
  - Languages at launch, accessibility standards, offline/low-bandwidth design.

- Transaction safety:
  - Pre-simulation of transactions and human-readable decoding of approvals/transfers.
  - Scam/phishing heuristics, address-poisoning defense, and domain allowlists.
  - Session approvals, transaction risk scoring, and MEV-safe/private submission.

- Approvals and allowances:
  - Visualization of existing allowances and prompts for one-time vs. unlimited approvals.
  - Revoke tooling and reminders; auto-revoke policies and per-dapp limits.
  - Allowance risk education and defaults that prefer least privilege.

- Multi-device and sessions:
  - Session management, logout-all devices, and session timeouts.
  - Key rotation flows; compromised/lost device response procedures.

- Identity and contacts:
  - Contacts/address book, verification status, nicknames, ENS/UD support.
  - Email/handle mapping where applicable; import/export; contact data privacy.

- Developer platform:
  - SDKs/APIs, WalletConnect v2, intents, and extension points.
  - Sandbox permissions, rate limits, and developer onboarding.

- Support and operations:
  - Support channels and SLAs; escalation and incident response runbooks.
  - Public status page and transparency reports cadence.

- Legal and UX disclosures:
  - Clear fees, sponsored gas limits, and custody disclosures; jurisdictional limitations.
  - Risk disclosures for bridges, stablecoin depegs, and yield products.

### Roadmap
- Phased milestones (alpha, beta, mainnet) with dates or quarters.
- Feature rollout order (core wallet, gas sponsor, Gmail send, swaps, earn/borrow, hub).
- Audit and compliance timelines.
- Ecosystem partnerships and listing plans.
- Regional expansion and support model evolution.
- KPI targets by phase (users, MAU, tx/day, revenue, CSAT).

### Vision
- Long-term mission and what “decentralized bank” means in 3–5 years.
- Differentiation vs. Coinbase Wallet, MetaMask, OKX, etc.
- Role of MTX in the ecosystem long-term (governance, utility, incentives).
- Commitment to openness (standards, SDKs, dev platform).
- Ethical guidelines (user rights, privacy, censorship resistance).

### Team & Advisors
- Founders’ bios and relevant experience.
- Key hires needed (security, compliance, mobile, protocol engineers).
- Advisors and their roles/incentives.
- Company entity, jurisdiction, licenses (present/planned).
- Token allocations (team/advisors) and vesting terms.

### MTX Token — On Ethereum with Total Supply and Decimals
- Chain(s) and token standard (ERC‑20, extensions), symbol, decimals.
- Total supply and mint/burn policy (capped? deflationary mechanisms?).
- Contract roles (owner, pauser, minter), upgradeability (proxy?).
- Deployer, multisig setup, key management, timelocks.
- Audits and renunciation plans.

### MTX Token — Utility
- Concrete utilities at launch (fee discounts, gas sponsorship access, premium features).
- Staking utility (governance power, revenue share eligibility, priority support).
- Governance scope (treasury, paymaster policy, listings, risk controls).
- In-app incentives (referrals, cashbacks, quests) funded by what pool.
- Does MTX unlock higher gas sponsor caps or earn/borrow benefits?

### MTX Token — Tokenomics
- Initial liquidity:
  - Confirm: 1% of supply deposited to DEX at $0.50 initial price. Which DEX/pool params?
  - Initial market cap and FDV implications.
- Emissions/unlock:
  - Confirm: daily 0.3% of total supply “unfrozen” to Matrix Foundation.
  - Define “freeze/refreeze” mechanics (on-chain vesting? timelock? CEO discretion boundaries?).
  - Clear policy for selling to fund ops vs. refreezing; transparency and reporting cadence.
- Allocations:
  - Foundation, ecosystem, community, team, advisors, market making, reserves.
  - Vesting cliffs/schedules; anti-dump protections; lockups for insiders.
- Treasury and reserves:
  - Insurance account vs. profit account definitions, controls, signers, auditability.
- Staking and rewards:
  - Reward source (revenue share vs. emissions), distribution frequency (block/weekly/monthly).
  - Eligibility (stakers only vs. all holders), snapshot mechanism, slashing conditions if any.
- Buybacks and burns:
  - Triggers (revenue thresholds, governance votes), execution rules.
- Compliance:
  - Security vs. utility token stance, jurisdictions, offering status, KYC requirements.

### MTX Token — Market and Revenue Forecast
- Revenue drivers and assumptions:
  - Breakdown of the ~$500K/month at 5M users (ARPU, conversion, take rates).
  - Sources: swap fees/spread, earn referral/APR share, borrow margins, premium plans,
    interchange/partners, ad or listing fees in hub.
  - Gas sponsorship cost model and net margin impact.
- User growth model:
  - Acquisition channels, CAC, referral mechanics, target geographies.
  - Retention levers and power users.
- Cost structure:
  - Infra (nodes, bundlers, relayers), security/audits, compliance/legal, support, R&D.
- Unit economics:
  - Payback period, breakeven MAU, sensitivity to gas price and volatility.
- Scenarios:
  - Base/bear/bull projections for 24–36 months with key risks.

### References & Disclaimer
- Technical references (standards, protocols), third-party integrations.
- Legal disclaimers (not investment advice, forward-looking statements, risk factors).
- Regional restrictions and eligibility.
- Data and metrics sources.
- Brand and trademark notices.

### Optional Clarifications (If Helpful)
- Competitive landscape and positioning map.
- Governance framework details (vote types, quorums, delegation).
- Risk management (bridge risk, stablecoin depegs, protocol insolvency).
- Customer support SLAs and incident response.
- Business continuity planning and disaster recovery.

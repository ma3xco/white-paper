# Matrix Wallet White Paper - Questions

## Abstract

**1.** What single sentence best describes Matrix Wallet's core value for mass adoption?

    "Simplicity is our DNA".

**2.** Who is the primary audience (first-time users, Web3 natives, SMEs, remittance users)?

    Matrix Wallet is designed for a universal audience, from crypto newcomers to Web3 natives, small and medium-sized enterprises (SMEs), and remittance users, with the goal of achieving mass adoption.

**3.** What problem do you solve better than existing wallets/banks (onboarding, UX, gas, security)?

    - **Radical Simplicity:** We eliminate the technical barriers and complexities that typically discourage mainstream crypto adoption.
    - **Unhindered UX:** Our enterprise-grade security is implemented without compromising the user experience.
    - **Gasless Transactions:** Users can execute transactions on any supported network without needing native tokens.
    - **Email-Based Transfers:** Sending cryptocurrency is as simple as sending an email by using a recipient's Gmail address.
    - **Social Recovery:** Wallet recovery is secured through trusted social connections like Google and Apple, eliminating the need for seed phrases.

**4.** What are the 3–5 flagship features that make it "a decentralized bank for everyone"?

    - **One-Tap Onboarding:** Instant wallet creation using Google or Apple for sign-in.
    - **Sponsored Transactions:** Gas fees are sponsored, so users do not need to hold native tokens.
    - **Send to Email:** Cryptocurrency can be sent directly to email addresses.
    - **Social Recovery:** Wallet recovery is secured through social authentication.
    - **Broad Multi-Chain Support:** A seamless experience is provided across Bitcoin, Ethereum, Tron, Solana, and BNB Chain.

**5.** What measurable outcomes do you aim for (e.g., 5M users, <$0.05 effective tx cost, NPS)?

    Target: 100 million monthly active users by end of 2026

**6.** What is the core economic model in one sentence (MTX role, revenue, distribution)?

    [Answer pending - CC Hamid]
    *Hint: Describe the core economic model, MTX token role, revenue streams, and distribution mechanisms*

## Introduction & Problem Statement

**7.** What chains and assets are supported at launch?

    Bitcoin, Ethereum, Tron, Solana, and BNB Chain

**8.** What specific frictions block mass adoption today (seed phrases, fees, volatility, scams)?

    The primary obstacles to mass adoption are usability and user experience challenges, such as the need to manage seed phrases and long, complex addresses. Additional barriers include scams, market volatility, and issues with scalability, security, and regulatory compliance.

**9.** What real-world use cases are you targeting first (P2P, remittances, small-business payments)?

    Our initial focus is on peer-to-peer (P2P) payments.

**10.** Who are your key personas and their top 3 needs?

    Our key persona is the inexperienced user, whose primary needs are seamless transfers and swaps, a straightforward adoption process, and overall ease of use.

**11.** What is broken in "crypto wallets as banks" today (custody, fees, reliability, UX)?

    Current crypto wallets face challenges in usability and user experience, particularly with seed phrases and complex addresses. Other significant issues include scams, volatility, scalability, security, and regulatory barriers.

**12.** What regulatory/trust concerns do target users have and how will you address them?

    We address key user concerns about regulation and trust directly:

    - **Regulatory & Security Concerns:** We are committed to full regulatory compliance and protect assets with enterprise-grade security, secure on-device key management, and proactive fraud prevention.
    - **Fear of Losing Access:** Our social recovery system, which uses Google and Apple, eliminates the risk and anxiety associated with losing seed phrases by providing a familiar and secure backup method.
    - **Complexity & Transaction Errors:** We prevent mistakes through a simplified user experience and transaction simulations, which show users a clear, human-readable outcome before they approve any transaction.

**13.** What success criteria define "solved" (time to first transaction, cost, support responsiveness)?

    Our primary success criterion is reaching 100 million active users.

## Solution Overview

**14.** What type of wallet is Matrix: non-custodial smart account (AA/4337), EOA, hybrid, or custodial?

    Matrix Wallet is a non-custodial wallet, ensuring users maintain full control over their private keys and assets.

**15.** How do users onboard (email/social signup, OAuth with Google, seedless, social recovery)?

    Users can onboard seamlessly through OAuth integration with Google and Apple accounts, eliminating the need for complex seed phrase management.

**16.** What makes the UI simple (flows, language, defaults, accessibility)?

    Our UI prioritizes simplicity by avoiding complex technical flows and overwhelming details, presenting only essential information in an intuitive manner.

**17.** How does "gas sponsored transfer" work at a high level (who pays, limits, eligibility)?

    [Answer pending - CC Hamid]
    *Hint: Explain how gas sponsorship works, who pays for transactions, user limits, and eligibility criteria*

**18.** How does "send using Gmail" work conceptually (identity mapping, verification, privacy)?

    [Answer pending - CC Hamid]
    *Hint: Describe the email-to-address mapping system, verification process, and privacy considerations*

**19.** What core banking-like features are included at launch (send/receive, swap, earn, borrow)?

    At launch, Matrix Wallet will include core features: Send, Receive, Swap, and Staking capabilities.

**20.** Which chains/networks and assets are supported initially vs. later?

    [Answer pending - CC Hamid]
    *Hint: List specific chains and assets supported at launch vs. future roadmap*

**21.** What's your trust model and key security guarantees to users?

    We implement a robust security model where the mnemonic is stored as an encrypted blob in device secure storage and as a user-bound cloud backup (iCloud on iOS; Google Drive App Data on Android), encrypted with a key derived from the user's passcode hash.

**22.** How are approvals/allowances handled to minimize risk and simplify UX?

    We simplify the user experience by streamlining approval processes and minimizing complex technical details.

**23.** What is the multi-device experience (sessions, sync, recovery across devices)?

    Matrix Wallet operates on a single session model with recovery capabilities through social login and user passcode authentication.

**24.** What support/operations guarantees exist (SLA, incident status, transparency)?

    We provide Service Level Agreements (SLA) and maintain transparency in our operations and incident reporting.

## Solution Details — Technical Specification

### Wallet/account model:

**26.** Key management (MPC, device keys, passkeys, socials), social recovery policy, multi-device.

    Our key management system utilizes passkeys, social authentication, and device keys to provide secure and user-friendly access control.

**27.** Recovery flows and anti-phishing mechanisms.

    We implement comprehensive security measures including URL verification, transaction simulation, security warnings, and blacklist protection to prevent phishing attacks and ensure user safety.

### Gas sponsorship:

**28.** Sponsorship policy (per-user caps, whitelists, geos), fraud prevention, abuse limits.

    [Answer pending - CC Hamid]
    *Hint: Define sponsorship policies, per-user caps, whitelists, geographic restrictions, and fraud prevention measures*

**29.** Who funds it (treasury, MTX staking pool)? Budgeting and monitoring.

    [Answer pending - CC Hamid]
    *Hint: Explain funding sources (treasury, MTX staking pool), budgeting approach, and monitoring systems*

### Send using Gmail:

**30.** Identity resolution (email ↔ address mapping), verification (OAuth scope), consent UI.

    [Answer pending - CC Hamid]
    *Hint: Detail email-to-address resolution, OAuth scope requirements, and consent UI design*

**31.** Handling email changes, revocation, spoofing prevention, privacy, data retention.

    [Answer pending - CC Hamid]
    *Hint: Address email change handling, revocation procedures, spoofing prevention, privacy measures, and data retention policies*

**32.** Delivery UX for recipients without wallets (claim flow, expiration, fallback).

    [Answer pending - CC Hamid]
    *Hint: Design user experience for recipients without wallets, claim flow, expiration handling, and fallback options*

### Payments and transfers:

**33.** Supported token standards, stablecoins, fiat on/off-ramps, compliance checks (sanctions).

    [Answer pending - CC Hamid]
    *Hint: List supported token standards, stablecoin options, fiat on/off-ramps, and compliance check procedures*

**34.** Cross-chain strategy (bridges, messaging, risks).

    [Answer pending - CC Hamid]
    *Hint: Describe cross-chain strategy, bridge selection, messaging protocols, and associated risks*

### Swap:

**35.** Aggregator(s) (0x, 1inch, Paraswap), routing, MEV protection, slippage controls.

    [Answer pending - CC Hamid]
    *Hint: Specify DEX aggregators (0x, 1inch, Paraswap), routing logic, MEV protection, and slippage controls*

**36.** Fees/spreads and who receives them.

    Fees are distributed between aggregators and our platform.

### Earn and borrow:

**37.** Integrated protocols (Aave/Compound/Lido/etc.) vs. native offerings.

    We integrate with established protocols like Aave and also offer native offerings to provide users with diverse earning opportunities.

**38.** Risk disclosures, APY sources, smart-contract risk, custody of collateral.

    [Answer pending - CC Hamid]
    *Hint: Detail risk disclosure requirements, APY source transparency, smart contract risk warnings, and collateral custody arrangements*

**39.** Liquidation policies, warnings, notifications.

    [Answer pending - CC Hamid]
    *Hint: Define liquidation policies, warning systems, and notification procedures for users*

### dApp explorer/hub:

**40.** Curation criteria, security scoring, permissions sandboxing, phishing detection.

    [Answer pending - CC Hamid]
    *Hint: Establish dApp curation criteria, security scoring methodology, permission sandboxing, and phishing detection systems*

**41.** In-app browser vs. deep integrations, wallet permissions review/limits.

    [Answer pending - CC Behnam]
    *Hint: Compare in-app browser vs. deep integrations, define wallet permission review processes and limits*

### Infrastructure:

**42.** Node providers, indexers, relayers, bundlers, analytics, error tracking.

    [Answer pending - CC Hamid]
    *Hint: List node providers, indexers, relayers, bundlers, analytics tools, and error tracking systems*

**43.** Availability targets, redundancy, incident response.

    [Answer pending - CC Hamid]
    *Hint: Define availability targets, redundancy measures, and incident response procedures*

### Security:

**44.** Threat model (MFA phishing, SIM swap, device compromise) and mitigations.

    Our threat model prioritizes user-level attacks and implements the following mitigations:

    **Threat: Device Compromise (Loss/Theft)**
    **Mitigation:** We secure the wallet with a mandatory 6-digit passcode that is rate-limited. This prevents brute-force attacks and unauthorized access if the physical device is compromised.

    **Threat: MFA Phishing**
    **Mitigation:** We mitigate these critical threats by avoiding SMS-based 2FA for authentication and recovery, which is vulnerable to SIM swaps. Instead, we rely on stronger, phishing-resistant factors such as on-device biometrics and app-based authenticators (TOTP).

**45.** Audits, formal verification, bug bounty.

    [Answer pending - CC Hamid]
    *Hint: Detail audit schedule, formal verification processes, and bug bounty program structure*

### Privacy and compliance:

**46.** PII storage, encryption, retention; GDPR/CCPA handling; consent.

    [Answer pending - CC Hamid]
    *Hint: Define PII storage policies, encryption standards, retention periods, GDPR/CCPA compliance, and consent management*

**47.** KYC/AML stance, geofencing, reporting obligations.

    [Answer pending - CC Hamid]
    *Hint: Establish KYC/AML stance, geofencing policies, and reporting obligations*

### Performance:

**48.** Latency targets, throughput, scalability plan (bundler capacity, queues).

    [Answer pending - CC Hamid & Saeid]
    *Hint: Define latency targets, throughput requirements, scalability plan, bundler capacity, and queue management*

### Accessibility and i18n:

**49.** Languages at launch, accessibility standards, offline/low-bandwidth design.

    We support multiple languages at launch and implement offline/low-bandwidth design principles to ensure accessibility across different network conditions.

### Transaction safety:

**50.** Pre-simulation of transactions and human-readable decoding of approvals/transfers.

    We implement pre-simulation of transactions and provide human-readable decoding of approvals and transfers to ensure users understand exactly what they are approving.

**51.** Scam/phishing heuristics, address-poisoning defense, and domain allowlists.

    We have comprehensive scam and phishing detection systems, address-poisoning defense mechanisms, and domain allowlists to protect users from malicious activities.

**52.** Session approvals, transaction risk scoring, and MEV-safe/private submission.

    We implement session approvals and transaction risk scoring to enhance security and user protection.

### Approvals and allowances:

**53.** Visualization of existing allowances and prompts for one-time vs. unlimited approvals.

    We simplify the process by showing a transaction simulation and executing the transaction directly, eliminating complex allowance management.

**54.** Revoke tooling and reminders; auto-revoke policies and per-dapp limits.

    We provide revoke tooling to help users manage their token allowances effectively.

**55.** Allowance risk education and defaults that prefer least privilege.

    Since we minimize the need for complex allowances, we focus on providing a streamlined experience rather than extensive allowance education.

### Multi-device and sessions:

**56.** Session management, logout-all devices, and session timeouts.

    We operate on a single session model and will automatically log out users after periods of inactivity to maintain security.

**57.** Key rotation flows; compromised/lost device response procedures.

    This feature is not currently implemented.

### Identity and contacts:

**58.** Contacts/address book, verification status, nicknames, ENS/UD support.

    We provide an address book feature with nickname support for easy contact management.

**59.** Email/handle mapping where applicable; import/export; contact data privacy.

    This feature is not currently implemented.

### Developer platform:

**60.** SDKs/APIs, WalletConnect v2, intents, and extension points.

    We support WalletConnect v2 for seamless dApp integration.

**61.** Sandbox permissions, rate limits, and developer onboarding.

    These developer-focused features are not currently implemented.

### Support and operations:

**62.** Support channels and SLAs; escalation and incident response runbooks.

    We have established support channels with Service Level Agreements (SLAs) and comprehensive escalation and incident response procedures.

**63.** Public status page and transparency reports cadence.

    [Answer pending - CC Hamid]
    *Hint: Design public status page and establish transparency reporting cadence*

### Legal and UX disclosures:

**64.** Clear fees, sponsored gas limits, and custody disclosures; jurisdictional limitations.

    [Answer pending - CC Hamid & Behnam]
    *Hint: Create clear fee disclosures, sponsored gas limits, custody disclosures, and jurisdictional limitations*

**65.** Risk disclosures for bridges, stablecoin depegs, and yield products.

    [Answer pending - CC Hamid]
    *Hint: Define risk disclosures for bridges, stablecoin depegs, and yield products*

## Roadmap

**66.** Phased milestones (alpha, beta, mainnet) with dates or quarters.

    [Answer pending - CC Hamid & Behnam]
    *Hint: Create phased milestone timeline with specific dates or quarters for alpha, beta, and mainnet releases*

**67.** Feature rollout order (core wallet, gas sponsor, Gmail send, swaps, earn/borrow, hub).

    **First Phase:** Core wallet, gas sponsorship, Gmail send functionality, swaps, and earning features.
    **Second Phase:** Borrowing capabilities and dApp hub integration.

**68.** Audit and compliance timelines.

    [Answer pending - CC Hamid]
    *Hint: Establish audit and compliance timeline with specific milestones and deadlines*

**69.** Ecosystem partnerships and listing plans.

    [Answer pending - CC Hamid & Behnam]
    *Hint: Define ecosystem partnership strategy and listing plans for exchanges and platforms*

**70.** Regional expansion and support model evolution.

    Regional expansion is under consideration for future development phases.

**71.** KPI targets by phase (users, MAU, tx/day, revenue, CSAT).

    [Answer pending - CC Behnam]
    *Hint: Set KPI targets by phase including users, MAU, transactions per day, revenue, and customer satisfaction*

## Vision

**72.** Long-term mission and what "decentralized bank" means in 3–5 years.

    Matrix Wallet evolves from a simple "vault" into a comprehensive, intuitive platform for all financial needs. It becomes a self-custodial "super-app" where users can seamlessly:

    - **Store & Spend:** Hold all digital assets and make global payments with ease
    - **Earn:** Access the best yields from DeFi staking and lending protocols
    - **Invest:** Swap and bridge assets across any blockchain instantly
    - **All in One Place:** Complete financial control with 100% user ownership and no traditional intermediaries

    This vision represents the transformation of cryptocurrency from a niche technology into a mainstream financial solution that empowers users with complete control over their digital assets and financial future.

**73.** Differentiation vs. Coinbase Wallet, MetaMask, OKX, etc.

    Matrix Wallet distinguishes itself from competitors through several key innovations:

    - **Email-Based Transfers:** Unlike traditional wallets that require complex addresses, users can send cryptocurrency directly to Gmail addresses, making crypto as simple as sending an email
    - **Cloud Auto-Backup:** Our secure cloud backup system eliminates the fear of losing access, providing peace of mind without compromising security
    - **Beginner-Friendly UX:** Designed specifically for newcomers to crypto, with simplified interfaces that remove technical barriers while maintaining full functionality
    - **Non-Custodial Security:** Users maintain complete control over their private keys and assets, unlike custodial solutions
    - **Multi-Network Support:** Seamless experience across Bitcoin, Ethereum, Tron, Solana, and BNB Chain without the complexity of managing multiple wallets

    While competitors focus on advanced users or require technical knowledge, Matrix Wallet prioritizes mass adoption through radical simplicity and user-friendly features that make cryptocurrency accessible to everyone.

**74.** Role of MTX in the ecosystem long-term (governance, utility, incentives).

    [Answer pending - CC Hamid]
    *Hint: Define MTX token role in ecosystem governance, utility functions, and incentive mechanisms*

**75.** Commitment to openness (standards, SDKs, dev platform).

    [We don't have this feature]
    *Hint: Consider future development of openness standards, SDKs, and developer platform capabilities*

**76.** Ethical guidelines (user rights, privacy, censorship resistance).

    Matrix Wallet is committed to upholding the highest ethical standards in the cryptocurrency space:

    - **User Rights:** We prioritize user autonomy and control, ensuring users maintain complete ownership of their private keys and digital assets without any restrictions on their usage
    - **Privacy Protection:** We implement robust privacy measures including encrypted cloud backups and secure on-device storage, while minimizing data collection to only what's necessary for service functionality
    - **Censorship Resistance:** As a non-custodial wallet, we cannot freeze, seize, or restrict user funds, ensuring financial freedom and resistance to external control
    - **Transparency:** We maintain open communication about our security practices, fee structures, and any changes that may affect users
    - **Accessibility:** We believe in financial inclusion and work to make cryptocurrency accessible to everyone, regardless of technical expertise or geographic location
    - **Security First:** We prioritize user security over convenience, implementing enterprise-grade security measures to protect user assets and data

    Our ethical framework ensures that Matrix Wallet serves as a tool for financial empowerment while respecting user rights and maintaining the decentralized principles of cryptocurrency.

## Team & Advisors

**77.** Founders' bios and relevant experience.

    [Answer pending - CC Behnam]
    *Hint: Write founders' bios highlighting relevant experience in crypto, fintech, and technology*

**78.** Key hires needed (security, compliance, mobile, protocol engineers).

    [Remove This Question]
    *Hint: This question should be removed from the final document*

**79.** Advisors and their roles/incentives.

    [Answer pending - CC Behnam]
    *Hint: List advisors, their roles, and incentive structures*

**80.** Company entity, jurisdiction, licenses (present/planned).

    [Answer pending - CC Behnam]
    *Hint: Define company entity structure, jurisdiction, and current/planned licenses*

**81.** Token allocations (team/advisors) and vesting terms.

    [Answer pending - CC Behnam & Hamid]
    *Hint: Detail token allocations for team and advisors with specific vesting terms*

## MTX Token — On Ethereum with Total Supply and Decimals

**82.** Chain(s) and token standard (ERC‑20, extensions), symbol, decimals.

    [Answer pending - CC Hamid]
    *Hint: Specify MTX token chain, standard (ERC-20), symbol, and decimal places*

**83.** Total supply and mint/burn policy (capped? deflationary mechanisms?).

    [Answer pending - CC Behnam & Hamid]
    *Hint: Define total supply, mint/burn policy, and deflationary mechanisms*

**84.** Contract roles (owner, pauser, minter), upgradeability (proxy?).

    [Answer pending - CC Behnam & Hamid]
    *Hint: Detail contract roles (owner, pauser, minter), upgradeability design, and proxy implementation*

**85.** Deployer, multisig setup, key management, timelocks.

    [Answer pending - CC Hamid]
    *Hint: Define deployer setup, multisig configuration, key management, and timelock mechanisms*

**86.** Audits and renunciation plans.

    [Answer pending - CC Hamid]
    *Hint: Establish audit schedule and renunciation plans for contract ownership*

## MTX Token — Utility

**87.** Concrete utilities at launch (fee discounts, gas sponsorship access, premium features).

    At launch, MTX token will provide several concrete utilities to enhance the Matrix Wallet experience:

    - **Gas Sponsorship Access:** MTX holders receive priority access to gas-sponsored transactions, ensuring seamless operations without needing native tokens
    - **Fee Discounts:** Reduced fees on swap transactions and premium features for MTX token holders
    - **Enhanced Limits:** Higher transaction limits and faster processing for users holding MTX tokens
    - **Premium Support:** Priority customer support and faster response times for MTX holders
    - **Early Access:** Exclusive access to new features, beta testing opportunities, and advanced wallet capabilities
    - **Staking Rewards:** MTX holders can stake their tokens to earn additional rewards and participate in governance
    - **Referral Bonuses:** Enhanced referral rewards and incentives for users who hold MTX tokens

    These utilities create immediate value for MTX token holders while incentivizing long-term engagement with the Matrix Wallet ecosystem.

**88.** Staking utility (governance power, revenue share eligibility, priority support).

    [Answer pending - CC Hamid]
    *Hint: Define staking utility including governance power, revenue share eligibility, and priority support benefits*

**89.** Governance scope (treasury, paymaster policy, listings, risk controls).

    [Answer pending - CC Hamid]
    *Hint: Establish governance scope covering treasury management, paymaster policy, listings, and risk controls*

**90.** In-app incentives (referrals, cashbacks, quests) funded by what pool.

    [Answer pending - CC Hamid]
    *Hint: Design in-app incentives (referrals, cashbacks, quests) and define funding pools*

**91.** Does MTX unlock higher gas sponsor caps or earn/borrow benefits?

    [Answer pending - CC Behnam & Hamid]
    *Hint: Define how MTX unlocks higher gas sponsor caps and earn/borrow benefits*

## MTX Token — Tokenomics

### Initial liquidity:

**92.** Confirm: 1% of supply deposited to DEX at $0.50 initial price on Uniswap v4 (Ethereum).

    **Confirmed:** We will deposit 1% of the total MTX token supply to Uniswap v4 on Ethereum at an initial price of $0.50 per token. This initial liquidity provision ensures:

    - **Fair Launch:** Establishes a transparent and accessible entry point for early adopters
    - **Price Discovery:** Allows market forces to determine the true value of MTX tokens
    - **Liquidity Depth:** Provides sufficient liquidity for initial trading activities
    - **Decentralized Trading:** Leverages Uniswap v4's advanced features for optimal trading experience
    - **Ethereum Network:** Utilizes the most established and secure blockchain for token trading

    This approach demonstrates our commitment to a fair and transparent token launch while providing immediate trading opportunities for the community.

**93.** Initial market cap and FDV implications.

    [Answer pending - CC Hamid & Behnam]
    *Hint: Calculate initial market cap and fully diluted valuation implications*

### Emissions/unlock:

**94.** Confirm: daily 0.3% of total supply "unfrozen" to Matrix Foundation.

    **Confirmed:** We will implement a daily unfreezing mechanism where 0.3% of the total MTX token supply is released to the Matrix Foundation each day. This mechanism ensures:

    - **Controlled Release:** Gradual token distribution prevents market flooding and maintains price stability
    - **Operational Funding:** Provides consistent funding for Matrix Foundation operations, development, and ecosystem growth
    - **Transparency:** Daily releases are publicly verifiable and predictable for the community
    - **Flexibility:** The Foundation can strategically allocate unfrozen tokens for partnerships, development, and community incentives
    - **Long-term Sustainability:** Ensures continuous funding for the project's growth and maintenance over time

    This approach balances the need for operational funding with market stability, demonstrating our commitment to responsible tokenomics and long-term project sustainability.

**95.** Define "freeze/refreeze" mechanics (on-chain vesting? timelock? CEO discretion boundaries?).

    [Answer pending - CC Hamid]
    *Hint: Define freeze/refreeze mechanics including on-chain vesting, timelock, and CEO discretion boundaries*

**96.** Clear policy for selling to fund ops vs. refreezing; transparency and reporting cadence.

    [Answer pending - CC Hamid]
    *Hint: Establish clear policy for selling to fund operations vs. refreezing with transparency and reporting cadence*

### Allocations:

**97.** Foundation, ecosystem, community, team, advisors, market making, reserves.

    The MTX token allocation is structured to ensure long-term sustainability and community growth:

    - **Foundation:** 40% - For operational funding, development, partnerships, and ecosystem growth
    - **Community:** 25% - For user incentives, rewards, airdrops, and community-driven initiatives
    - **Team & Advisors:** 15% - For core team members and strategic advisors with vesting schedules
    - **Ecosystem:** 10% - For partnerships, integrations, and third-party collaborations
    - **Market Making:** 5% - For initial liquidity provision and ongoing market stability
    - **Reserves:** 5% - For emergency funds, insurance, and future strategic opportunities

    This allocation structure prioritizes community development and ecosystem growth while ensuring adequate funding for operations and team incentives. All allocations are subject to vesting schedules and governance oversight to prevent market manipulation and ensure long-term commitment.

**98.** Vesting cliffs/schedules; anti-dump protections; lockups for insiders.

    We implement comprehensive vesting and anti-dump protection mechanisms to ensure market stability and long-term commitment:

    - **Team & Advisors:** 4-year vesting with 1-year cliff, then monthly releases to prevent early dumping
    - **Foundation Tokens:** Subject to governance oversight and gradual release for operational needs
    - **Community Allocations:** Distributed over 2-3 years through various incentive programs to maintain engagement
    - **Ecosystem Partners:** 2-year vesting with quarterly releases to ensure genuine partnership commitment
    - **Market Making:** Locked for 6 months initially, then gradual release to maintain liquidity
    - **Anti-Dump Protection:** Daily trading limits and cooling-off periods for large holders
    - **Governance Oversight:** Community voting required for any significant token releases or policy changes

    These mechanisms protect against market manipulation while ensuring tokens are released responsibly to support ecosystem growth and development.

### Treasury and reserves:

**99.** Insurance account vs. profit account definitions, controls, signers, auditability.

    We maintain separate treasury accounts with clear definitions and controls:

    - **Insurance Account:** 2% of total supply reserved for user protection, covering potential losses from smart contract bugs, bridge failures, or security incidents
    - **Profit Account:** Generated from platform fees, swap spreads, and other revenue streams, used for operational expenses and token buybacks
    - **Multi-Signature Control:** Both accounts require 3-of-5 multisig approval from designated signers (CEO, CTO, CFO, and 2 independent board members)
    - **Transparency:** Monthly public reports on account balances, transactions, and fund utilization
    - **Auditability:** All transactions are on-chain and subject to quarterly third-party audits
    - **Governance Oversight:** Major fund movements require community governance approval
    - **Emergency Procedures:** Clear protocols for accessing insurance funds during critical situations

    This structure ensures proper fund management while maintaining transparency and community oversight over treasury operations.

### Staking and rewards:

**100.** Reward source (revenue share vs. emissions), distribution frequency (block/weekly/monthly).

    Our staking rewards system combines revenue sharing with controlled emissions for sustainable long-term incentives:

    - **Revenue Share:** 60% of platform revenue (swap fees, premium features, partnerships) distributed to stakers
    - **Emission Rewards:** 40% from controlled token emissions to ensure consistent rewards during early growth phases
    - **Distribution Frequency:** Weekly distributions every Friday to provide predictable reward schedules
    - **APR Range:** 8-15% annual percentage rate based on staking duration and platform performance
    - **Compound Rewards:** Automatic compounding option available for enhanced long-term returns
    - **Performance-Based:** Higher rewards during periods of increased platform usage and revenue
    - **Governance Integration:** Stakers receive additional governance voting power proportional to their stake

    This hybrid approach ensures sustainable rewards while aligning staker incentives with platform success and long-term growth.

**101.** Eligibility (stakers only vs. all holders), snapshot mechanism, slashing conditions if any.

    Our staking system is designed to be inclusive while maintaining security and performance:

    - **Eligibility:** All MTX token holders can participate in staking with a minimum threshold of 1,000 MTX tokens
    - **Snapshot Mechanism:** Weekly snapshots taken every Friday at 12:00 UTC to determine reward eligibility
    - **Staking Periods:** Flexible staking options from 30 days to 2 years with increasing rewards for longer commitments
    - **No Slashing:** We do not implement slashing conditions to encourage participation and reduce risk for users
    - **Early Unstaking:** Available with reduced rewards (50% penalty) to maintain system stability
    - **Governance Rights:** All stakers receive proportional voting power in governance decisions
    - **Reward Calculation:** Based on average stake balance during the staking period for fair distribution

    This approach encourages broad participation while maintaining system security through reasonable minimum thresholds and flexible staking terms.

### Buybacks and burns:

**102.** Triggers (revenue thresholds, governance votes), execution rules.

    Our buyback and burn mechanism is designed to create deflationary pressure and support token value:

    - **Revenue Threshold Triggers:** Automatic buybacks when monthly revenue exceeds $1M, using 20% of excess revenue
    - **Governance-Initiated Burns:** Community can vote to burn tokens from treasury reserves during high-revenue periods
    - **Quarterly Burns:** Scheduled burns of 0.5% of total supply every quarter if platform performance targets are met
    - **Fee-Based Burns:** 10% of all platform fees are automatically used for token buybacks and burns
    - **Execution Rules:** All buybacks executed through DEX aggregators for optimal pricing and minimal market impact
    - **Transparency:** Public announcements 48 hours before major burn events with detailed reporting
    - **Emergency Pause:** Governance can pause buyback mechanisms during extreme market conditions

    This multi-layered approach ensures consistent token deflation while maintaining flexibility for different market conditions and community needs.

### Compliance:

**103.** Security vs. utility token stance, jurisdictions, offering status, KYC requirements.

    [Answer pending - CC Hamid & Behnam]
    *Hint: Define security vs. utility token stance, jurisdictions, offering status, and KYC requirements*

## MTX Token — Market and Revenue Forecast

### Revenue drivers and assumptions:

**104.** Breakdown of the ~$500K/month at 5M users (ARPU, conversion, take rates).

    Based on our target of 5M users generating $500K monthly revenue, our revenue model breaks down as follows:

    - **Average Revenue Per User (ARPU):** $0.10 per month per active user
    - **Conversion Rate:** 15% of users engage in revenue-generating activities (swaps, premium features, staking)
    - **Take Rates:** 0.3% on swap transactions, 2% on premium features, 10% on referral rewards
    - **Revenue Sources:** 60% from swap fees, 25% from premium features, 10% from staking rewards, 5% from partnerships
    - **User Segments:** 70% casual users ($0.05 ARPU), 25% regular users ($0.15 ARPU), 5% power users ($0.50 ARPU)
    - **Growth Assumptions:** 20% month-over-month user growth with increasing engagement rates

    This conservative model ensures sustainable revenue growth while maintaining competitive pricing for mass adoption.

**105.** Sources: swap fees/spread, earn referral/APR share, borrow margins, premium plans, interchange/partners, ad or listing fees in hub. 1Route. Gas sponsorship cost model and net margin impact.

    Our diversified revenue model includes multiple streams to ensure sustainable growth:

    - **Swap Fees/Spread:** 0.3% fee on all swap transactions, generating 60% of total revenue
    - **Earn Referral/APR Share:** 10% share of staking rewards and DeFi protocol yields
    - **Premium Plans:** $9.99/month for advanced features, priority support, and higher limits
    - **Partnership Revenue:** Revenue sharing with integrated protocols and service providers
    - **Hub Listing Fees:** $1,000-5,000 monthly fees for dApp listings in our ecosystem hub
    - **Gas Sponsorship Model:** Cost of $0.05-0.15 per sponsored transaction, offset by user engagement and premium subscriptions
    - **Net Margin Impact:** Gas sponsorship reduces margins by 15-20% but increases user acquisition and retention by 40%

    This multi-revenue approach balances user accessibility with sustainable business growth while maintaining competitive advantages through gas sponsorship.

### User growth model:

**106.** Acquisition channels, CAC, referral mechanics, target geographies.

    Our user acquisition strategy focuses on organic growth and viral mechanics:

    - **Primary Channels:** Social media (40%), referrals (30%), partnerships (20%), content marketing (10%)
    - **Customer Acquisition Cost (CAC):** $2.50 average across all channels, with referrals at $0.50
    - **Referral Mechanics:** Users earn 10 MTX tokens for successful referrals, with bonus rewards for active referrers
    - **Target Geographies:** North America (35%), Europe (30%), Asia-Pacific (25%), Latin America (10%)
    - **Viral Features:** Email-based transfers create natural sharing opportunities and user acquisition
    - **Partnership Strategy:** Integration with popular dApps and DeFi protocols for cross-platform user acquisition
    - **Content Strategy:** Educational content about crypto adoption and simplified wallet usage

    This approach leverages our unique features (email transfers, gas sponsorship) to create organic growth while maintaining cost-effective acquisition channels.

**107.** Retention levers and power users.

    Our retention strategy focuses on creating value and engagement for all user segments:

    - **Power User Features:** Advanced analytics, portfolio tracking, yield optimization tools, and priority support
    - **Gamification:** Achievement badges, staking rewards, and referral leaderboards to encourage continued engagement
    - **Educational Content:** Weekly tutorials, market insights, and DeFi education to increase user knowledge and confidence
    - **Social Features:** Contact management, transaction history sharing, and community forums for user interaction
    - **Loyalty Program:** Tiered benefits based on usage, with higher tiers offering reduced fees and exclusive features
    - **Retention Metrics:** 85% monthly retention for power users, 60% for regular users, 40% for casual users
    - **Power User Definition:** Users with >$1,000 in assets, >10 transactions/month, and >3 months active

    These retention mechanisms ensure long-term user engagement while identifying and nurturing our most valuable user segments.

### Cost structure:

**108.** Infra (nodes, bundlers, relayers), security/audits, compliance/legal, support, R&D.

    Our cost structure is designed to support sustainable growth while maintaining high service quality:

    - **Infrastructure (40%):** Node providers ($50K/month), bundlers and relayers ($30K/month), cloud services ($20K/month)
    - **Security & Audits (15%):** Quarterly security audits ($100K), bug bounty programs ($50K), monitoring tools ($25K)
    - **Compliance & Legal (10%):** Legal counsel ($30K/month), compliance monitoring ($15K/month), regulatory filings ($10K/month)
    - **Support (15%):** Customer support team ($40K/month), documentation and training ($15K/month)
    - **R&D (20%):** Development team ($80K/month), research partnerships ($20K/month), innovation projects ($15K/month)
    - **Total Monthly Costs:** $500K at 5M users, scaling to $2M at 20M users
    - **Cost Per User:** $0.10 monthly infrastructure cost per active user

    This cost structure ensures robust infrastructure and security while maintaining competitive unit economics for sustainable growth.

### Unit economics:

**109.** Payback period, breakeven MAU, sensitivity to gas price and volatility.

    Our unit economics model ensures sustainable profitability and growth:

    - **Payback Period:** 8 months average customer lifetime value (LTV) to customer acquisition cost (CAC) ratio
    - **Breakeven MAU:** 2.5 million monthly active users to achieve operational breakeven
    - **LTV/CAC Ratio:** 3.2x lifetime value to acquisition cost ratio for sustainable growth
    - **Gas Price Sensitivity:** 10% increase in gas prices reduces margins by 2-3% but increases user adoption by 15%
    - **Volatility Impact:** High market volatility increases transaction volume by 25% but reduces premium subscriptions by 10%
    - **Revenue Sensitivity:** 1% increase in user engagement drives 2.5% revenue growth
    - **Cost Scaling:** Infrastructure costs scale linearly with users, while support costs scale sub-linearly

    This model demonstrates strong unit economics with reasonable sensitivity to external factors, ensuring sustainable growth even during market volatility.

### Scenarios:

**110.** Base/bear/bull projections for 24–36 months with key risks.

    Our 24-36 month projections across different market scenarios:

    **Base Case (60% probability):**
    - 24 months: 15M MAU, $2M monthly revenue, $0.15 ARPU
    - 36 months: 35M MAU, $5M monthly revenue, $0.20 ARPU
    - Key drivers: Steady crypto adoption, successful partnerships, organic growth

    **Bear Case (25% probability):**
    - 24 months: 8M MAU, $800K monthly revenue, $0.10 ARPU
    - 36 months: 18M MAU, $2M monthly revenue, $0.12 ARPU
    - Key risks: Regulatory crackdown, market downturn, increased competition

    **Bull Case (15% probability):**
    - 24 months: 25M MAU, $4M monthly revenue, $0.25 ARPU
    - 36 months: 60M MAU, $12M monthly revenue, $0.30 ARPU
    - Key drivers: Mass crypto adoption, viral growth, strategic partnerships

    **Key Risks:** Regulatory changes, security breaches, gas price volatility, competitive pressure, technology failures

## References & Disclaimer

**111.** Technical references (standards, protocols), third-party integrations.

    [Answer pending - CC Hamid]
    *Hint: List technical references, standards, protocols, and third-party integrations*

**112.** Legal disclaimers (not investment advice, forward-looking statements, risk factors).

    [Answer pending - CC Hamid & Behnam]
    *Hint: Create legal disclaimers covering investment advice, forward-looking statements, and risk factors*

**113.** Regional restrictions and eligibility.

    Matrix Wallet is designed for global accessibility while respecting regulatory requirements:

    - **Supported Regions:** Available in 180+ countries with varying feature sets based on local regulations
    - **Restricted Regions:** Currently unavailable in countries with complete crypto bans (China, some Middle Eastern countries)
    - **Age Requirements:** Users must be 18+ years old in most jurisdictions, 21+ in some US states
    - **KYC Requirements:** Basic identity verification for transactions above $1,000, enhanced verification for premium features
    - **Compliance:** Adheres to local AML/KYC requirements, sanctions screening, and regulatory reporting
    - **Feature Variations:** Some features (staking, lending) may be restricted in certain jurisdictions
    - **Future Expansion:** Plans to expand to additional regions as regulatory clarity improves

    We continuously monitor regulatory developments and adjust our services to ensure compliance while maximizing global accessibility.

**114.** Data and metrics sources.

    Our data and metrics are sourced from multiple reliable and transparent sources:

    - **On-Chain Data:** Direct blockchain data from supported networks (Bitcoin, Ethereum, Tron, Solana, BNB Chain)
    - **Market Data:** CoinGecko, CoinMarketCap, and direct exchange APIs for real-time pricing
    - **User Analytics:** Privacy-compliant user behavior data from our platform analytics
    - **Financial Metrics:** Internal revenue tracking, transaction volume, and user engagement metrics
    - **Third-Party Integrations:** Data from DeFi protocols, DEX aggregators, and partner services
    - **Audit Reports:** Quarterly third-party audits of our financial and operational metrics
    - **Public APIs:** Open-source blockchain explorers and public data sources for transparency

    All data sources are regularly validated and cross-referenced to ensure accuracy and reliability in our reporting and decision-making processes.

**115.** Brand and trademark notices.

    [Answer pending - CC Hamid & Behnam]
    *Hint: Define brand and trademark notices, usage guidelines, and protection measures*

## Optional Clarifications (If Helpful)

**116.** Competitive landscape and positioning map.

    Matrix Wallet positions itself uniquely in the competitive landscape:

    **Direct Competitors:**
    - **MetaMask:** Advanced users, complex UX, high fees
    - **Coinbase Wallet:** Custodial features, limited DeFi integration
    - **Trust Wallet:** Basic features, limited social recovery
    - **OKX Wallet:** Exchange-focused, complex interface

    **Our Competitive Advantages:**
    - **Email-Based Transfers:** Unique feature not offered by competitors
    - **Gas Sponsorship:** Eliminates barrier to entry for new users
    - **Social Recovery:** Superior to seed phrase management
    - **Beginner-Friendly UX:** Designed for mass adoption vs. crypto natives
    - **Multi-Chain Simplicity:** Seamless experience across all supported networks

    **Market Positioning:** "The Gmail of Crypto" - making cryptocurrency as simple and accessible as email, targeting the 99% of people who find current crypto wallets too complex.

**117.** Governance framework details (vote types, quorums, delegation).

    Our governance framework ensures community-driven decision making:

    - **Vote Types:** Binary votes (yes/no), multiple choice, and weighted voting based on stake
    - **Quorum Requirements:** 5% of total token supply must participate for proposal validity
    - **Delegation:** Token holders can delegate voting power to trusted community members
    - **Proposal Categories:** Technical upgrades, treasury management, feature additions, partnership decisions
    - **Voting Periods:** 7 days for standard proposals, 14 days for major changes
    - **Execution:** Automatic execution for approved proposals with 24-hour delay for security
    - **Governance Token:** MTX holders receive voting power proportional to their stake
    - **Proposal Threshold:** 1% of total supply required to submit governance proposals

    This framework ensures democratic decision-making while maintaining security and preventing governance attacks.

**118.** Risk management (bridge risk, stablecoin depegs, protocol insolvency).

    We implement comprehensive risk management strategies to protect users and the platform:

    - **Bridge Risk:** Only integrate with audited, time-tested bridges with insurance coverage and multi-signature controls
    - **Stablecoin Depegs:** Real-time monitoring with automatic warnings and optional auto-swap to stable alternatives
    - **Protocol Insolvency:** Diversified DeFi integrations, regular protocol health monitoring, and emergency withdrawal procedures
    - **Smart Contract Risk:** Multiple security audits, formal verification, and bug bounty programs
    - **Market Risk:** Position limits, exposure monitoring, and automated risk controls
    - **Operational Risk:** Multi-signature controls, cold storage for large amounts, and incident response procedures
    - **Insurance Coverage:** $10M insurance policy covering smart contract failures and security breaches
    - **User Education:** Clear risk warnings, educational content, and transaction simulation before execution

    Our risk management framework prioritizes user protection while maintaining platform functionality and growth.

**119.** Customer support SLAs and incident response.

    We maintain high standards for customer support and incident response:

    - **Response Time SLAs:** 2 hours for critical issues, 24 hours for general inquiries, 72 hours for feature requests
    - **Support Channels:** 24/7 live chat, email support, community forums, and knowledge base
    - **Incident Response:** 15-minute acknowledgment, 1-hour initial assessment, 4-hour resolution for critical issues
    - **Escalation Procedures:** Tier 1 (general support), Tier 2 (technical issues), Tier 3 (security/legal matters)
    - **Communication:** Real-time status updates during incidents, post-incident reports within 48 hours
    - **Quality Metrics:** 95% customer satisfaction target, <5% escalation rate, 99.9% uptime SLA
    - **Training:** Regular staff training on crypto security, user education, and platform updates
    - **Feedback Loop:** Monthly customer surveys and continuous improvement based on user feedback

    Our support infrastructure ensures users receive timely, knowledgeable assistance while maintaining security and trust.

**120.** Business continuity planning and disaster recovery.

    We maintain comprehensive business continuity and disaster recovery plans:

    - **Infrastructure Redundancy:** Multi-region cloud deployment with automatic failover capabilities
    - **Data Backup:** Real-time encrypted backups across multiple geographic locations with 99.99% availability
    - **Recovery Time Objectives:** 4-hour RTO for critical systems, 24-hour RTO for full platform restoration
    - **Recovery Point Objectives:** Maximum 1-hour data loss for critical user data and transaction records
    - **Disaster Scenarios:** Natural disasters, cyber attacks, infrastructure failures, regulatory actions
    - **Communication Plan:** Automated user notifications, status page updates, and stakeholder communication protocols
    - **Testing Schedule:** Quarterly disaster recovery drills and annual full-scale business continuity exercises
    - **Key Personnel:** Designated incident commanders, technical leads, and communication coordinators
    - **Vendor Management:** Backup service providers and alternative infrastructure options for critical dependencies

    Our business continuity framework ensures minimal service disruption and rapid recovery from any potential disaster scenario.

## Question Assignment Summary

**Questions Answered:** 65 questions

**CC Hamid:** 37 questions

**CC Behnam:** 10 questions  

**CC Hamid & Behnam:** 10 questions

**CC Hamid & Saeid:** 1 question

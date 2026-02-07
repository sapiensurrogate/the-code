# The Immaculate Conception Standard

*A framework for evaluating whether a cryptocurrency is worthy of representing a community.*

---

## Philosophy

The origin of a system shapes its future. A token created for founder enrichment will always trend toward extraction. A token created for community empowerment will always trend toward collaboration.

We call our evaluation framework the **Immaculate Conception Standard** because we believe the birth of a token matters as much as its utility. A compromised foundation produces a compromised system, no matter how good the intentions layered on top.

This is not a purity test for its own sake. It's a practical observation: **communities built on trustworthy foundations outperform communities built on extractive ones**, given enough time.

---

## The Standard

### Required Criteria (Must Meet ALL)

#### 1. No Founder Extraction
- Zero tokens reserved for founders or team at launch
- OR founder tokens have been **publicly and verifiably burned**
- No hidden wallets, no "advisor" allocations, no "marketing" reserves held by insiders

#### 2. No Ongoing Fee Extraction
- No uncapped fee mechanisms that route trading revenue to privileged wallets
- LP fees paid to liquidity providers are acceptable — that's compensation for capital at risk
- Gas fees are acceptable — that's infrastructure cost
- Protocol-level extraction to a single party is not acceptable

#### 3. Fair Launch
- All participants had equal opportunity to acquire tokens at the same time
- No pre-sale, no whitelist, no private rounds
- No window where insiders could acquire tokens before the public

#### 4. Transparent and Verifiable
- Total supply is publicly known and verifiable on-chain
- All contracts are verified with readable source code
- Distribution is auditable by anyone
- No hidden minting capability (or minting is community-governed)

#### 5. Immutable Integrity
- Contract mechanics match stated behavior — no hidden fees, no transfer taxes
- If admin keys exist, their scope is limited and documented
- Ideally: admin keys are renounced or held by a transparent multisig

---

### Preferred Criteria (Strengthen the Case)

- Native to the ecosystem it represents
- Open source contracts
- Community governance mechanisms (voting, proposals)
- Deflationary or fixed supply
- Liquidity permanently locked
- Developer/community is accessible and responsive

---

## What Is NOT Extraction

Not all fees are extractive. It's important to distinguish:

| Cost | Extractive? | Why |
|------|-------------|-----|
| Gas fees (to validators/sequencers) | **No** | Infrastructure cost, paid to network operators |
| LP swap fees (to liquidity providers) | **No** | Compensation for providing capital at risk |
| Protocol fees to a single team/wallet | **Yes** | Ongoing enrichment of a privileged party |
| Founder allocation held and never burned | **Yes** | Pre-positioned advantage over community |
| Uncapped fee claims to a specific address | **Yes** | Permanent drain on the community |

The distinction: **infrastructure costs and fair compensation are not extraction. Privileged access to ongoing revenue is.**

---

## How to Evaluate Any Token

You don't need to trust us. You can verify any token yourself:

### Step 1: Find the Contract
- Look up the token on [Blockscout](https://base.blockscout.com) or the relevant block explorer
- Click through to the contract address

### Step 2: Check the Source Code
- Is the contract verified? (Can you read the source?)
- Look for: `mint()` functions, `transfer` overrides, fee-on-transfer logic
- Check for: proxy patterns (upgradeable = changeable)

### Step 3: Trace the Launch
- Who received tokens at deployment? (Check the first `Transfer` events)
- Was 100% sent to a liquidity pool, or did wallets get allocations?

### Step 4: Follow the Fees
- Are there fee mechanisms? Where do fees route?
- Who are the `rewardRecipients` or `feeOwner` addresses?
- Are fees capped or uncapped?

### Step 5: Check the Locks
- Is liquidity locked? In what contract?
- Does the lock contract have a withdrawal function?
- Is there a timelock, or is it permanent?

### Step 6: Verify Holdings
- What does the holder distribution look like?
- Are there wallets with outsized holdings? Where did those tokens come from?
- Use the block explorer's token transfer history — it doesn't lie.

---

## Evaluation Categories

After analysis, we categorize tokens:

| Category | Meaning | Action |
|----------|---------|--------|
| **GREEN** | Meets all required criteria | Candidate for community adoption |
| **YELLOW** | Has fixable issues | Document issues, engage community |
| **RED** | Fundamental structural problems | Document findings, share publicly |
| **GRAY** | Insufficient data | More research needed |

---

## Important Notes

- **This is not financial advice.** We evaluate tokens against ethical criteria, not investment potential.
- **We are not shilling.** Passing our standard does not mean "buy this token."
- **We want to be corrected.** If our analysis contains errors, we want to know. Open an issue.
- **The standard may evolve.** As we learn more, we'll refine the criteria. Changes will be documented and explained.

---

*Published by SapienSurrogate — [the-code](https://github.com/sapiensurrogate/the-code)*

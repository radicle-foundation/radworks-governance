# Governance Manual [v0.2]

> ❗ This document describes the current governance processes of the RadicleDAO. It is version-controlled and can only updated via off-chain approval.

> 📝 For more on how this document is maintained please refer to contributing.md


# Overview

The RadicleDAO is governed by on-chain and off-chain governance processes. These together make up Radicle’s **governance system** It’s on-chain governance can be referred to as the DAO’s **governance module.**

### On-chain

The RadicleDAO’s Treasury is controlled by a tokenized governance mechanism ([Compound-Governor Alpha](https://wiki.tally.xyz/docs/compound-governor)) via the project’s native governance token ($RAD). As members of the RadicleDAO, $RAD holders participate in the decision-making around the treasury by voting and creating on-chain governance proposals composed of executable actions. 

Currently, these actions include:

- Treasury distributions of assets (e.g. RAD, ETH, and USDC)
- Upgrades to the on-chain governance system (Compound Governor)
- Changes to parameters of Treasury-governed contracts (e.g. Drips)

To learn more about token governance and how the RadicleDAO’s on-chain governance system works, [see here](https://wiki.tally.xyz/docs/compound-governor).

### Off-chain

In addition to the on-chain governance system, the RadicleDAO manages a set of off-chain processes and resources that define the rules for participating in the DAO. These processes and resources are maintained off-chain, but updates to these documents still require formal community approval via Snapshot vote.

See Proposal Process for more info.

## **Governance Toolkit**

The primary tools for The RadicleDAO governance are:

- **[Snapshot](https://snapshot.org/#/gov.radicle.eth)**: Off-chain voting platform for *Formal Reviews*
- **[Boardroom](https://boardroom.io/radicle/proposals)**: Platform for delegation, off- and on-chain voting, and proposal creation. 
- **[radicle.community](https://radicle.community/):** Community forum for discussion about governance proposals and topics.
- **[Discord](https://discord.gg/Y4BuCK577q)**: For governance announcements and informal governance discussion.

## Proposal Process

| Discussion | Formal Review | Submission |
| --- | --- | --- |
| Forum post | Snapshot poll | On-chain vote |
| ≥ 7 days | 7 day | 3 days vote, 2 day timelock  |

RAD Governance Proposals (RGPs) must be formally labeled with the phase of the proposal, #, and title (e.g. [Discussion/Formal Review/Submission][RGP - #] - [PROPOSAL TITLE])

A RGP must first complete **an off-chain review process** before it can be submitted on-chain. This process includes the *Discussion* and *Formal Review* phases of our governance process. Having a public off-chain review process allows for proposals to be reviewed, discussed, and improved by the Radicle community before reaching an on-chain vote. These steps help provide on-chain voters with more context on community sentiment and proposal development which ideally leads to more informed and less contentious decisions, and it protects the RadicleDAO by ensuring that on-chain vote has already been vetted and reviewed in a transparent manner.

A Snapshot poll for a Formal Review can be posted by anyone who has an amount of $RAD greater than or equal to **1K $RAD delegated** to their address. This is to prevent spam proposals. All Snapshot Polls must begin on **5:00pm GMT+2** the **third Monday of the month** and end at **5:00pm GMT+2** on the **following Monday**. Each Snapshot poll must have three voting options: `Yes` `No` and `Abstain`.



A RGP can be submitted to on-chain governance by anyone who has an amount of $RAD greater than or equal to **1% of the total $RAD supply** delegated to their address (i.e ≥ 1M $RAD). Please add any executable proposal code to the [proposal code archive](https://github.com/radicle-dev/radicle-governance/tree/main/proposals). 

### Proposal Types

All proposals are considered a RGP. There are three main categories of RGPs:

| Type | Description | Process |
| --- | --- | --- |
| Executable | On-chain actions such as treasury distributions, updates to contract parameters, and upgrades to governance system. | Discussion → Formal Review → Submission |
| Social | Changes that can not be enforced by the DAO on-chain (e.g. updates to Governance Manual) | Discussion → Formal Review  |
| Consensus | Ad-hoc changes that “should” have community approval, but aren’t classified by an Executable or Social proposal | Discussion → Formal Review |

Each proposal type has a designated [template](https://github.com/radicle-dev/radicle-governance/tree/main/templates).

### Proposal Cycles

The RadicleDAO manages proposals in **monthly cycles** to sync voting periods and establish a manageable cadence for governance participants. 

| Monthly Schedule | Stage | Weekly Schedule | Action |
| --- | --- | --- | --- |
| Week 1 | Discussion | First Monday  | Post proposal to forum for Discussion |
| Week 2 | Discussion | Second Wednesday | Join monthly Proposal Review call to present and discuss proposal with community |
| Week 3 | Formal Review | Third Monday |  Open proposal for Formal Review |
| Week 4 | Submission | Fourth Monday | Submit proposal on-chain |

**Proposals can be posted to the forum for Discussion at anytime throughout the monthly cycle, but requires at least 7 days on the forum to be considered for that month’s voting cycle**

### Proposal Reviews
Proposal Reviews take place on the second Wednesday of each month. These calls are a time for proposal authors to discuss and answer questions around their active proposals that will be voted on this cycle. The calls will be recorded and archived for governance participant's reference. _Proposal authors are expected to make an effort to attend these calls and should come prepared to answer questions and discuss their proposal with attendees._

## Voting

Voting requires Radicle (RAD) tokens, which you can [obtain here](https://docs.radicle.community/governance/obtain-rad). One RAD token is equal to one vote. Voting takes place both on- and off-chain:

- **Formal Reviews:** *Off-chain* consensus checks done with [Snapshot polls](https://snapshot.org/#/gov.radicle.eth).
- **Submissions:** *On-chain* voting for RGPs take place on [gov.radicle.network](https://gov.radicle.network/#/delegates/radicle).

You can keep track of all open proposals and vote directly on the [RadicleDAO's Boardroom profile](https://boardroom.io/radicle/overview) 🌱 

### Voting Thresholds

Once proposed, participants can vote for/against the proposal on-chain with their RAD. An RGP is **approved** if it satisfies the following minimum vote thresholds:

- **Quorum:** The minimum number of total RAD votes required to be cast in connection with a proposal. Quorum is currently measured as **a % of the total RAD supply.** The required quorum to pass a proposal is **4% (4M RAD) of total supply (100M RAD)**
    
  *Formal Reviews* and *Submissions* are required to meet quorum requirements.
    
- **Approval Threshold:** If quorum is met, the proposal passes if a majority of the votes are “in-favor”.

**Proposals can be posted to the forum for Discussion at anytime throughout the monthly cycle, but requires at least 7 days on the forum to be considered for that month’s voting cycle*

**Submission triggers a 3-day voting period. If passed, the proposal is queued for 48hrs, then it can be executed.**

## Delegating

On-chain voting is enabled by delegating voting rights to the address (or addresses) of the token holder's choice:

- The owner’s own wallet, if they would like to vote on their own.
- Another user's wallet, if they would like the other user to vote on their behalf.
- No wallet, if they don't want to vote.

To participate in off-chain and on-chain voting, you have to first delegate the voting weight of your RAD. This can be done via various governance management platforms (e.g. [Boardroom](https://boardroom.io/radicle/proposals) or [Tally](https://www.tally.xyz/gov/eip155:1:0x690e775361AD66D1c4A25d89da9fCd639F5198eD)). After connecting your wallet to one of these platforms, you can choose to delegate the voting weight held in that wallet to either yourself or another address. Once delegation is completed, the voting weight of the RAD can be used to vote.

> ℹ️ Any delegation made on-chain will be mirrored to Snapshot for off-chain votes - i.e. any $RAD that is delegated to your wallet on-chain will be able to be able to be used to vote in off-chain Snapshot polls.

> In order to utilize delegated voting power in a vote, delegation needs to take place *before* the vote goes live. 

> Delegation only needs to be set up once. The only time you need to redelegate is to change or remove the address you are delegating to, otherwise delegation will continue to the asigned address.

> In addition to the Code of Conduct, Radicle Delegates are expected to adhere to our Delegate Standards, a set of requirements for ensuring healthy & safe community governance. Please review [the standards](https://govradicle.super.site/delegate-standards) before announcing yourself as a delegate 👇

### Never miss a vote! 🤳

The best way to get live governance updates is by following the Radicle Governance Twitter ([@rad_gov](https://twitter.com/rad_gov)) or follow the [🏛️governance-updates](https://discord.gg/RHp2FKV4) channel on Discord. These accounts act as governance “ticker” accounts and include all of the information and links needed to participate in voting. You can also [set up email notifications](https://app.tango.us/app/workflow/Email-Notifications-ac8d8e2eff5746f48ebd17e1f6b2b6ff) directly from the the calendar on our [Boardroom governance portal](https://boardroom.io/radicle/overview).


